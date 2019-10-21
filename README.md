UVCCamera
=========

Fork of [UVCCamera by saki](https://github.com/saki4510t/UVCCamera) that:

1. Fixes compilation errors when using the latest Android SDK (28) and NDK (20).
2. Turns usbCameraTest4 into a simple app that can be used by non tech savvy people to watch, photograph and record a live stream from a USB camera (my goal).

This is just a quick hack to enable the usage of an endoscope camera on Android with only free software. All free software apps I could find lacked one of the above mentioned features (watch, photograph, record) or were malfunctioning.

For a working apk check the [releases on GitHub](https://github.com/dllud/UVCCamera/releases).

Tested on a Samsung Galaxy S3 (GT-i9300) running LineageOs 14.1 (Android 7.1.2).

For an alternative take a look at [AndroidUSBCamera by Jiangdongguo](https://github.com/jiangdongguo/AndroidUSBCamera).

    Copyright (c) 2019 dllud
    Copyright (c) 2014-2017 saki t_saki@serenegiant.com

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

      http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

All files in this project are under this Apache License, Version 2.0.

Files in the `jni/libjpeg`, `jni/libusb` and `jin/libuvc` directories may have a different license, see the respective files.

Building
========

Install both Android SDK and NDK on your system and set up the proper paths on `local.properties`.

To build the entire project run: `./gradlew build`

To build just a specific test app run: `./gradlew :usbCameraTest4:build`

