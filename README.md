# Paranoid Android #

### Creating workspace folder ###

```bash
mkdir AOSPA
cd AOSPA
```

### Initializing repo ###

```bash
repo init -u https://github.com/aospa-lagvender/manifest -b topaz
```

### Initializing depth repo ###

```bash
repo init --depth=1 -u https://github.com/aospa-lagvender/manifest -b topaz
```

### Downloading the source tree ###

```bash
repo sync -c --force-sync --optimized-fetch --no-tags --prune -j$(nproc --all)
```

## Building ##

```bash
./rom-build.sh lavender -j$(nproc --all)
```
