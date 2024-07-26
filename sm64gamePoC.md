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
> I have my custom Makefile that works with emcc, so gonna upload it when I can fix current issues
> it is shit, and WILL make anyone with any knowledge on makefiles recoil in disgust, but it should work :)

Other Probably needed Dependencies

- LibUSB        (sudo apt-get install libusb1.0)
- LibSDL2       (sudo apt-get install libsdl2-dev)
> I say should, because it is possible to compile it without them, but having them missing is probably the reason why I'm having issues

## Building

1. Open Terminal
2. ```cd``` into your ```emsdk``` folder (for me, it's ```cd emsdk```)
3. Add Emscripten to your PATH Directory by using ```source emsdk_env.sh```

shit, i gotta end it here, sorry

will update in due time
