# Pixel Experience 9810 Fork #

### Sync ###

```bash

# Initialize local repository
repo init --depth=1 -u https://github.com/9810-S/manifest -b twelve-blob

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
$ mka bacon -jX
```
