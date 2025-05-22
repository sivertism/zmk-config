# Outputs
The keyboard firmware is built using GitHub actions. Find the resulting `.uf2` binaries in the Actions tab.

# Keymap editor

[Keymap editor](https://nickcoutsos.github.io/keymap-editor/)

# Flashing
Flash the boards by plugging in usb-c and double-resetting within 500 ms. They'll show up as a USB mass storage device. Simply copy in the generated UF2 files

# Pairing
If pairing between the halves fails, use the `settings_reset` uf2.

1. connect both halves
2. put both halves in bootloader mode (double reset)
3. copy in `settings_reset.uf2` into each half.
4. put both halves in bootloader mode.
5. copy each half's firmware.
6. reset both halves simultaneously
