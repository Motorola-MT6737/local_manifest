the local manifests:

	git clone https://github.com/CarlosArriagaCM/local_manifest -b perry .repo/local_manifests

Then sync up with this command:

	repo sync --force-sync
	
You can make the 4 higher depending on how fast your internet connection is. 

-------------
 
_Building from source_
---------------

	$ echo "export USE_CCACHE=1" >> ~/.bashrc
	$ prebuilts/misc/linux-x86/ccache/ccache -M 50G
	$ . build/envsetup.sh
	$ brunch codename
