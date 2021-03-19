# DeSmuME with Analog Hack for SM64DS

This is a modified version of the [DeSmuME emulator](https://desmume.org/) which can be use to play Super Mario 64 DS with an analog stick. This is a drop-in replacement for official releases and includes all the changes of the recent development version.

To play SM64DS with an analog stick, it requires a small patch to the game, which can be applied either as a cheat code or by applying an IPS patch file to the ROM. The provided patch also put camera rotation controls on the D-Pad so you can control it without using the touchscreen.

## How To Use

Using the analog stick with Super Mario 64 DS requires a few steps to set it up.

### Download the Latest Releases (optional)

The v0.9.11 release of DeSmuME includes additonal files, such as a database file, that you might want to have. These files appear to be optional, though.

You can download the latest release build from https://desmume.org/download/ under "Stable Releases".

### Download the Modded Emulator Build

Download the modded emulator build from [the Release page](https://github.com/LRFLEW/desmume/releases/latest) and replace the release exe with the the downloaded version.

NOTICE: The original and modified DeSmuME emulators are licensed under the GNU General Public License v2.0. The text of this license is available [here](https://github.com/TASVideos/desmume/blob/master/license.txt).

### Enable the Analog Stick

Before opening DeSmuME, connect your controller with an analog stick you want to use. Open DeSmuME, go to Config -> Slot 2 (GBA slot), and in the window that opens select "Analog Stick" from the dropdown menu.

### Configure the Analog Stick

In the GBA slot window, you can configure how the analog stick works.

The "Left" and "Up" settings changes what's used for the horizontal and vertical axis respectively. The default is to use what is the left analog stick on most controllers. This setting also allows you to mirror the direction. For example, if you configure "Left" to be "(J0)Right", the horizontal axis will be mirrored.

Deadzone configures the range of inputs that are assumed to be centered in percent. Most controllers don't rest perfectly centered, so the deadzone accounts for that.

The two checkboxes modify how the deadzone works. "Joined Deadzone" changes whether each axis has its deadzone applied individually or together. When the option is deselected, the deadzone can be applied to one axis but not the other (which helps with holding straight up, left, down, or right), while selected means that if either axis is out of the deadzone, the deadzone isn't applied to either axis. "Circular Deadzone" modifies a joined deadzone to use the distance from the center point to determine if the deadzone should be active.

### (Optional) Switch GBA slot to Auto

If you want to play other games that use the GBA slot with the emulator, you can change the setting to Auto at this point. The emulator will use the Analog Stick option when playing SM64DS. If you only plan on playing SM64DS with the emulator, it's recommended to leave this option on "Analog Stick"

### (Optional) Configure button controls

At this point, you likely want to switch the other controls to use the same controller as the analog stick. This can be done in Config -> Control Config. If you've already configured the controls how you want, you can skip this step.

**Note:** The D-Pad is used to rotate the camera (in Standard Mode), so it's recommended to not map the D-Pad to the same analog stick configured in the GBA-slot window. You can map the D-Pad to another analog stick, such as the right analog stick, if you want to control the camera with it.

### Apply the game patch (cheat code or IPS patch)

You need to patch the game to read the analog stick values from the emulator. There are two ways of doing this: Applying a ROM patch or using a cheat code.

To use the ROM patch, Download the IPS file for your version of the game from [the PATCHES page](PATCHES.md) and apply it to your ROM file using an IPS patching tool, such as [Marc Robledo's browser tool](https://www.marcrobledo.com/RomPatcher.js/).

To use the cheat code, open the game ROM (File -> Open ROM...) and go to Tools -> Cheats -> List, find the code needed for your game version from [the PATCHES page](PATCHES.md), and add the code as an "Action Replay" cheat code. Make sure the cheat is enabled and click Save to apply it.

---

At this point, everything is setup to use the analog stick mod. If you you close the game or emulator, you just need to reopen the game or emulator and the mod will still be applied. If you wish to play the game with the original control scheme again, disable the cheat code in the cheats lists, close, and reopen the ROM.