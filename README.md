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
;)

Your source port will expect your ill-gotten gains to be in a particular directory and will automatically load them on startup. If it can't find it every source port should have a command-line parameter to specify the directory of your WADs.


## 5. Mix and serve

In your Trenchbroom preferences, set the Game Path to the binary of your Quake source port, and set the respective paths for each of the compilation tools (`qbsp`, `vis`, and `light`).

Try opening the maps from the Quake WAD to get a feel for the workflow. The game files for Quake are typically under an `id1` subdirectory, and consist of a `pak0.pak` and a `pak1.pak` file. These are just renamed `.zip` files.
