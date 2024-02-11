# Quake Yam Setup

## 1. Install Quake source port

There are very (very) many source ports to choose from. Pick whichever you like. If you have no preference you can try:

- `sudo apt install quakespasm`
- https://github.com/andrei-drexler/ironwail


## 2. Install Trenchbroom
- Cop from the [releases](https://github.com/TrenchBroom/TrenchBroom/releases) page on GitHub or the [Flatpak](https://flathub.org/apps/com.kristianduske.TrenchBroom).

## 3. Install map compilation tools

- Think of Trenchbroom like your code editor and ericw-tools as your compiler.
- Clone [ericw-tools](https://github.com/ericwa/ericw-tools)

## 4. Obtain illegal Quake 1 game files from guli or the internet

[piracy is a serious crime](https://archive.org/details/quake_dos)

Your source port will expect your ill-gotten gains to be in a particular directory and will automatically load them on startup. If it can't find it every source port should have a command-line parameter to specify the directory of your WADs.


## 5. Mix and serve

In your Trenchbroom preferences, set the Game Path to the binary of your Quake source port, and set the respective paths for each of the compilation tools (`qbsp`, `vis`, and `light`).

## 6. Test drive

You can [download](https://rome.ro/news/2016/2/14/quake-map-sources-released) the original Quake 1 map source files and use them both as reference for level-design and as a way to test that your setup and workflow and working and flowing.


## Troubleshooting

### TrenchBroom says: Could not load texture collection 'gfx/base.wad': Cannot open file 
This means your paths for your Quake game files (pak0.pak and pak1.pak) aren't right, or maybe your .pak files aren't any good.
