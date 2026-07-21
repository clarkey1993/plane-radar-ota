# Plane Radar OTA

Public update assets for both Plane Radar device families.

## ESP32

ESP firmware continues to use the existing raw-file layout without changes:

- versioned binary: `releases/firmware-vX.Y.Z/firmware.bin`
- current manifest: `releases/latest/manifest.json`
- platform value: `esp32`

## Raspberry Pi

Pi updates are published as GitHub Releases and do not modify the ESP folders
or manifest:

- tag: `pi-vX.Y.Z`
- assets: `plane-radar-pi.tar.gz` and `pi-manifest.json`
- platform value: `raspberry-pi`
- source: [`clarkey1993/plane-radar-2.0-pi`](https://github.com/clarkey1993/plane-radar-2.0-pi)

Run the **Build and publish Raspberry Pi release** workflow to test the source,
build a SHA-256-verified archive, and publish the next Pi release. Release tags
are immutable: increase the version in the Pi source before each run.
