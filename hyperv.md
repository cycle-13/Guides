# Configure a Hyper-V OS

### Turn on Hyper-V
Start --> Windows Features
Check the Hyper-V box on
Reboot machine

### Configure VM
Start --> Hyper-V Manager
One the left side , right click on the name of the machine then click on 'Quick Create'
Install OS from downloaded .iso
To configure network
* Type “nmcli d” command in your terminal for quick list ethernet card installed on your machine
* Type “nmtui” command in your terminal to open Network manager. After opening Network manager chose “Edit connection” and press Enter (Use TAB button for choosing options)
* Choose you network interfaces and click 'Edit'
* DHCP: Choose “Automatic” in IPv4 CONFIGURATION and check Automatically connect check box and press OK and quit from Network manager
* Reset network services > service network restart