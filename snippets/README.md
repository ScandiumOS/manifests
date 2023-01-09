# ScandiumOS | Open Source Software
android based on AOSP.

### Requirements
- Around 500GB disk space.
- Around 18GB RAM running Linux.

### Sync our source ###
```bash
repo init -u https://github.com/scandiumOS/android -b 12.1
```
```bash
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

### Build our source ###
```bash
. build/envsetup.sh
lunch lineage_$devicecodename-userdebug
mka bacon -j$(nproc --all)
```

### Credits ###
 * [**AOSP**](https://android.googlesource.com)
 * [**PixelExperience**](https://github.com/PixelExperience)
 * [**LineageOS**](https://github.com/LineageOS)
 * [**POSP**](https://github.com/PotatoProject)
 * [**DerpFest**](https://github.com/DerpLab)
 * [**Superior OS**](https://github.com/SuperiorOS)
 * [**ExtendedUI**](https://github.com/Extended-UI)
