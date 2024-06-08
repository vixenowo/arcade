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

## Step 1
Create a folder in the **Games** folder, this folder is pinned in the start menu.

> [!IMPORTANT]
> The folder **MUST** be the same name as your game .exe name or it won't show up.
> For example: if it was called test.exe then call the folder "test".

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
    "creator": "[change_this]",
    "coverImage": "./Games/[your_folder]/[file_name].png",
    "description": "[change_this]",
    "soundUrl": "./Games/[your_folder]/[file_name].mp3"
}
```

> [!IMPORTANT]
> Replace all the [change_this] with any details you want about your game, below is details on what to add
> 
> Replace all the [your_folder] to the name of your folder you made.
>
> Replace all the [file_name] with the file names of your CoverImage and SoundURL, you can change the .png / .mp3 depending on which you have

### Title
The name of your game
- **Max Length:** 100 characters

### Year
The current year you made the game, helps orginise between years
- The UI orginises by newest year

### Creator
Your name, put whatever but make sure to keep it PG
- **Max Length:** 50 characters
- It will be formatted as *Created by: (name)*

### CoverImage
Image for your game, a poster basically
- It is explained in Part 0, [here](https://github.com/vixenowo/arcade/edit/main/importgames.md#cover-image)
  
### Description
Describe your game, pretty simple
- **Max Length:** 100 characters
  
### SoundURL
The audio that plays when your game is selected
- It is explained in Part 0 again, [here](https://github.com/vixenowo/arcade/edit/main/importgames.md#audio)
  
<br>

Once finished, it should look like something like this this:
```
{
    "title": "Example game",
    "year": "2024",
    "creator": "SillyCat",
    "coverImage": "./Games/ExampleGame/coverimage.png",
    "description": "This is an example game",
    "soundUrl": "./Games/ExampleGame/sound.mp3"
}
```

<br>

## Step 4

Test to make sure it shows up and launches as expected, if it doesnt work then try this tutorial again

If it does work, then great success!
