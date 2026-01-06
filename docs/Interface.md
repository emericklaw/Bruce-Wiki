![Interface options](https://raw.githubusercontent.com/pr3y/Bruce/main/media/pic3.png)

# Keyboard shortcuts (Cardputer only)

When you are on the main menu of Bruce, you can utilize the following keyboard shortcuts:

- `i` : Navigate to IR codes.
- `r` or `s` : Navigate to RF codes.
- `b` : Navigate to BadUSB.
- `w` : Navigate to WebUI.
- `f` : Start the file manager on SD card (if present).
- `l` : Start the file manager on LittleFS.

After [#1488](https://github.com/BruceDevices/firmware/pull/1488), you can now customize these keys with a `/shortcuts.json` file.

example:

```js
{
    "f": "loader open files",
    "i": "loader open ir",
    "r": "loader open rf",
    "b": "loader open badusb",
    "w": "loader open webui",
    "c": "loader open config",
    "1": "rf tx_from_file BruceRF/plug1_on.sub",
    "2": "rf tx_from_file BruceRF/plug2_on.sub",
    "t": "ir tx_from_file BruceIR/tv_telefunken_power.ir",
    "l": "ir tx_from_file BruceIR/desklamp_off.ir",
    "L": "ir tx_from_file BruceIR/desklamp_on.ir"
} 

````

The action string on the right can be [any supported serial command](https://github.com/BruceDevices/firmware/wiki/Serial).

 > [!TIP]
> Uppercase/lowercase letters are considered different and so can have different actions associated. Symbols are also supported as trigger keys.


While inside any app these shortcuts are no longer active.

In the file picker you can cycle filenames by pressing the initial letter in the keyboard, and jump pages with left and right.