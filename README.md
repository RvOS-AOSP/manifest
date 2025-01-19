# RvOS

## Getting Started

To get started with the RvOS sources, you'll need to get
familiar with [Git and Repo](https://source.android.com/setup/build/downloading).

To initialize your local repository, use command:

```bash
repo init -u https://github.com/RvOS-AOSP/manifest.git -b fifteen --git-lfs
```

Then sync up:

```bash
repo sync
```

## RvOS Flags
```Makefile
RVOS_MAINTAINER := Rve
TARGET_FACE_UNLOCK_SUPPORTED := true/false
```

## Building the System

Initialize the ROM environment with the envsetup.sh script.

```bash
. build/envsetup.sh
```

Lunch your device after cloning all device sources if needed.

```bash
lunch rvos_devicecodename-ap4a-buildtype
```

Start compilation

```bash
mka bacon
```
