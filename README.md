# Adwaita for Steam

A skin to make Steam look more like a native GNOME app

<p align="center"><img src="(https://raw.githubusercontent.com/tkashkin/Adwaita-for-Steam/master/screenshot.png)](https://github.com/tkashkin/Adwaita-for-Steam/blob/master/screenshot.png?raw=true)"/></p>

## Current state and plans

* **Main Window**: Done.
* **Login**: Done
* **Library**: Done
* **Small Mode**: Done.
* **Chat**: Done
* **Settings**: Mostly done.
* **New Overlay**: Mostly done.
* **New Big Picture**: Not done.
* **Recoloring**: Colors can be changed via making a new theme. See [colorthemes](/adwaita/colorthemes) dir.
* **Light Themes**: Not currently planned, though may now be more feasible with the new UI.

### Limitations

* **Steam updates may reset theme**: While the installer will patch steam files in order to theme the interface, these files may be reset by steam updates. If this happens, you will need to reinstall to repatch them.
* **Rounded corners**: Not all elements can be rounded, use [Rounded Window Corners extension](https://github.com/yilozt/rounded-window-corners) or [mutter-rounded](https://github.com/yilozt/mutter-rounded) on GNOME.
* **Steam website pages (Store/Community/Profiles/Etc)**: No longer themable with our current method.
* **Position of notifications**: Doesn't seem to be possible to change.
* **Height of sidebar items**: Doesn't seem to be possible to increase.

## Theme Template

### General 

This repository serves as a boilerplate for themes that are compatable with Millennium. 


### Developers

This template does not rely on any 3rd party dependencies and works as is. To get started clone or use this template and place the contents in your skins folder. From there you can select it with Millennium.

Familiarizing yourself with the tree
```
Folder: Theme-Name
|    bigpicture.custom.css
|    bigpicture.custom.js
|    friends.custom.css
|    friends.custom.js
|    libraryroot.custom.css
|    libraryroot.custom.js
|    webkit.css
|    skin.json -- main directive file used by Millennium
```

With Steam started with `-dev` you can hit `CTRL+SHIFT+I` to open the inspector, and you can also use `F5` to refresh the Steam UI.
From there, you can develop your theme within the inspector. whenever you make changes you can mirror them into their respective file so it saves them.

### Advanced Setup

The boilerplate `skin.json` file provided in this template is as simple as possible to future proof it, and to make it easier for new developers. With that said, you can much further customize how your theme interacts with Steam, however we don't have documentation ready just yet. 
Check back later when this documentation is fully fledged. 
