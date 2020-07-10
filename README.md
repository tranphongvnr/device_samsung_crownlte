# TWRP device tree for Samsung Note9 aka crownlte

## Kernel source 
Available at https://github.com/corsicanu/android_kernel_samsung_universal9810

## How to build
This was tested and it's fully compatible with [minimal manifest twrp](https://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni).
1. Set up the build environment following instructions from [here](https://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni/blob/twrp-9.0/README.md#getting-started)
2. In the root folder of cloned repo you need to clone the device tree:
```bash
git clone -b android-9.0 https://github.com/tranphongvnr/device_samsung_crownlte device/samsung/crownlte
```
3. To build:
```bash
export ALLOW_MISSING_DEPENDENCIES=true && . build/envsetup.sh && lunch omni_crownlte-eng && mka recoveryimage -j128
```

