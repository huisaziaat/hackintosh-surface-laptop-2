# Hackintosh Configuration for Surface Laptop 2 (Mojave 10.14.4)

### Notice
Feel free to fork this repo or create pull requests for newer macOS versions. It took me a lot of time and effort to figure out how to get this to work on the surface laptop 2. I hope this guide will be a good starting point for other talented developers to be able to boot newer versions of macOS on their surface devices.

### Screenshot
![Mojave 10.14.4](images/1.png?raw=true "Surface Laptop 2 Running Mojave 10.14.4")

### Disclaimer
This is not a full installation guide of how to install macOS on your surface device, there are many tutorials online to help you out with that, the only thing you have to do is use macOS 10.14.4 and the EFI folder in this project.

### What is working?
- QE/QC Intel UHD 620 (Full Graphics Acceleration)
- Sleep / Wake
- Internal Display
- Displayport
- Displayport audio
- Audiojack
- Microphone
- Touchpad/Trackpad
- USB Ports
- Everything else NOT listed in not working

### Not working
- Wifi / Bluetooth (Use a dongle for that)
- Keyboard, this is due Microsoft using a non standard config for driver (Surface Aggretator Module) which hasn't been ported over to macOS, it has been ported over for linux.
- Touch-screen

### Specs
- Intel Core i5-8250u
- Intel UHD Graphics 620
- 8GB LPDDR3 RAM
- 13.5", 2256 × 1504 (201 PPI) LCD Touch-screen
- 128GB nvme SSD

### Notes
- There are 3 configs files in Clover, 1 is for installing and first boot, then rebuild caches and boot the regular config for full graphics acceleration. The final one is for just the internal display.

## Credits
- [Rehabman] (https://www.tonymacx86.com/members/rehabman.429483/)
- [Molie34] (https://github.com/molie34/Surface-Pro-6-macOS) *(For the base config, Surface Pro 6 is a similar device so it was a good starting point.)