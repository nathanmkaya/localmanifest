Welcome to Pacman ROM for Galaxy Grand Prime
============================================


Instructions
---------------

Initializing:

First, create a folder to hold the source code: 

	mkdir ~/pac

Next..

	cd ~/pac

Initialize local repository:

	repo init -u git://github.com/PAC-ROM/pac-rom.git -b pac-6.0

Also add the local manifests:

    git clone https://github.com/CarlosArriagaCM/localmanifest -b pac-6.0 .repo/local_manifests

Sync up:

	repo sync --force-sync
	
---------------
 
_Building_
---------------

First:

	cd ~/pac
	echo "export USE_CCACHE=1" >> ~/.bashrc
	~/pac/prebuilts/misc/linux-x86/ccache/ccache -M 50G

Second:

	./build-pac.sh fortuna3g or ./build-pac.sh fortunave3g
