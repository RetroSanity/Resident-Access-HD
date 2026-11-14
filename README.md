# Resident Access HD

A screen reader mod for Resident Evil HD Remaster (Steam, PC) that lets blind players play the whole game with an Xbox controller.

It reads the game out loud through your screen reader (NVDA, JAWS, ZoomText, System Access and others) or, with none running, through Windows' own voices. It also tells you what is in each room and can walk you to anything in it.

[Download the latest version](https://github.com/RetroSanity/Resident-Access-HD/releases/latest)

## What it does

- Reads the game: title screens and menus, the Option menu and the values on its screens, New game setup, difficulty and Character select, load and save slots, every message and question, cutscene subtitles, your items, files, the item box, the status screen, and puzzle screens such as the lab computer and keypads.
- Room lists: everything in the room you are in, in five lists: Doors, Items, Things to check, Puzzles and Enemies. Each one comes with its distance and direction ("13 metres, ahead and to the right"). Puzzles explain how they are done, and where order matters the next step is listed first.
- Auto walk: pick anything in the list and the mod walks you there. It goes round walls, furniture and enemies, and through stairs, ladders and doors within a room. Hold the run button to run. Works with both control schemes, Original and Alternate.
- 3D beacon: if you'd rather walk yourself, follow a sound placed all round you on headphones (OpenAL Soft with HRTF). It leads you round obstacles to where you want to go, turn by turn. Behind you the knock is lower. On the Alternate controls the sound is placed the way the stick walks you: in front means push up.
- Combat: names the enemies in the room with their health. A soft aim beep rings when a shot would hit. On Plant 42, the aim stays on the bulb and the mod tells you how far it is.
- Jill and Chris: both characters work.
- Updates itself: it checks for a new version each time it starts. If its files are ever broken, it downloads them again.

## Requirements

- Resident Evil HD Remaster on Steam, on Windows 10 or 11
- An Xbox controller (or any controller the game sees as one)
- A screen reader is recommended; without one, Windows' voices are used
- Nothing else: Python comes with the mod

## Installing

1. Download the zip from the [latest release](https://github.com/RetroSanity/Resident-Access-HD/releases/latest) and unzip it anywhere, for example in Documents.
2. Run Install Resident Access.bat. It finds the game through Steam and adds a small controller add-on to the game's folder.
3. Start the game from Steam. The mod starts with it and says "Resident Access ready".
4. Keep Subtitles on in the game's options. Auto walk and the 3D beacon work with either control scheme, Original or Alternate.

## Controls

Hold the left bumper and use:

| Button | What it does |
| --- | --- |
| D-pad left and right | Previous and next list |
| D-pad up and down | Previous and next thing in the list |
| Left stick press | Auto walk to it |
| Right stick press | 3D beacon to it (again to stop) |
| B | Stop walking |
| Y | Where it is again |
| X | Your health |
| A | The room and its doors |
| Right bumper | Enemies in the room |

The game ignores these buttons while the left bumper is held. There are keyboard keys for everything too: see README.txt in the download.

## Updating and uninstalling

- The mod updates itself when it starts. Update Resident Access.bat checks straight away. Your settings are kept.
- To remove it, run Uninstall Resident Access.bat, then delete the folder.

## Reporting a problem

The mod writes everything it says, and any errors, to rehdaccess.log in its folder. The session before is kept as rehdaccess.old.log. Please attach both, and say where in the game you were, when you report a problem in [Issues](https://github.com/RetroSanity/Resident-Access-HD/issues).

## Credits

- [OpenAL Soft](https://openal-soft.org/) for the 3D sound (LGPL)
- [Prism](https://github.com/ethindp/prism) for screen reader and Windows voice support (MPL 2.0)
- NVDA Controller Client for speech through NVDA

Their licences are in the `lib` folder of the download.
