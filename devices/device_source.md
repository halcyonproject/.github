# conquerOS Device source code guidelines.

You can check reference of used keyword [here](https://datatracker.ietf.org/doc/html/rfc2119).

## Device tree and Vendor Tree
* MUST have proper commit authorship
* MUST include working Proprietary files list
- MUST NOT ship any prebuilt APKs. Including Google Camera, GrapheneOS Camera
- MUST NOT contain any unused overlays
- MUST NOT include any features that doesn't exist on their stock ROM
- MUST NOT remove packages that comes from the ROM by default
- MUST NOT include any overlays that don't have anything to do with the device. e.g: QS Tile order
- MUST have Enforcing SELinux
- MAY include OEM Camera ports.

## Kernel Source
- MUST have complete commit history and proper authorship
- MUST NOT include any types of blocker e.g: Boeffla Wakelock Blocker, fs blocker
- MUST NOT include any types of Overclocking e.g: CPU/GPU Overclock. Screen Overclock