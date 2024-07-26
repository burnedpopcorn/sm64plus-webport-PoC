# Compiling SM64Plus

> This is NOT compiling the Launcher, this is for the actual game

> [!IMPORTANT]
> This is currently a HEAVY WIP, and there are still some important things that I have to fix
>
> also I am solely using Linux Mint for this, so no Windows Compiling instructions for you

> plus I'm pretty sure Windows just uses WSL anyways

## Prerequisites

- Emscripten (v3.1.59)
> To compile the files into WebAssembly
- The Game Files and Source Code
> I have my custom Makefile that works with emcc, so download it from Releases
> 
> it is shit, and WILL make anyone with any knowledge on makefiles recoil in disgust, but it should work :)
- LibSDL
> just use Emscripten's built-in SDL package
>
> it should be auto-installed on your computer when you run my custom makefile
>
> (THIS MAKEFILE HAS NOT RELEASED YET)

## Building

1. Open Terminal
2. ```cd``` into your ```emsdk``` folder (for me, it's ```cd emsdk```)
> You should have Emscripten set up BEFORE doing any of this
3. Add Emscripten to your PATH Environment Variables by using ```source emsdk_env.sh```
4. Do ```cd``` again, and then cd into the root of the source code
5. Then type in ```emmake make TARGET_WEB=1``` to start compiling
> If something goes wrong, you should be able to do ```emmake make clean``` to wipe all progress to completely start over
>
> If that don't work, then just delete the ```/build``` directory
>
> and if the project fails to compile, make an Issue here
>
> NO NOT NOW! REMEMBER THIS IS STILL WIP

## Current Issues
There are massive issues, such as

- Graphics don't display
> Because of this, I can't really Playtest it or discover other issues

What does work is Audio and Controls, so you can still technically play it

## Botched shit I did
- removed code relating to in-game camera modes in camera.c
> did this because it caused implict function errors cuz SOMEONE decided to state variables from a different c file, and then NOT INCLUDE SAID FILE
- removed c files relating to Direct X11 and 12
> because this is Windows only APIs, so they obviously won't work
- removed wup.c
> I'm pretty it calls LibUSB, but I can't get it to find LibUSB, so it errors out, because again implict functions
>
> plus, keyboard controls still work without it, so I don't really care about it

This stuff also might be the reason why I'm getting graphics issues
