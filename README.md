# Quake Yam Setup


## Setup

### Install Quake source port
   
   There are very (very) many source ports to choose from. Pick whichever you like. If you have no preference you can try:

- `sudo apt install quakespasm`
- https://github.com/andrei-drexler/ironwail


### Install Trenchbroom
- Cop from the [releases](https://github.com/TrenchBroom/TrenchBroom/releases) page on GitHub or the [Flatpak](https://flathub.org/apps/com.kristianduske.TrenchBroom).

### Install map compilation tools

- Think of Trenchbroom like your code editor and ericw-tools as your compiler.
- Clone [ericw-tools](https://github.com/ericwa/ericw-tools)

### Obtain Quake game files

[piracy is a serious crime](https://archive.org/details/quake_dos)

Your source port will expect your ill-gotten gains to be in a particular directory and will automatically load them on startup. If it can't find it every source port should have a command-line parameter to specify the directory of your WADs.

### Download Quake Textures

In addition to the original Quake game files, you will need textures which can be found [here](https://www.quaddicted.com/files/wads/base.zip).

### Mix and serve

In your Trenchbroom preferences, set the Game Path to the binary of your Quake source port, and set the respective paths for each of the compilation tools (`qbsp`, `vis`, and `light`).

Here's an example of the correct preferences in Trenchbroom, where the `quake` directory is your game files (i.e the contents of the archive.org download) 
![image](https://github.com/ranguli/quake-jam-2024/assets/5544782/73ad01c4-2d3a-4126-9ef3-281af038034d)

### Test drive

You can [download](https://rome.ro/news/2016/2/14/quake-map-sources-released) the original Quake 1 map source files and use them both as reference for level-design and as a way to test that your setup and workflow and working and flowing.



## Setting a Quake engine in Trenchbroom

Select "Run > Launch Engine" from the menubar in TrenchBroom.

![image](https://github.com/ranguli/quake-jam-2024/assets/5544782/5de5716a-af30-4c05-a7eb-7686b59b07b5)

Select "Configure engines...", then create a profile. Add a name for the engine (like the name of your source port) and set the path to the executable of the source port.

![image](https://github.com/ranguli/quake-jam-2024/assets/5544782/29cf08cb-f3b7-4f62-b1c7-02edb6e007d4)



## Opening a map in TrenchBroom

In TrenchBroom, open `E1M1.WAD` from the download in Step 7 of the setup. 

**Ensure you select Quake for the game, and "Standard" for the Map Format!**


![image](https://github.com/ranguli/quake-jam-2024/assets/5544782/bf425c27-920d-41ff-a6b5-6dede7147898)

You should see the geometry of the map, as well as some of the 3D models in the "Entity" tab of the sidebar. If you don't see both of these, something went wrong.

![image](https://github.com/ranguli/quake-jam-2024/assets/5544782/a2862969-b242-4c15-a846-93e358532a2f)

### Getting map textures to work
In order to address the missing textures from the map, select the "Face" tabe in the sidebar. Under Texture Collection, click "Show". Click the "+" icon to add a Texture Collection, and select the `base.wad`  file downloaded in step 5. 

Upon successful completion of this step, the map will now have textures. 

![image](https://github.com/ranguli/quake-jam-2024/assets/5544782/bfdd8bf8-af12-430f-aa1f-740bd3235afe)

You can follow along this same process when creating a new map as well. 

## Compiling a map from TrenchBroom
Maps must be compiled beforet they can be played in Quake.

[See the Wiki article](https://github.com/ranguli/quake-jam-2024/wiki/Compiling-a-map-in-TrenchBroom)



## Troubleshooting

For common issues, see the [Wiki article](https://github.com/ranguli/quake-jam-2024/wiki/Troubleshooting) on troubleshooting.
