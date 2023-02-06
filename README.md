# Hackintosh-DellXPS9360
--LAPTOP SPECS--
- Dell 13 XPS 9360
- CPU: Intel Core i7-8550u 2.71 GHz
- GPU: Intel UHD Graphics 620 2048MB
- RAM: 8GB 1867 MHz LPDDR3
- WIFI CARD: Intel Wireless-AC 8265 (Killer Wireless-AC 1535 not supported)
- OS: macOS Big Sur 11.7.3

--USB Bootloader Preparation--
  1) Load Big Sur onto USB
    - If on windows, download TransMac to format drive for Mac and add OS image to it
  2) Create an EFI partition on the USB Drive and copy the EFI file into it
  3) Install Appropriate Kexts
      - *wifi kext is specifically for me, make sure you have correct kext for YOUR wifi card*
      - WIFI: https://github.com/OpenIntelWireless/itlwm
      - BLUETOOTH: https://github.com/OpenIntelWireless/IntelBluetoothFirmware

4) Using ProperTree, add downloaded Kexts into KERNAL
    - Change BundlePath to kextfilename.kext
    - Change ExecutablePath, can be found within the Kext file (may need a mac machine for this)
    - Make sure PlistPath points to Contents/info.plist
  5) Drive is now ready, eject


