the local manifests:

	git clone https://github.com/Motorola-MT6737/local_manifest -b cm-14.1 .repo/local_manifests

Then sync up with this command:

	repo sync --force-sync -q
	
You can make the 4 higher depending on how fast your internet connection is. 

-------------
 
_Building from source_
---------------

	$ echo "export USE_CCACHE=1" >> ~/.bashrc
	$ prebuilts/misc/linux-x86/ccache/ccache -M 50G
	$ . build/envsetup.sh
	$ brunch codename
