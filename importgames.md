# Importing your games to the arcade

So you want to add your own game to the arcade, heres a step by step tutorial to not explode things.

> The "Games" folder can be accessed by closing the UI > Start Menu > Games folder (should be pinned)

## First things first:
1. Create a subfolder in the Games folder (name it anything)
2. Import your files (exes, folders, etc.)

## Then next:
Create a file called
` info.json `
or just nick one from another game and copy n paste to your folder (with ur game in)

if you copied it, it should look something like this: 
```
{
    "title": "My Game",
    "description": "This is an exciting game.",
    "author": "arcadian",
    "icon": "https://cdn-icons-png.flaticon.com/512/742/742263.png",
    "banner": "./Games/game2/icon.png"
}
```
or if you made it new then **copy this code in** (including the brackets)

![warn](https://github.com/vixenowo/arcade/assets/121322529/9bc502e0-ad7d-415b-85a5-8fd86a77e6e1)


## After you done adding the info.json and content 
Now you can edit the values to be about your game, its important that you make sure to keep the " " inbetween and such.

> Do NOT use vertical line ( | ) for any names, authors, description, etc. this will cause problems as its a reserved character

### Title
Self explainitory, it isnt recommended to make it too long as it will be cut off if too long.

### Description
Also self explanitory.

### Author
This shows as *Created by (your author name*, pick anything PG i guess

### Icon
This is the cover art in the game picker

- Minimum size: 200px by 300px (width, height)
- Recommended size: 800px by 1200px (width, height)

Any lower will make it blurry and too high quality can cause it to load slowly

![image](https://github.com/vixenowo/arcade/assets/121322529/94ce65a7-f07a-430f-97a1-8c0412d63c52)

### Banner
This is the image that shows up when your game is hover overed (itll show your game details on hover too)

- Recommended size: 2600px by 673px (width, height)

Take note of the fade on the left too

![image](https://github.com/vixenowo/arcade/assets/121322529/189bc3d1-a1b3-4ad2-a3fb-4757515c879c)

### Adding images

If your getting an image from a website then just put the link to the image in there (the image, not the webpage)
but if your adding your own image then put it in the same folder as exe and json, you can call it anything and in the json file put

`"./Games/game2/icon.png"`
(replace game2 and icon.png with what you called your folder and image)

## Congrats
The program should automatically detect the files and show up in the game
