# LineageOS for Anica KTOUCH i9 (i9)

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/b/b2/Lineage_OS_logo.svg/2560px-Lineage_OS_logo.svg.png">

This is a W.I.P project to bring stable LineageOS roms to this mediatek phone<br/>
For now just use this builds for testing or fun, hardware/software bugs are present

## Build Rules (Q) (Stable)
```
#Init LineageOS
mkdir -p ~/android/lineage&&cd ~/android/lineage
repo init -u https://github.com/LineageOS/android.git -b lineage-17.1
repo sync
source build/envsetup.sh

#Repos
git clone -b device_tree_stable https://github.com/daviiid99/LineageOS_KTOUCH-i9.git device/ktouch/i9
git clone -b vendor_mediatek_Q https://github.com/daviiid99/LineageOS_KTOUCH-i9.git  vendor/mediatek
git clone  -b vendor_tree_VNDK27 https://github.com/daviiid99/LineageOS_KTOUCH-i9.git vendor/ktouch/i9
```

## Build Rules (Q) (Testing)
```
#Init LineageOS
mkdir -p ~/android/lineage&&cd ~/android/lineage
repo init -u https://github.com/LineageOS/android.git -b lineage-17.1
repo sync
source build/envsetup.sh

#Repos
git clone -b device_tree_Q https://github.com/daviiid99/LineageOS_KTOUCH-i9.git device/ktouch/i9
git clone -b vendor_mediatek_Q https://github.com/daviiid99/LineageOS_KTOUCH-i9.git  vendor/mediatek
git clone  -b vendor_tree_VNDK28 https://github.com/daviiid99/LineageOS_KTOUCH-i9.git vendor/ktouch/i9
git clone  -b vendor_tree_SAR__VNDK28 https://github.com/daviiid99/LineageOS_KTOUCH-i9.git vendor/ktouch/sar
```

#Patches
patch -d external/skia -p1 < device/ktouch/i9/patches/external/skia/0001-GrGLCaps-allow-ignoring-vendor-supplied-texture-swiz.patch
patch -d frameworks/base -p1 < device/ktouch/i9/patches/frameworks/base/0001-hwui-add-dependency-on-libbase.patch
patch -d frameworks/base -p1 < device/ktouch/i9/patches/frameworks/base/0002-Fix-crash-on-some-devices-by-checking-for-null-clien.patch
patch -d frameworks/opt/net/wifi -p1 < device/ktouch/i9/patches/frameworks/opt/net/wifi/0001-Restore-O-O-MR1-behaviour-of-initing-ifaces-before-s.patch
patch -d system/core -p1 < device/ktouch/i9/patches/system/core/0001-rootdir-add-support-for-custom-ld-template.patch

#Build
brunch i9
```

## Updates History

|   Date                 | Download                  | Changelog |
| :----------------------| :-------------------------------- | :--------------------------|
|20210808                |    <a href="https://github.com/daviiid99/LineageOS_KTOUCH-i9/releases/tag/20210808">Lineage-17.1-20210808-UNOFFICIAL-i9.zip</a> | Fixed Wi-Fi
|20210807                |    <a href="https://github.com/daviiid99/LineageOS_KTOUCH-i9/releases/tag/20210807">Lineage-17.1-20210807-UNOFFICIAL-i9.zip</a>  | Initial release

# Sources
<b><a href="https://github.com/daviiid99/android_device_ktouch_i9">Device tree</a><br/></b>
<b><a href="https://github.com/daviiid99/kernel_ktouch_i9">Kernel Source</a></b><br/>
<b><a href="https://github.com/daviiid99/android_vendor_ktouch_i9">Vendor Tree</a></b>
