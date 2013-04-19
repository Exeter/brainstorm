#Exeter Computing Club Server Setup
__Setup still in progress!__

##Hardware:
<table>
<tr><td>Motherboard</td><td>AMD A8-3850 Llano 2.9GHz Quad-Core Desktop APU</td></tr>
<tr><td>CPU</td><td>ASUS F1A75-M PRO FM1 AMD A75</td></tr>
<tr><td>CPU Fan</td><td>COOLER MASTER Hyper 212 EVO</td></tr>
<tr><td>SSD</td><td>Crucial M4 2.5" 64GB SATA III MLC SSD</td></tr>
<tr><td>RAM</td><td>G.SKILL Ripjaws Series 4GB (2 x 2GB) DDR3 1600</td></tr>
</table>
__(TODO: add psu and case)__


##Partitioning
    -- MBR Partition Table-- 

    512M	/boot	EXT4 
    8G		/	EXT4
    8G		/var	EXT4
    2G			swap
    30G		/home	EXT4

##Users and Groups
__(TODO: fill in with sudoers policy, etc.)__

##Server Software
__(TODO: Add httpd info (apache config). Also, nginx vs apache?)__

__(TODO: Format better)__

List of all manually installed packages:

__apache__
dialog
__gcc__
__git__
grub-bios
htop
__jdk7-openjdk__
nma
__nodejs__
openssh
__python__
__python2__
ranger
__ruby__
__sqlite__
__subversion__
sudo
vim
wget
wpa_supplicant
zsh


##To be implemented
- User account expiration
- Move machine to Mr. Sea's office
	- Give Mr. Sea root privilleges, disable visudo for all admins other than Mr. Sea

- Production mode: everything 'cept /var, /tmp and /home are read-only. 
- Upgrade mode: everything is readwrite, must be at computer though