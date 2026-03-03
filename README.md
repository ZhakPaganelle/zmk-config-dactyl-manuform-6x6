# dactyl-manuform-6x6-zmk

This is my config for the Dactyl Manuform 6x6.
It supports ZMK Studio

**!This keymap is a cursed abomination!**

I made it for myself and strictly discourage you from using it

Use one from main branch instead


## Layout
### DEFAULT 0
![Default](https://github.com/user-attachments/assets/8229f10b-ac3b-4cc6-87ba-4d0ac0dbdbab)

### LWR
![Lower](https://github.com/user-attachments/assets/5c6be9dc-65a3-4cd9-8006-944f87c30044)

### RSE
![Rised](https://github.com/user-attachments/assets/8a0e34b1-3b9d-4ceb-b72f-30022a086735)

### ADJ
![Settings](https://github.com/user-attachments/assets/d4f48563-1783-4e73-bcd0-6d65674c5e9a)


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
