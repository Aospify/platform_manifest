![SlimAOSP](https://github.com/SlimAOSP/manifest_slimaosp/blob/ten/banner/SlimAOSP.png)

# SlimAOSP #

# The Stock Experience #

### Sync ###

```bash

# Initialize local repository
repo init -u https://github.com/SlimAOSP/manifest_slimaosp -b ten

# Sync
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

### Build ###

```bash

# Set up environment
$ . build/envsetup.sh

# Choose a target
$ lunch slimaosp_$device-userdebug

# Build the code
$ mka bacon -jX