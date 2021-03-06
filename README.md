[![Build Status](https://travis-ci.org/intel-aero/packages.svg?branch=master)](https://travis-ci.org/intel-aero/packages)

# Packages

## Building

### All packages

`make`

### Only the Linux kernel 4.4 with patches

`make kernel`

### All aero-* packages except the kernel

`make aero-packages`

### Individual packages

You can build individual packages by executing:

```
./scripts/build-pkg.sh PACKAGE-NAME
```

Where PACKAGE-NAME matches the name of the directory where the package metadata is.

### Collect

`make collect` makes all deb files available in a `packages/` directory.

### Cleanup

`make clean` cleans up the build/ directory

`make cleanall` removes all build and source files

## Utils

`./scripts/update-pkg-changelog.sh` is a helper to update the debian/changelog file
using Debian helper tools (thus, it requires such tools available in your system).

## Updating meta-intel-aero and mavlink-router revisions

New revisions sha1 must be added to the configuration file scripts/conf.

## Camera Streaming Daemon
Install librealsense alongwith Camera streaming daemon package(aero-camera-streaming-daemon) from:
			https://github.com/IntelRealSense/librealsense
For RS200, install the legacy branch of librealsense(librealsense v1)
