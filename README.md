# dactyl-manuform-6x6-zmk

This is my config for the Dactyl Manuform 6x6.

## Layout
### DEFAULT 0
![Screenshot 2023-07-09 at 1 20 54 AM](https://github.com/nidzola/dactyl-manuform-5x6-zmk/assets/3450224/97fbda14-c02e-49ac-bf4e-c979eccc10ae)

### LWR
![Screenshot 2023-07-09 at 1 21 34 AM](https://github.com/nidzola/dactyl-manuform-5x6-zmk/assets/3450224/5adf8530-5e0b-4c2d-b56b-56d2dbff1a4b)

### RSE
![Screenshot 2023-07-09 at 1 21 54 AM](https://github.com/nidzola/dactyl-manuform-5x6-zmk/assets/3450224/deaca9ed-2b0d-44b6-a363-5034b9309f7b)

### ADJ
TBD screenshot


## Good to know

### Codes for the keys
https://zmk.dev/docs/codes

### Issues with flashing
Use terminal to flash the nice!nano.
OSX example:
```bash
cp your-file-path/to-file.uf2 /Volumes/NICE\!NANO
```

### Reset Split Keyboard Procedure
Perform the following steps to reset both halves of your split keyboard:

Put each half of the split keyboard into bootloader mode.
Flash one of the halves of the split with the downloaded settings reset UF2 image. Immediately after flashing the chosen half, put it into bootloader mode to avoid accidental bonding between the halves.
Repeat step 2 with the other half of the split keyboard.
Flash the actual image for each half of the split keyboard (e.g my_board_left.uf2 to the left half, my_board_right.uf2 to the right half).
After completing these steps, pair the halves of the split keyboard together by resetting them at the same time. Most commonly, this is done by grounding the reset pins for each of your keyboard's microcontrollers or pressing the reset buttons at the same time.

### Split Keyboard Halves Unable to Pair
Split keyboard halves pairing issue can be resolved by flashing a settings reset firmware to both controllers. For resetting the firmware, use the settings_reset.uf2 file from the ZMK build artifact. After flashing the settings reset firmware, flash the actual firmware to both controllers.

### General ZMK Troubleshooting
https://zmk.dev/docs/troubleshooting
