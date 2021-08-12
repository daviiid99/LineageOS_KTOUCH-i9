# Apply patches

# external/skia
```
patch -d external/skia -p1 < device/ktouch/i9/patches/external/skia/0001-GrGLCaps-allow-ignoring-vendor-supplied-texture-swiz.patch
```

# frameworks/base
```
patch -d frameworks/base -p1 < device/ktouch/i9/patches/frameworks/base/0001-hwui-add-dependency-on-libbase.patch
patch -d frameworks/base -p1 < device/ktouch/i9/patches/frameworks/base/0001-Disable-vendor-mismatch-warning.patch.patch
patch -d frameworks/base -p1 < device/ktouch/i9/patches/frameworks/base/0001-UI-Revive-navbar-layout-tuning-via-sysui_nav_bar-tun.patch
patch -d frameworks/base -p1 < device/ktouch/i9/patches/frameworks/base/0002-Fix-crash-on-some-devices-by-checking-for-null-clien.patch
patch -d frameworks/base -p1 < device/ktouch/i9/patches/frameworks/base/0002-Relax-requirement-for-visible-flag-to-sdcards.patch
patch -d frameworks/base -p1 < device/ktouch/i9/patches/frameworks/base/0008-Try-to-make-brightness-more-generic-using-property-s.patch
```

# frameworks/av
```
patch -d frameworks/av -p1 < device/ktouch/i9/patches/frameworks/av/0004-We-might-not-have-a-mFlashlight-at-this-state-but-th.patch
patch -d frameworks/av -p1 < device/ktouch/i9/patches/frameworks/av/0005-CameraService-Support-calling-addStates-in-enumerate.patch
patch -d frameworks/av -p1 < device/ktouch/i9/patches/frameworks/av/0007-fixup-FIH-devices-Fix-Earpiece-audio-output.patch
patch -d frameworks/av -p1 < device/ktouch/i9/patches/frameworks/av/0013-audiopolicy-try-again-with-trimmed-audio-port-name-i.patch
patch -d frameworks/av -p1 < device/ktouch/i9/patches/frameworks/av/0014-Ignore-unknown-audio-codecs-in-media-profiles-AudioE.patch
patch -d frameworks/av -p1 < device/ktouch/i9/patches/frameworks/av/0016-Ignore-broken-camcorder-profiles.patch
patch -d frameworks/av -p1 < device/ktouch/i9/patches/frameworks/av/0020-Fix-android.media.cts.ImageReaderDecoderTest-fail-on.patch
```

# frameworks/opt/net/wifi
```
patch -d frameworks/opt/net/wifi -p1 < device/ktouch/i9/patches/frameworks/opt/net/wifi/0001-Restore-O-O-MR1-behaviour-of-initing-ifaces-before-s.patch
patch -d frameworks/opt/net/wifi -p1 < device/ktouch/i9/patches/frameworks/opt/net/wifi/0002-Support-hostap-on-O-O-MR1-vendors.patch
patch -d frameworks/opt/net/wifi -p1 < device/ktouch/i9/patches/frameworks/opt/net/wifi/0003-Restore-O-O-MR1-behaviour-of-initing-ifaces-before-s.patch
patch -d frameworks/opt/net/wifi -p1 < device/ktouch/i9/patches/frameworks/opt/net/wifi/0004-Boot-wifi-supplicant-both-with-lazy-hal-style-and-in.patch
```
# system/core
```
patch -d system/core -p1 < device/ktouch/i9/patches/system/core/0001-rootdir-add-support-for-custom-ld-template.patch
```

# system/sepolicy
```
patch -d system/sepolicy -p1 < device/ktouch/i9/patches/system/sepolicy/0002-Mark-mediacodec_2-6-7-8-as-hal_omx_server.patch
patch -d system/sepolicy -p1 < device/ktouch/i9/patches/system/sepolicy/0003-Revert-Don-t-set-esdfs-or-exfat-genfscon.-Assume-OEM.patch
```
