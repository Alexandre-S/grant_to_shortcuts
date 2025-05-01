# grant_to_shortcuts
CK3 mod to add shortcuts on granting title to local vassal, default is `G` to grant, then `H` on the next window to grant to a local culture noble of your faith.

Shortcuts can be changed in the `shorcuts.shortcuts` file. You can also bind the same key, so you can two tap the key to grant fast

# Requirement

Unfortunately CK3 doesn't allow modding on the shortcut file `Crusader King III/game/gui/shorcuts.shortcuts`, You'll have to modify it by hand, or replace it with [mine](https://raw.githubusercontent.com/Alexandre-S/grant_to_shortcuts/refs/heads/main/grantToLocal_shortcut/gui/shortcuts.shortcuts), otherwise the shortcuts won't work.

To find it, navigate to your local gamefile installation (On steam, right click on the game, properties, local files, browse local files)

Typically, installation should be `C:\Program Files (x86)\Steam\steamapps\common\Crusader Kings III\`

Then, navigate to `game\gui` folder to find `shorcuts.shortcuts` file.

Replace the file with mine, or open it with a text editor like notepad++, and add those lines

```
# Grant title
	grant_to = "G"
	grant_title_local = "H"
```

at the bottom of the file, **BEFORE** the last brace

![Example of shortcut file.](/pics/example_shortcuts.png "Example of the shortcut file.")

**NOTE: When updating your game, of the mod, you may have to redo this step again.**

# Manual installation

- Download the package

- Extract the `grantToLocal_shortcut` folder to this location (replace `YOURUSERNAME` with your windows user account name) : `C:\Users\YOURUSERNAME\Documents\Paradox Interactive\Crusader Kings III\mod`

- In your `Documents\Paradox Interactive\Crusader Kings III\mod` folder, you have to create a file named `grantToLocal_shortcut.mod`, and paste inside this content (again, replace `YOURUSERNAME` with your windows user account name)

```
version="0.1"
tags={
	"Utilities"
}
name="grantToLocal_shortcut"
supported_version="1.15.0.2"
path="C:/Users/YOURUSERNAME/Documents/Paradox Interactive/Crusader Kings III/mod/grantToLocal_shortcut"
```
- Save the file, launch the game, add the mod to a playlist, enjoy :)
