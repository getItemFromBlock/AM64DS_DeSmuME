# DeSmuME with Analog Hack for SM64DS

This is a modified version of the [DeSmuME emulator](https://desmume.org/) which can be use to play Super Mario 64 DS with an analog stick. This is a drop-in replacement for official releases and includes all the changes of the recent development version.

## How To Use

Using the analog stick with Super Mario 64 DS requires a few steps to set it up.

### Download the Latest Releases

This is to make sure you have any support files needed for the emulator. You can download the latest release build from https://desmume.org/download/ under "Stable Releases".

### Download the Modded Emulator Build

Download the modded emulator build from [the Release page](https://github.com/LRFLEW/desmume/releases/latest) and replace the release exe with the the downloaded version.

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

### Apply the game patch (cheat code)

Open the game ROM (File -> Open ROM...) and go to Tools -> Cheats -> List. Find the code needed for your game version from [the CHEATS page](CHEATS.md) and add the code as an "Action Replay" cheat code. Make sure the cheat is enabled and click Save.

---

At this point, everything is setup to use the analog stick mod. If you you close the game or emulator, you just need to reopen the game or emulator and the mod will still be applied. If you wish to play the game with the original control scheme again, disable the cheat code in the cheats lists, close, and reopen the ROM.