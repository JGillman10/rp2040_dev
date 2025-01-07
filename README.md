# rp2040_dev

## January 2025
First attempt was setting up through VSCode. Along with following the instructions in the Getting Started with Raspberry Pi Pico Document, a few changes needed to be made.

### Raspberry Pi Pico Recognized but could not flash
I needed to set up a UDEV rule. The pico probe repository has this: https://github.com/raspberrypi/picotool/tree/master/udev
Once downloaded, move it to the computer's UDEV rule directory.
```bash
sudo cp udev/99-picotool.rules /etc/udev/rules.d/
```

### Pico Probe Not Working
I also tried to use the Pico Probe to flash/debug. This did not work. Needed to go here: https://www.raspberrypi.com/documentation/microcontrollers/debug-probe.html#getting-started
```bash
sudo apt install openocd
sudo apt install gdb-multiarch
```
