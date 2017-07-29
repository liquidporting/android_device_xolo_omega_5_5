## TWRP device tree for XOLO Omega 5.5 (omega_5_5)

Add to `.repo/local_manifests/omega_5_5.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project path="device/xolo/omega_5_5" name="android_device_xolo_omega_5_5" remote="liquidporting" revision="android-5.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_omega_5_5-eng
make -j5 recoveryimage
```
