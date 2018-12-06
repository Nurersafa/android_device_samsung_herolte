## TWRP device tree for Galaxy S7 (International & Canadian Exynos)

Add to `.repo/local_manifests/herolte.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project path="device/samsung/herolte" name="android_device_samsung_herolte" remote="TeamWin" revision="android-8.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_herolte-eng
make -j5 recoveryimage
```

