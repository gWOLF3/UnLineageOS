# Grokking AOSP (Android Open Source Project)

Grokking my custom Lineage build from start to finish.

```
Vendor: google
Device: Pixel XL
codename: Marlin
base ROM: Lineage 17.1
SDK version: 29 (Android 10)

```

## Understanding the Hardware

### The SoC 

- Qualcomm Snapdragon [821 (MSM8996)](https://www.notebookcheck.net/Qualcomm-Snapdragon-821-MSM8996-Pro-SoC.180683.0.html#:~:text=The%20Qualcomm%20Snapdragon%20821%20MSM8996,clocked)

### A/B Partition Schema

- overview and introduction: https://www.xda-developers.com/how-a-b-partitions-and-seamless-updates-affect-custom-development-on-xda/

- logistics of a/b slots: https://www.droidwin.com/flash-roms-magisk-twrp-kernels-a-b-partition-devices/

### Boot ROM

- [Comparing Qualcomm's XBL UEFI bootloaders on Snapdragon 820, 835, and 845](https://worthdoingbadly.com/qcomxbl/)

## Understanding The Boot Process

### Overview

- [Understanding the boot process from startup](https://sites.google.com/site/androidersclub/in-the-news/theandroidbootprocessfrompower-on)

### Fastboot OEM

- [A vuln perpective](https://www.usenix.org/system/files/conference/woot17/woot17-paper-hay.pdf) - used at comma
- [Comma flash process reference](https://github.com/commaai/eon-neos-builder/blob/master/devices/eon/flash.sh)

### The Bootloader

- [Little Kernal (LK)](https://developer.qualcomm.com/download/db410c/little-kernel-boot-loader-overview.pdf)

### Init Process

- [init.rc](https://github.com/openinternet-cc/android_system_core/blob/lineage-17.1/rootdir/init.rc)

### The Android Runtime (ART) / Dalvik

- [AOSP Documentation](https://source.android.com/devices/tech/dalvik)

### System Server 

- [SystemServer.java]()

- Activity Manager


## Gettings Started: Developing on AOSP

### Build Tooling

- [repo command](https://source.android.com/setup/develop/repo): like a "meta" git command 

> Advice for building efficiently: [Udi Cohen blog](http://blog.udinic.com/2014/07/24/aosp-part-3-developing-efficiently/)


#### Hybrid Build System (Make (legacy) -> Soong (new))

- [Make Build System](https://android.googlesource.com/platform/build/+/master/README.md)

- [Soong Build System](https://source.android.com/setup/build)

> Why are AOSP platform apps not building in Android Studio? 
[Link](https://android.jlelse.eu/building-aosp-platform-apps-on-android-studio-fae87d6c370a) (*Hint*: AOSP Doesn't use Gradle*)





