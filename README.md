# SM64Plus Web Browser Port PoC

This is a fork of SM64Plus that attempts to make it playable in the web browser

![image](https://github.com/burnedpopcorn/sm64plus-webport-PoC/blob/master/SM64PlusPOC.png)

![image](https://github.com/burnedpopcorn/sm64plus-webport-PoC/blob/master/SM64PlusPOCSettings.png)

### AS OF 5/11/24, 

only the launcher is useable, and the game itself isn't.
- If I can get the game working along with the launcher, it will be on a different github repo, and this one will be archived (no promises)
- Why that is the case is because this repository states it is a PoC (which it is for now), but if it develops to being fully functional, it will be inaccurate to say the least
- Also music works, unlike my Pizza Tower Port (fmod sucks)

### [Download the SM64Plus Web Launcher Here](https://drive.google.com/file/d/1OPXG3rSz2o_rIA3b3S4FUOhqPOFKp9hw/view?usp=drive_link)


## To run the project (if you really want to):

- Download it and extract the .zip

### For Linux
Open the Terminal and input: { cd '[File Path to]/SM64Plus_WebBuild_POC_Dump/runner/ } (not to any specific file, just the downloaded folder and DON'T include the brackets), then:
- Input { python3 -m http.server }
- Then open a Browser and open web page https://localhost:8000/runner.html (this link you can copy if you did the previous steps)
- Then barely enjoy 

### For Windows
Open Powershell and do everything in the Linux instructions, but:
- Input { py -m http.server }, instead of { python3 -m http.server }
> [!NOTE]  
> This assumes Python is installed on your Windows Computer
>
> If not, install it, or use some other method to run a local web server
>
> As the file:// protocol (double clicking on runner.html) does not work
- Then continue with the Linux instructions (including barely enjoying)

### To Compile for Yourself
- Download the Source Code from Mors' Repository [here](https://github.com/MorsGames/sm64plus-launcher)
- Import it into the 2022 LTS version of GameMaker Studio 2
> [!WARNING]
> Using any other version of GameMaker could and most likely would create problems when compiling
- Make some changes if you want to contribute
- Compile the project using the GX.GAMES and VM Export Options (HTML will not work unless some heavy modification is done if at all)
- You can then just go to C:/Users/(your username)/AppData/Local/GameMakerStudio2-LTS/GMS2TEMP while locally running the game
- In which you will find a folder called SM64Plus_(some numbers)_VM after you compiled the project
- At which point you can copy the files to a non-temporary folder within your computer

Also the code for the actual game is [here](https://github.com/MorsGames/sm64plus), but you need your own copy of sm64 to get the all the resources to port to the web browser
> [!NOTE]
> If you will use this as a base for a full game port to go along side with this launcher, keep in mind that
> - You will need Emscripten to port it (Apparently version 1.39.5 works best, forgot where I heard that tho)
>
>  And it is very unlikely that both projects can actually communicate with each other like they're supposed to, which will make full functionality very hard to achieve without extensive work and knowledge being poured in, so good luck
> to anyone that's up to the task

### [Orginal SM64Plus Project](https://github.com/MorsGames/sm64plus)

### Credits For the Original SM64Plus:

- **Mors:** Most new things you see here!
- **[Benial](https://twitter.com/Benial17):** Logo design.
- **[Catonator](https://www.catonator.net/):** Launcher music and sound effects.
- **[deanff](https://github.com/deanff):** SM64Plus Remain Mod, which was merged in v3.0 as the more seamless progression option.
- **[sm64-port Team](https://github.com/sm64-port):** The port that was used as a base for this project.
- **[A bunch of clever folks](https://github.com/n64decomp/sm64):** The original decompilation used for the port.
- **Emil:** The original 60FPS patch.
- **Kaze Emanuar:** Providing certain bug fixes, making the original BLJ anywhere cheat, being buff.
- **[sm64gs2pc](https://github.com/sm64gs2pc/sm64gs2pc):** Used to convert the game shark codes into cheats.
- And everyone who sent pull requests or reported issues. :)
