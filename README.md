
TECNO W4
==============
```
By : Nana Iyke Quame
```
![W4-BANNER](http://smartphonetobuy.com/wp-content/uploads/2016/04/Tecno-W4-Price-In-Nigeria.jpg)

The Tecno W4  (codenamed _"w4"_) was one of the smartphones with Android 6.0 out-of-the-box  from tecno.

This Device tree of Tecno W4 for Compiling TWRP

For more information about building read "manual"

Device Look :
==============
![TECNO W4](https://www.naijatechguide.com/wp-content/uploads/2016/04/tecno-w4.jpg)

Basic        | Spec Sheet
------------:|:------------------------
CPU          |  ARM Cortex A53 | 1.3GHz Quad-Core | MT6580
GPU          | ARM Mali-T720 MP2, 2-Cores
Memory       | 1GB RAM
Shipped Android Version | 6.0
Storage      | 16GB
Battery      | Non-Removable 2300 mAh Lithium-Ion
Display      | 5.0
Rear Camera | 8.0 MP , Video
Front Camera | 2.0 MP
Camera Features | LED Flash, Autofocus


# tecno_w4_device_tree

To clone tree automatically, then;
 `cd .repo && mkdir local_manifests`
 `cd local_manifests`

Add to `.repo/local_manifests/w4.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>

	<project path="device/tecno/w4" name="iykequame/android_device_tecno_w4" remote="github" revision="master" />

</manifest>
```

Then run `repo sync` or  `repo sync --force-sync`  to check it out.

or

`git clone https://github.com/iykequame/android_device_tecno_w4.git -b master  device/tecno/w4`


# How To Compile

```
 1. source build/envsetup.sh
 2. lunch
  and select your device from menu [select omni_w4-userdebug]
 3. mka -j5 recoveryimage
```
It will take time to compile your build/compile

 4. Find your compiled recovery - image in "$out/out/target/product/codename"


---------------
