# Importing your games to the arcade

Here is how to install your custom games onto the ArcadeUI
>[!NOTE]
> The games folder should be pinned to the start menu

<br>

## Step 0
ArcadeUI has support for Cover Images and Background Audio!
Here is how to create them

### Cover Image
<img src="https://github.com/vixenowo/arcade/assets/121322529/fbdeace0-1c8b-44b1-9c3b-c81eea9f47a4" width="300" height="400">
<br><br>

This will show on the game selection screen and when the game has been selected

> [!TIP]
> - **Width:** 900px width
> - **Width:** 1200px height
> - PNG, JPG/JPEG recommended

  
Images are automatically crop to fit.

<br>

### Audio
This will play when your option is hovered over on the game selector, it can be any length but shorter is better

> [!TIP]
> - Make sure not too loud or too quiet!
> - MP3 recommended

<br>

And there we are! Now for adding the game itself.

<br>

## Step 1
Create a folder in the **Games** folder, you can call it whatever but preferably named after your game

<br>

## Step 2
Put all your files into the folder, make sure that the **.exe** is in the folder you just made

> [!NOTE]
> Put the Cover Image and Audio file in the same folder

<br>

## Step 3
Create a file called `status.json` in the folder and put this inside of the file:

```
{
    "title": "[change_this]",
    "year": "[change_this]",
    "coverImage": "./Games/[your_folder]/[file_name].png",
    "description": "[change_this]",
    "soundUrl": "./Games/[your_folder]/[file_name].mp3"
}
```

> [!IMPORTANT]
> Replace all the [change_this] with any details you want about your game, the titles on the left show what to put.
> 
> Replace all the [your_folder] to the name of your folder you made.
>
> Replace all the [file_name] with the file names of your CoverImage and SoundURL, you can change the .png / .mp3 depending on which you have

Once finished, it should look like something like this this:
```
{
    "title": "Example game",
    "year": "2024",
    "coverImage": "./Games/ExampleGame/coverimage.png",
    "description": "This is an example game",
    "soundUrl": "./Games/ExampleGame/sound.mp3"
}
```

<br>

## Step 4

Test to make sure it shows up and launches as expected, if it doesnt work then try this tutorial again

If it does work, then great success!
