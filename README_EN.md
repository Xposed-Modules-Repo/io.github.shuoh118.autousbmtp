# Auto USB MTP

Xposed/LSPosed module: Automatically switches the USB connection mode to MTP after plugging in the cable, eliminating the need to manually pull down the notification bar and select it each time.
-----
[中文](README.md)

## Function

- Automatically switches from USB mode to MTP after the data cable is plugged in.
- Hook `UsbDeviceManager`、`AdbService`It takes effect at the system_server layer.

## Environmental requirements

- Android 12 and above (module minApiVersion / targetApiVersion = 102)
- LSPosed (either Zygisk or Riru are acceptable)
- Root access (KernelSU/Magisk are both acceptable)

## Install

1. from [Releases](../../releases)  Download the latest APK
2. After installation, open the LSPosed manager.
3. Enable **Auto USB MTP** in the module list.
4. Select **system framework** as the scope.
5. Restart the device

## Configuration
Changes are written immediately, and the new settings will take effect the next time the cable is plugged in.

## Update Log

### v1.2
- Optimize Hook installation process
- Fixed the issue where the mode did not work after plugging in the cable on some models.


## license

This project uses the Mulan Public License, version 2. See the full license details below. [LICENSE](https://license.coscl.org.cn/MulanPubL-2.0)。

## Publish and Feedback
* Release page: <https://github.com/Xposed-Modules-Repo/io.github.shuoh118.autousbmtp/releases>
* Other release pages: <https://github.com/Shuoh118/Auto-USB/releases>
* Issue feedback: <https://github.com/Shuoh118/Auto-USB/issues>

## at last
* If you find this project helpful, please click the star icon in the upper right corner; it would be the best encouragement for me.
* Finally, thank you to @https://github.com/TigerSpirit217
* This project is based on https://github.com/TigerSpirit217/USBManager?tab=readme-ov-file
* This was modified; without him, this project wouldn't exist.
