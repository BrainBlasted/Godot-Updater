# Godot Updater

This is a simple bash script to update [Godot](https://github.com/godotengine/godot). It pulls the latest commits from master, then compiles the targets. Optionally can compile export targets for Linux/X11 and Windows.

## Dependencies
- Clang
- Scons
- Mingw64 (for building Linux targets)

## Usage
   1. With your editor of choice, set `$GDPATH` to where you have git cloned the godot source to, ex. `~/godot`
   2. Place the script in a folder where bash can find it. You can change this through your `~/.bashrc` file.
   3. Make sure to give the script executable persmissions, and then you can call `update-godot` from the terminal.
   4. Copy the `godot` file in `$GDPATH/bin` to where you'd like to launch it from, and move your export templates where Godot can find them.
   5. Optionally, make a .desktop file to launch Godot from that path.
## Issues
- Current builds cannot be double clicked from the file manager to run. This can be worked around by calling the full path to godot when you want to run it, or making your .desktop file for godot call the full path.
- Building the editor or export templates may sometimes fail. This is due to changes in godot code not always working out.
