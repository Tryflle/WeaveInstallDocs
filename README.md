<img
    align="right" alt="title" width="200px"
    src="https://raw.githubusercontent.com/Weave-MC/.github/master/assets/icon.png"
/>

# Weave, A Universal Minecraft Mod Loader
- Note: Weave is it's own Mod Loader, forge/fabric mods are not compatabile and must be ported.

## Weave Supports:
### Stable (v0.2.4):
<table>
<tr><th>Supported Clients</th><th>Supported Versions</th></tr>
<tr><td>
        
| Client  | Supported |
| ------- | :-------: |
| Vanilla | ❌ |
| Forge   | ❌ |
| Lunar   | ✅ |
| Badlion | ❌ |
| Feather | ❌ |
| Labymod | ❌ |

</td><td>
    
| Version | Supported |
| ------- | :-------: |
| 1.7     | ❌ |
| 1.8     | ✅ |
| 1.12    | ❌ |
| 1.16    | ❌ |
| 1.17    | ❌ |
| 1.18    | ❌ |
| 1.19    | ❌ |
| 1.20    | ❌ |
</td></tr>
</table>

### Beta Branch with Weave Manager Tauri:
<table>
<tr><th>Supported Clients</th><th>Supported Versions</th></tr>
<tr><td>
        
| Client  | Supported |
| ------- | :-------: |
| Vanilla | ✅ |
| Forge   | ✅ |
| Lunar   | ✅ |
| Badlion | ❌ |
| Feather | ❌ |
| Labymod | ✅ |

</td><td>
    
| Version | Supported |
| ------- | :-------: |
| 1.7     | ✅ |
| 1.8     | ✅ |
| 1.12    | ✅ |
| 1.16    | ❌ |
| 1.17    | ❌ |
| 1.18    | ❌ |
| 1.19    | ❌ |
| 1.20    | ❌ |

</td></tr>
</table>

- Weave Manager Tauri is currently in beta, but set to supercede the buggy and unusable Weave Manager Electron.
## Mod information
- Directory: `~/.weave/mods`//`%userprofile%/.weave/mods`
- Mods must be made for Weave. You can find mods in the Discord server https://discord.gg/zzncWwGg5X or https://efo-chi.vercel.app/ , however, the latter has been deprecated.
## Installation Methods for Weave Loader
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
     - Unix: Set your current directory to the directory with Lunar Launcher Inject, then run `chmod +x nameoflliexecutable` (Please note, Mac users will have to rename the executable in order to remove all dots otherwise it will not work.)
       1. `./nameoflliexecutable`
       2. Launch!
- Command Line Interface (Windows)
  1. Download Process Hacker https://processhacker.sourceforge.io/
  2. Run Lunar
  3. Right click the process and go to properties
  4. Copy the launch command (general -> command line) and save it in notepad as a `.bat`.
  5. In the `.bat`, just after Java is defined add `-javaagent:"path/to/agent.jar"` https://github.com/Weave-MC/Weave-Loader/releases
  6. At the very end, on a new line, write `pause`.
  7. Save the file
  8. Open the file, and you've launched lunar!
 - Weave Diagnose
   1. Create the folder `.weave` and inside `mods` in your user profile path
     - Windows: Windows+R, type `%userprofile%`, create the directories there
     - Unix: `mkdir -p ~/.weave/mods`
   2. Download Weave Diagnose from https://gitlab.com/candicey-weave/weave-diagnose/-/releases
   3. Double click Weave Diagnose jar and add your mods to the `.weave/mods` folder, hit run Weave when ready and that's it.
- Command Line Interface (Linux)
  1. Run Lunar
  2. Open your terminal and run `ps aux | grep lunar.jar`
  3. Copy the command and add it to a `.sh` script
  4. In the `.sh`, just after Java is defined add `-javaagent:"path/to/agent.jar"` https://github.com/Weave-MC/Weave-Loader/releases
  5. Create the folder `.weave` and inside `mods` in your user profile path, to do this run: `mkdir -p ~/.weave/mods`
  6. Add your mods to the folder and then run the `.sh` script.
## Installion Method for Weave Manager
- Weave Manager Electron
  1. Note: Weave Manager Electron is very buggy and I don't recommend it as it usually fails to relaunch and uses excess amounts of resources. You should use Weave Loader instead.
  2. Install the corresponding version for your operating system from https://github.com/exejar/Weave-Manager/releases
  3. Add your mods to:
     - Unix: `~/.weave/mods`, create it if it does not exist.
     - Windows: Press Windows + R, then in the run dialogue type `%userprofile`, look for `.weave`, if it doesn't exist create it and inside make a folder called mods, the full path is `%userprofile%/.weave/mods`
  4. Run it and launch lunar then hit relaunch with Weave.
  5. Enjoy, if it works.
- Weave Manager Tauri (Windows) (BETA)
   1. Download it:
     - [Here is a version that I compiled.](https://github.com/Tryflle/WeaveInstallDocs/releases/tag/newtauri)
   2. Building it:
     - https://github.com/Weave-MC/Weave-Manager Download the source code.
     - Download NodeJS
     - Download RustUp
     - Download VCC Build tools (12GB+)
     - Open CMD and change your current directory to the folder containing index.html and whatnot, to do this run `cd PATH`, PATH being the path to the folder.
     - Run `npm i`, and then `npm run tauri build`
     - Grab some water and develop patience.
     - Once your build is finished, you may get an error about keys, ignore it.
     - Navigate to `src-tauri\target\release` and `Weave Manager.exe` is it!
     - I have found Weave Manager Tauri to be very reliable and easy to use, minus the build tax.
   3. Usage:
     - Add your mods to `%userprofile%/.weave/mods`
     - Launch Lunar
     - Hit relaunch
     - Inquire Candice about using the beta branch if you wish to use it. The best place to do this would be in the help channel. I personally have not tried the beta branch.
