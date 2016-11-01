Welcome to AOSP for Galaxy Grand Prime
======================================


Instructions
---------------

Initializing:

First, create a folder to hold the source code: 

	mkdir ~/aosp

Next..

	cd ~/aosp

Initialize local repository:

	repo init -u git://github.com/AOSP-RRO/manifest.git -b marshmallow

Also add the local manifests:

    git clone https://github.com/CarlosArriagaCM/localmanifest -b aosp-6.0 .repo/local_manifests

Sync up:

	repo sync --force-sync
	
---------------
 
_Building_
---------------

First:

	cd ~/aosp
	echo "export USE_CCACHE=1" >> ~/.bashrc
	~/aosp/prebuilts/misc/linux-x86/ccache/ccache -M 50G

Second:

	./build.sh fortuna3g or ./build.sh fortunave3g



