# RetroArch Passthrough

Arcadium detects .exe's located in the Games folder, however if you are familiar with emulated games such as with RetroArch they are not exe's 
(well the emulators themselves are) but the games themself arent, so if you just had the RetroArch program in the Games folder then
you'd have to go through 2 game pickers

HOWEVER 

With the Arcadium Passthrough™ application, it opens a specific game on the emulator directly from Arcadium

*RetroArch supports parameters to launch games directly so check that documentation*

## All you have to do

BUG: with the current iteration, it doesnt work when running on the UI but I cba to fix it so adjust the code in visual studio to what the folder for your game is called (such as ../mygame/gamelocation.arcade) for the 2 variables on the top

then you can change the `GAMELOCATION.ARCADE` to the url of where RetroArch is

**Make sure its the / and not \ slashes.**

and for launch parameters, change `PARAMETERS.ARCADE` and include them depending on what you need (check retroarch docs)

and thats it! Make sure you got the launch parameters correct and make sure that you add the Passthrough into the games folder
Feel free to remove the text file when finished, dont remove other files though.

## Installation

**DONT FORGET TO ADD A INFO.JSON!! else itll show as nothing and may break**
Add this for the specific game it launches

1 passthrough exe per game (so multiple folders for different games with passthrough exe but info.json adjusted for the game it launched)

Follow this guide: [Install Guide](https://github.com/vixenowo/arcade/blob/main/importgames.md#then-next "Install Guide")
