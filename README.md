# SM64Plus Web Browser Port PoC

This is a fork of SM64Plus that attempts to make it playable in the web browser

### AS OF 5/11/24, 

only the launcher is useable, and the game itself isn't.
- If I can get the game working along with the launcher, it will be on a different github repo, and this one will be archived (no promises)
- Why that is the case is because this is PoC (for now), which if it develops to being fully functional, will be inaccurate to say the least

### [Download the SM64Plus Web Launcher Here](https://drive.google.com/file/d/1OPXG3rSz2o_rIA3b3S4FUOhqPOFKp9hw/view?usp=drive_link)
### To run the project (if you really want to):

- Download it and extract the .zip

### For Linux
Open the Terminal and input: { cd '[File Path to]/SM64Plus_WebBuild_POC_Dump/runner/ } (not to any specific file, just the downloaded folder), then:
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
