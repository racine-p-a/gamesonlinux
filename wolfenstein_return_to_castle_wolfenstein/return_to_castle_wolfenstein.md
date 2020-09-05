# Installation

In order to play Return to Castle Wolfenstein, you need two things : the engine and the game files.

## Get the engine

Grab the files from [the releases page](https://github.com/iortcw/iortcw/releases). While I am writing, the last
release is the 1.51.c. Download it.

### Which file ?

I assume that you are a linux user (it's the point of this project), so you must choose one of the two linux files.

- iortcw-1.51c-linux-x86.zip
- iortcw-1.51c-linux-x86_64.zip
 
The first one will always work (but not always as efficiently as it could be). The second works only for 64 bits
processors (most recent PC).
In other words, if you have a r/d-ecent PC, pick the [...]linux-x86_64.zip. Otherwise pick the first one (for potato
computers).

Extract the archive where you want Wolfenstein installed. If you want to launch the game in single player mode,
use this commandes :

```shell script
cd path/to/your/wolfenstein/folder/ # This folder must contains two folders named Docs and main.
./iowolfsp.x86_64 # If you downloaded the second archive.
```

Aaaaaaaaaaaand it failed. Because you only have the engine files. Now you need to get the game data.


## Get the data files

You still need the game files, the .pk3 files.

### You do have a legal version of the game

Install it somewhere.

* on your own linux computer using wine or steam
* on a windows system (then copy it on USB stick/GoogleDrive/whatever way you prefer)

Then copy the .pk3 files and paste them in the folder named _main_ of therelesa

### You do not have a legal version

Well... I am preparing something


# Launching

Juste execute the launcher :

```shell script
./iowolfsp.x86_64 # If you downloaded the second archive.
```

# Mod support

YES ! MODS ARE SUPPORTED !

Download your mod and place its folder in your game folder.


piste : 
https://github.com/id-Software/RTCW-SP
http://zerowing.idsoftware.com/linux/wolf/