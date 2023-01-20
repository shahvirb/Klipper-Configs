# Klipper-Configs
My Artillery Genius Pro with Klipper + Moonraker + Mainsail

## Installation + Configuration
- Raspberry Pi OS Lite (32 bit)
- Set hostname to ```octopi.local```
- [Install KIAUH](https://www.lpomykal.cz/kiauh-installation-guide/)
  - In KIAUH install Klipper + Moonraker + Mainsail
- Clone this git repo into ```/home/pi/printer_data/config/```
- Double check IP address and output_id of TPLink Smart Plug in ```moonraker.conf```. ```output_id: 0``` is plug 1.

## Octodash Setup (Obsolete)
TODO remove this and replace it with KlipperScreen
```cp ~/klipper_config/octodash_config.json ~/.config/octodash/config.json```

## Display Configuration
Edit ```/boot/config.txt``` and add
```
#Settings for my 1024x600 7" display
disable_overscan=1
hdmi_cvt=1024 600 60 3 0 0 0
hdmi_force_hotplug=1
hdmi_group=2
hdmi_mode=87
```