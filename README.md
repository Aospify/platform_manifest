# Aospify #

# Pure AOSP #

### Sync ###

```bash

# Initialize local repository
repo init -u https://github.com/Aospify/platform_manifest -b Q

# Sync
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

### Build ###

```bash

# Set up environment
$ . build/envsetup.sh

# Choose a target
$ lunch aospify_$device-userdebug

# Build the code
$ mka bacon