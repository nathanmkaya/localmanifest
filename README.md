Welcome to Cyanogenmod ROM for Galaxy Grand Prime
============================================


Instructions
---------------

Initializing:

First, create a folder to hold the source code: 

	mkdir ~/cm-14.1

Next..

	cd ~/cm-14.1

Initialize local repository:

	repo init -u git://github.com/CyanogenMod/android.git -b cm-14.1

Also add the local manifests:

    git clone https://github.com/CarlosArriagaCM/localmanifest -b cm-14.1 .repo/local_manifests

Sync up:

	repo sync --force-sync
	
---------------
 
_Building_
---------------

First:

	cd ~/cm-14.1
	echo "export USE_CCACHE=1" >> ~/.bashrc
	~/cm-14.1/prebuilts/misc/linux-x86/ccache/ccache -M 50G

Second:

	. build/envsetup.sh && brunch fortuna3g or brunch fortunave3g
