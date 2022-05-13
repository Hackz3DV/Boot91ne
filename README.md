# Boot91ne is finally here!

A super simple online exploit for IOS devices

## What's in it?

Boot91ne, responsive experience that you can't find anywhere else, with support for iOS versions from iOS 9.0.0 - 9.3.6, including iPod & iPhone devices.

---

## Supported Devices

All A7-A8 devices on iOS 9.0.0 - 9.3.6

---

## Repo structure & building

Repo structure & building
Frontend and WebKit exploit are in /root.
Kernel exploit is in /glue.
Post-exploitation is in /glue/dep.

DoubleH3lix and Meridian can be built independently into static libraries with make headless and make all respectively, in their directories.
Those are then used to build the payload in /glue, which is the binary that is ran from JIT after the WebKit exploit. Can be built with just a make, and will build all dependencies as needed.
And that is all finally strung together with the WebKit exploit by running make in /root, which will again build dependencies as needed.

