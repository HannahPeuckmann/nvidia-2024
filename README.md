# Nvidia and Mesa libraries for `base: core24` snaps

A content snap providing the Nvidia and Mesa userspace libraries and
drivers for core24-based snaps.

This supplies the gpu-2404 content interface:

Path|Description|Use
--|--|--
bin/gpu-2404-provider-wrapper|Sets up all the environment|Run your application through it
||
libdrm|Needed by mesa on AMD GPUs|Layout to /usr/share/libdrm
X11/XErrorDB|X11 locales etc|Layout to /usr/share/X11/XErrorDB
||
mir-quirks|(optional)Mir configuration|Mir specific

----

For more information about the `gpu-2404` interface, see: [The gpu-2404 snap interface](https://mir-server.io/docs/the-gpu-2404-snap-interface) documentation.

The repository license is GPL v3 with copyright Canonical LTD 2023,
however the license of the actual content snap is mixed license
(proprietary NVIDIA for NVIDIA libraries, and various open source
licenses for all other libraries). Installing this snap implies
accepting NVIDIA license terms.
