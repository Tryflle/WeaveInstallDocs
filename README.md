# Overview
- Weave is a mod loader aimed to work everywhere. https://github.com/Weave-MC
- Weave is it's own mod loader, forge/fabric mods won't work unless they have been ported.
# Support for
1. Stable
   - Lunar Client
     1. 1.8.9
2. Module testing branch with Weave Manager Tauri
   - Labymod
   - Lunar Client
   - Forge
   - Vanilla
     1. 1.7.10
     2. 1.8.9
     3. 1.12.2
- Weave Manager Tauri is currently in beta, but set to supercede the buggy and unusable Weave Manager Electron.
# Installation Methods for Weave Loader
- Lunar Client Qt (any version or fork, including 2.0 and the original)
  1. Download the latest release of Weave Loader and add it as an agent https://github.com/Weave-MC/Weave-Loader/releases
  2. Create the folder `.weave` and inside `mods` in your user profile path
     - Windows: Windows+R, type `%userprofile%`, create the directories there
     - Unix: `mkdir -p ~/.weave/mods`
  3. In this folder add your mods
  4. Launch!
- Lunar Launcher Inject
  1. Download the latest release from https://github.com/Nilsen84/lunar-launcher-inject/releases for your operating system.
  2. Make a new directory anywhere, and put the file you downloaded inside
  3. Download the latest Weave Loader https://github.com/Weave-MC/Weave-Loader/releases and put it in the same folder.
  5. Open Lunar's launcher normally, then disable exit to dock and close it, ensure it's not running in the background, if it is you'll want to kill it.
     - Windows: Open Lunar Launcher Inject
       1. Launch!
     - Unix: Set your current directory to the directory with Lunar Launcher Inject, then run `chmod +x nameoflliexecutable`
       1. `./nameoflliexecutable`
       2. Launch!
- Command Line Interface (Windows)
  1. Download Process Hacker https://processhacker.sourceforge.io/
  2. Run Lunar
  3. Right click the process and go to properties
  4. Copy the launch command and save it in notepad as a `.bat`.
  5. A little after Java is defined add `-javaagent:"path/to/agent.jar"` https://github.com/Weave-MC/Weave-Loader/releases
  6. Launch
 - Weave Diagnose
   1. Create the folder `.weave` and inside `mods` in your user profile path
     - Windows: Windows+R, type `%userprofile%`, create the directories there
     - Unix: `mkdir -p ~/.weave/mods`
   2. Within your .weave folder, add the Weave Loader Agent, don't put it in the mods folder. https://github.com/Weave-MC/Weave-Loader/releases
   3. Download Weave Diagnose from https://gitlab.com/candicey-weave/weave-diagnose/-/releases
   4. Double click Weave Diagnose jar and add your mods to the `.weave/mods` folder, hit run Weave when ready and that's it.
# Installion Method for Weave Manager
- Weave Manager Electron
  1. Note: Weave Manager Electron is very buggy and I don't recommend it.
  2. Install the corresponding version for your operating system from https://github.com/exejar/Weave-Manager/releases
  3. Add your mods to:
     - Unix: `~/.weave/mods`, create it if it does not exist.
     - Windows: Press Windows + R, then in the run dialogue type `%userprofile`, look for `.weave`, if it doesn't exist create it and inside make a folder called mods, the full path is `%userprofile%/.weave/mods`
  4. Run it and launch lunar then hit relaunch with Weave.
  5. Enjoy, if it works.
- Weave Manager Tauri
  Soon™
