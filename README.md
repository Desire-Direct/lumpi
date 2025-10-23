# Pinephone Devel
## Arch Linux ARM barebone image on the eMMC

### keyboard fix
Characters on function keys /top row are not working out of the box. [Tried this](https://codeberg.org/HazardChem/PinePhone_Keyboard/src/branch/main/tty), `udevadm control --reload` did not work at first, as the *ppkb_detector.sh* file needs to be made executable with chown.\
Expected behaviour with AltG + function key,\
switching between (6)consoles with Ctrl + Fn + number
