# Aospify - Pure AOSP #

<p align="center">
<img src="https://i.postimg.cc/3rV8CRPP/Aospify.jpg" >

### Sync ###

```bash

# Initialize local repository
repo init -u https://github.com/Aospify/platform_manifest -b R

# Sync
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

### Build ###

```bash

# Set up environment
$ . build/envsetup.sh

# Choose a target
$ lunch aosp_$device-userdebug

# Build the code
$ mka bacon