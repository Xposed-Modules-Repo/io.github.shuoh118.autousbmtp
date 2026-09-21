# Auto USB MTP

An Xposed/LSPosed module: once the cable is plugged in, it automatically switches the USB connection mode to MTP, so you no longer have to pull down the notification shade and tap through it by hand every time.
-----
[中文](README.md)

## Features

- Automatically switches the USB mode to MTP once the data cable is plugged in
- Hooks UsbDeviceManager and AdbService, taking effect at the system_server layer

## Requirements

- Android 12 or later (module minApiVersion / targetApiVersion = 102)
- LSPosed (Zygisk or Riru)
- Root access (KernelSU or Magisk)

## Installation

1. Download the latest APK from Releases
2. Open the LSPosed manager after installing
3. Enable Auto USB MTP in the module list
4. Tick the System Framework (system) scope
5. Reboot the device

## Configuration
Changes are written immediately and take effect the next time the cable is plugged in.

## Changelog

### v2.0
- Fixed the issue where the cable was not detected when it was plugged and unplugged repeatedly within a short time
- Reduced the APK size

### v1.2
- Optimized the hook installation process
- Fixed the issue where the mode did not take effect after plugging in on some devices

## License

This project uses the Mulan Public License, Version 2 (Mulan PubL v2). See [LICENSE](https://license.coscl.org.cn/MulanPubL-2.0) for the full text.

## Releases and Feedback

- Release page: https://github.com/Xposed-Modules-Repo/io.github.shuoh118.autousbmtp/releases
- Other release page: https://github.com/Shuoh118/Auto-USB/releases
- Issue feedback: https://github.com/Shuoh118/Auto-USB/issues

## Finally

- If you find this project useful, please hit the star in the top right corner. It is the greatest encouragement for me.
- Finally, thanks to @TigerSpirit217
- This project was modified from https://github.com/TigerSpirit217/USBManager. Without him, this project would not exist.
