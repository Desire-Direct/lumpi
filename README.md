# Pinephone Devel
## Arch Linux ARM barebone image on the eMMC

### statusbar with dvtm
- [x] installed rxvt-unicode
- [ ] config dvtm 

### keyboard fix
Characters on function keys /top row are not working out of the box. [Tried this](https://codeberg.org/HazardChem/PinePhone_Keyboard/src/branch/main/tty), `udevadm control --reload` did not work at first, made *ppkb_detector.sh* file executable with chmod.\
Expected behaviour with AltG + function key,\
switching between (6)consoles with Ctrl + Fn + number
