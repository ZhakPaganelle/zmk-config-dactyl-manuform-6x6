# dactyl-manuform-6x6-zmk

This is my config for the Dactyl Manuform 6x6.
It supports ZMK Studio


## Layout
### DEFAULT 0
![Default](https://github.com/user-attachments/assets/afed2455-4d0b-41cf-b629-ecaf54a45d91)

### LWR
![Lower](https://github.com/user-attachments/assets/59a8c71a-afe6-4b93-a27c-69d8faffc154)

### RSE
![Rised](https://github.com/user-attachments/assets/0d97a3a2-f85e-4113-a456-0651e0e3a256)

### ADJ
![Settings](https://github.com/user-attachments/assets/a52f05ea-3d46-45e1-a70c-62d7c0bf734d)


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
