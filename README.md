_LineageOS 14.1 for Motorola MediaTek Devices_
------------------------------------

Create directories

	$ mkdir los-15.0
	$ cd los-15.0

the local manifests:

	$ repo init -u git://github.com/LineageOS/android.git -b linegae-15.0
	$ git clone https://github.com/Motorola-MT6737/local_manifest -b lineage-15.0 .repo/local_manifests

Then sync up with this command:

	$ repo sync --force-sync -q

-------------
 
_Building from source_
---------------

	$ cd device/motorola/mt6737-common/patches
	$ ./check-patches.sh
	$ ./apply-patches.sh
	$ . build/envsetup.sh
	$ lunch lineage_device-userdebug
	$ make bacon -j8

-------------
 
_Credits:_
---------------
@darklord4822
@olegsvs 
@MediatekAndroidDevelopers 
@iykequame 
@SamarV-121 
@ashwinr64 
igor1144 
Decker 
danielhk 
mdeejay 
Zormax 
and more people :D
