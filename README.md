# Pinephone Devel
## Arch Linux ARM barebone image on the eMMC 
for the purpose of a PDA

- How to kill a tty?\
check with `ps -H -t /dev/tty1` and kill with `kill -SIGKILL *PID*`

### statusbar with dvtm
- [x] installed rxvt-unicode
- [ ] config dvtm 

### Lynx text-based web browser
Google Search does not work :t-rex:

### charging
The keyboard battery can be toggled on [short] / off [double, long(15s)],\
and is basically a power bank, which charges the phone and drains it whent its turned off. :sweat_smile:

In a desktop environment (phosh, gnome), I was able to monitor the battery levels of both phone and keyboard, so there is no need to shim the POGO pins.

### keyboard fix
Characters on function keys /top row are not working out of the box. [Tried this](https://codeberg.org/HazardChem/PinePhone_Keyboard/src/branch/main/tty), `udevadm control --reload` did not work at first, made *ppkb_detector.sh* file executable with chmod.\
Expected behaviour with AltG + function key,\
switching between (6)consoles with Ctrl + Fn + number

