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

