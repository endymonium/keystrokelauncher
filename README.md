# Keystroke Launcher

![logo](images/avatar.jpg)

Execute commands fast, no need to clutter your desktop with a lot of icons, just remember the name and execute it directly!

* **Fast and small footprint**
* **Frequency based search results**
* **Configuration UI**
* **Configurable look and feel**

Idea based on the awesome keystroke launcher for Windows [Keyperinha](http://keypirinha.com/). Does not work in combat, due to Blizzard API limiations. Needs one free slot in the "General" macro tab.

## Quickstart

1. Press `ctrl+alt` to open the window
2. Type something
3. Press *Enter*, the first entry will be executed

To change the keybinding go into the configuration menu: `ctrl+alt` --> type in `kl` --> select `kl show` --> `Enter`

**Tipps:**

* Use the *Up/ Down* keys to select a different item. Or use the mouse abd clicking on it.
* Search database is refreshed once at login time. Can also manually be refreshed using the button in the configuration ui.

**How To:**

* [Associate a keyword to an item](docs/assoc.md)
* [Edit the search index or add new items](docs/edit.md)
* [Experimental: quick search type filter setting](docs/quick.md)

## The search index can contain

* (*) All spells which are castable and not passive
* All addons as long as they have a slash command registered and are enabled/ loaded
* All macros
* (*) A few additnioal commands like reload, logout, dismout, kl show
* (*) All inventory items which are usable
* (*) All mounts
* (*) Equipment Sets
* (*) Blizzard Unit Frames

(*) enabled by default, for the rest go into the configuration window.

## Gotchas& Known Issues

* Addons are executed as `/(addon name in lower case)`, therefore will not work for addons with a diffent slash commands. See [here](docs/edit.md) how to edit the search database.
* The way the up/down keys work is very basic, it does not handle resizing, manual scrolling using the mouse wheel, etc.
* Creating clickable icons for every item leads to lag when opening up the main window. Therefore it is currently limited to the first 10 items.
* I think there is a memory leak somehwere, at least the memory consumption rises everytime you open/ close the main window.

## Let me know if you find any bugs or have a feature request :)
