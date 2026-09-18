# Auto USB MTP

An Xposed/LSPosed module: automatically switches the USB connection mode to MTP when a cable is plugged in, so you no longer have to pull down the notification shade and tap it manually every time.
-----
[中文](README.md)

## Features

- Automatically switches the USB mode to MTP when a data cable is connected
- Hooks `UsbDeviceManager` and `AdbService`, taking effect at the system_server layer
- Mode switching happens instantly, no device reboot required

## Requirements

- Android 12 or above (module minApiVersion / targetApiVersion = 102)
- LSPosed (either Zygisk or Riru)
- Root access (KernelSU / Magisk)

## Installation

1. Download the latest APK from [Releases](../../releases)
2. After installing, open the LSPosed Manager
3. Enable **Auto USB MTP** in the module list
4. Set the scope to **System Framework** (system)
5. Reboot the device

## Configuration

Changes are written immediately and take effect the next time you plug in the cable.

## Changelog

### v1.2
- Improved the hook installation flow
- Fixed USB mode not taking effect after plugging in on some devices

## Notes

This module is based on the open-source project USBManager, with the package name and app name adjusted to comply with the submission requirements of the official LSPosed repository. The functional logic is consistent with upstream.

## License

This project is licensed under the Mulan Public License, Version 2 (Mulan PubL v2). See [LICENSE](https://license.coscl.org.cn/MulanPubL-2.0) for the full license text.

## Releases and Feedback

* Releases: <https://github.com/Shuoh118/Auto-USB/releases/tag/main>
* Issues: <https://github.com/Shuoh118/Auto-USB/issues>

## Finally

If you find this project useful, please give it a star in the top-right corner — that is the best encouragement for me.
Lastly, thanks to @https://github.com/TigerSpirit217
This project is modified from <https://github.com/TigerSpirit217/USBManager?tab=readme-ov-file> — without him, this project would not exist.
