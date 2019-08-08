# Set Up Virtualbox Machine

### Download VirtualBox
https://www.virtualbox.org/wiki/Downloads


### Download OS Iso
* Download the live cd/installation media for the OS
* For Linux distro info: http://distrowatch.org
* Supported Formats
	* .iso, .dmg, .cdr, .cue, .viso
	* VDI  – Virtual Disk Image
	* VMDK – VMware virtual hard disk format
	* VHD  – Microsoft virtual hard disk format
	* HDD  – Parallels Version 2 format

### Create Virtual Machine
* Launch Virtual Box App
* On the top right, click 'New'
* Give the machine a name and select the type
	* The app is smart enough that if you name the machine 'arch' or 'windows' or 'osx' it will auto populate the type and machine

### Configure Machine
* When the machine is created it will show up on the left hand side of the VirtualBox app
* Highlight the virtual machine then click settings
* Under 'System' make sure Optical is before Hard Disk
Under 'Storage' click on the empty optical drive
* On the farthest right side click on the will be a small, blue disc image
* Navigate to the downloaded OS iso
* Save all settings
* Start the virtual machine
	* On the first boot, the machine will use the downloaded image file as the boot drive
	* Install the OS onto the hard drive of virtual machine