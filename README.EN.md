# Auto USB MTP

Xposed/LSPosed Module: Automatically switches USB connection mode to MTP upon connecting a data cable, eliminating the need to manually pull down the notification bar and select each time.  
-----  
[中文](README.md)

## Features

- Automatically switches USB mode to MTP when a data cable is connected  
- Hooks `UsbDeviceManager` and `AdbService`—effective at the `system_server` layer  

## Requirements

- Android 12 or higher (module’s `minApiVersion` / `targetApiVersion` = 102)  
- LSPosed (works with either Zygisk or Riru)  
- Root access (compatible with KernelSU or Magisk)  

## Installation

1. Download the latest APK from [Releases](../../releases)  
2. Install the APK  
3. Open the LSPosed manager and enable the *Auto USB MTP* module in the module list  
4. Select *System Framework (system)* as the activation scope  
5. Reboot the device  

## Configuration  
Changes take effect immediately and apply to subsequent cable connections.  

## Changelog

### v3.0 Fix  
- Resolved several known issues  
- Optimized APK size  

### v2.0  
- Fixed inability to detect repeated plugging/unplugging within short intervals  
- Further optimized APK size  

### v1.2  
- Optimized the hook installation process  
- Fixed an issue where the mode failed to activate on certain devices after connecting the cable  

## License

This project is licensed under the Mulan Public License, Version 2 (Mulan PubL v2). Full license text: [LICENSE](https://license.coscl.org.cn/MulanPubL-2.0).

## Releases & Feedback

- Release page:<https://github.com/Shuoh118/Auto-USB/releases>
- Issue reporting:<https://github.com/Shuoh118/Auto-USB/issues>

## Credits

- If you find this project useful, please give it a ⭐ star in the top-right corner—your support means a lot!  
- Special thanks to @TigerSpirit217  
- This project is based on [https://github.com/TigerSpirit217/USBManager](https://github.com/TigerSpirit217/USBManager); without them, this project would not exist.