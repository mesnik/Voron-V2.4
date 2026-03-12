**How to back up and recover**
https://github.com/EricZimmerman/Voron-Documentation/blob/main/community/howto/EricZimmerman/BackupConfigToGithub.md


**OS Upgrade**
https://github.com/EricZimmerman/VoronTools/blob/main/OSUpgrade.md

**Kiauh**
https://github.com/dw-0/kiauh

**Update CanBus**

https://github.com/EricZimmerman/VoronTools/blob/main/EBB_CAN.md#pi

https://canbus.esoterical.online/toolhead_klipper_updating.html

https://canbus.esoterical.online/toolhead_klipper_updating.html

https://canbus.esoterical.online/toolhead_flashing/common_hardware/BigTreeTech%20SB2209%20(RP2040)/README.html


**Update CanBus COMPLETE**
https://canbus.esoterical.online/

**Load G-Code to Printer via USB**
https://github.com/shiftingtech/Moonraker-loader/tree/main

**Rpi Micro Controller Setup:**

https://www.klipper3d.org/RPi_microcontroller.html

https://docs.ldomotors.com/en/voron/Picobilical 


**Update/Flash MCU**

cd ~/klipper/scripts
python3 -c 'import flash_usb as u; u.enter_bootloader(/dev/serial/by-id/usb-Klipper_stm32f446xx_35001B000450534E4E313020-if00)'
cd ..
make flash FLASH_DEVICE=0483:df11

1) Turn printer off
2) Add jumper to BOOT0
3) Turn printer on
4) Run script above
5) Turn printer off
6) Remove jumper
7) Turn printer on
