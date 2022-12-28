# rofi-radio 📻
An extendable rofi based menu for streaming audio (optionally but preferably) on linux 🐧.

This script is inspired by [Rofi-Beats](https://github.com/Carbon-Bl4ck/Rofi-Beats).

## Dependencies
* notify-send
* rofi

For Debian:
```
$ sudo apt install rofi notify-osd mpv
```

For Arch Linux:
```
$ sudo pacman -S rofi notify-osd mpv
```

Clone this repository:

```
$ git clone https://github.com/aerosol-can/rofi-radio
$ cd rofi-radio
```
```
$ chmod +x rofi-radio
```

Now test out the script:
```
$ ./rofi-radio
```

## Usage

The script toggles the radio on and off depending on it's current state.

The script first checks to see if an instance of the radio is already playing.

If it finds the script is already playing music it kills the music. If the radio is not already playing it will launch the list of stations you can choose from.

### `mpv` arguments

- You can add options in the `ARGS` variable in the script to specify those options for running mpv. The default of `--no-video` is already added.
- You can also add accitional arguments on a per stream basis using the `ADDITIONAL_ARGS` variable.

## Extra Tips 📝

- I'd highly recommend linking this script to a keybinding, using a tool such as [skhd](https://github.com/koekeishiya/skhd) or [sxhkd](https://github.com/baskerville/sxhkd).
