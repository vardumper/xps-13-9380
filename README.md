# xps-13-9380

Stable EFI Folder for installing macOS Ventura and Sonoma on Dell XPS 13 9380 (i7-8656U).
Tested successfully with Ventura 13.+ and up as well as Sonoma up to 14.5
I use OCAuxiliary Tools to keep OpenCOre (currently 1.0) and kexts updated.

![preview](https://github.com/vardumper/xps-13-9380/blob/main/preview-sonoma.png?raw=true)

## Get started
1. Create a bootable install media `sudo /Applications/Install\ macOS\ Sonoma.app/Contents/Resources/createinstallmedia --volume /Volumes/SOME_USB_DRIVE`
2. Download [MountEFI](https://github.com/corpnewt/MountEFI). Run the command to mount the EFI partition of the USB.
3. Copy and paste the EFI folder from this repository to the EFI partition of your USB.
4. Download [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS). Run the command and execute all steps to generate new Serial, ROM, MLB, UID.
5. Reboot to USB, install macOS.
6. After install copy the USBs EFI folder to the EFI partition of your SSD.

## Not working

- Fingerprint reader (not really needed)
- Audio Jack
- The XPS' Wifi chipset isn't supported by macOS

## Working

- Display Port
- SD Card Reader
- Bluetooth (tested successfully with Logitech MX3 Master, Airpods Pro not working)
- Audio
- Mic
- Wifi via Dongle (tested with Archer T3U and T2U nano)
- Camera
- Thunderbolt (I don't have any TB devices to test this with.)
- Function keys

## Post-Install Steps

- Remap some keys to your needs using Karabiner (I switched left option and command keys to resemble a mac keyboard)
