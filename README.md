**How to back up and recover** https://github.com/EricZimmerman/Voron-Documentation/blob/main/community/howto/EricZimmerman/BackupConfigToGithub.md
___________________________________________________________________________________________________________________________________________________
**OS Upgrade** https://github.com/EricZimmerman/VoronTools/blob/main/OSUpgrade.md
_________________________________________________________________________________
**Kiauh** https://github.com/dw-0/kiauh
_______________________________________
**Update CanBus:**

https://canbus.esoterical.online/toolhead_klipper_updating.html

https://canbus.esoterical.online/toolhead_flashing/common_hardware/BigTreeTech%20SB2209%20(RP2040)/README.html
___________________________________________________________________________________________________________________
**Update CanBus COMPLETE** https://canbus.esoterical.online/
_______________________________________________________________
**Load G-Code to Printer via USB** https://github.com/shiftingtech/Moonraker-loader/tree/main
______________________________________________________________________________________________
**Rpi Micro Controller Setup:**

https://www.klipper3d.org/RPi_microcontroller.html

https://docs.ldomotors.com/en/voron/Picobilical
______________________________________________________
**Update/Flash BTT Octopus MCU:** https://docs.vorondesign.com/build/software/octopus_klipper.html

Turn on printer

Run: make menuconfig to create klipper.bin

Turn off printer

Install jumper to BOOT0

Connect BTT Octopus to Computer via USB

Turn on printer

Click Reset button on BTT Octopus

Run: lsusb to confirm STM Device in DFU mode

Run: flash FLASH_DEVICE=0483:df11

Turn off printer

Remove jumper from BOOT0

Turn on printer

Run: ls /dev/serial/by-id to confirm usb-Klipper_stm32f446xx_440016001050535556323420-if00
