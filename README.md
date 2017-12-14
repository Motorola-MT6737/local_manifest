_LineageOS 14.1 for Moto E4 Devices_
------------------------------------

Create directories

	$ mkdir cm-14.1
	$ cd cm-14.1

the local manifests:

	$ repo init -u git://github.com/LineageOS/android.git -b cm-14.1
	$ git clone https://github.com/Motorola-MT6737/local_manifest -b cm-14.1 .repo/local_manifests

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
