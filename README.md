# pocophone-guide
A journey with the pocophone f1

## Step 1: Unlock the bootloader

### Why
In order to flash through fastboot (fastboot roms or recovery roms) you need to unlock the bootloader.
In order to debloat the phone you need to unlock the bootloader.
In order to install custom recovery, you need to unlock the bootloader.

### Affects
Xiaomi will honor the warranty even with an unlocked bootloader. 

### Disadvantages
This lowers the bar of security on the phone and it will be possible for a third-party to install malware for e.g. onto the phone. Probably physical access will be required to compromise the phone but nevertheless its possible.

-
#### Notes 
It is possible to re-lock the bootloader.

### Pre-requisites for current method
- A valid nano-sim in the pocophone
- An accessible Mi account
- The MiUnlock tool
- Time: 72 hours
- A PC with Fastboot drivers installed
- Android platform-sdk-

## Method

*Prepare the phone*

- Put the sim in, and turn it on.
- Activate Developer Options.
- In developer options, activate USB Debugging Mode.
- In developer options, go to Mi Unlock device. Then register your phone. This is the step that requires a SIM present in the phone.

*Prepare the PC*

Download the Mi Unlock tool. 

Install fastboot drivers for the phone. On Windows Go to 'Device Manager', select the 'Android' device that has a 'Caution' icon next to it if it isnt properly installed. Select option to update drivers yourself by location, and point to the drivers in the Mi Unlock tool driver folder. The device should get recognized as Android Bootloader Interface. To verify, running 'fastboot devices' should return the name of the devices connected.

*Run the unlock tool*

Run the Mi Unlock tool and follow the instructions on it.

You can put the device into fastboot mode by turning it off, then holding VolDown+Power for a couple of seconds. In fastboot mode, the device screen shorts an Android mascot, and the words 'fastboot'
