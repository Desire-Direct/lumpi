# Pinephone Devel
## Keyboard fix
Characters on function keys /top row are not working out of the box. [Tried this](https://codeberg.org/HazardChem/PinePhone_Keyboard/src/branch/main/tty), `udevadm control --reload` did not work at first, as the *ppkb_detector.sh* file needs to be made executable with chown.

Switching between consoles(6) with Fn + Alt + number, however tty2 can only be accessed with Ctrl + Fn + F2.
