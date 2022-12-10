# Tips

## ubuntu
### First
- sudo apt update
- sudo apt -y install linux-oem
- sudo apt-get install gcc
- sudo apt install make
- sudo apt-get install git
- sudo apt-get install openssh-server
- sudo apt install net-tools

### grub
#### 1.disable for NVIDIA
```bash
sudo vim /etc/default/grub 
  GRUB_CMDLINE_LINUX_DEFAULT="quiet splash nomodeset"
sudo update-grub 

sudo vim /etc/modprobe.d/blacklist.conf
  blacklist nouveau
sudo update-initramfs -u
``` 

- cat /boot/grub/grub.cfg | grep memuentry

### Driver
- sudo ./NVIDIA-Linux-x86_64-515.65.01.run

### samba
#### samba server
- sudo apt-get install samba
- vim /etc/samba/smb.conf
```bash
[P1]
   comment = P1
   browseable = yes
   path = /home/andrew/samba_share
   guest ok = no
   writable = yes
   create mask = 0777
```
- sudo service smbd restart

- sudo apt-get install -y smbclient cifs-utils
- sudo mount -t cifs -o user=username  //ip_address/study  /local/samba_disk/
- sudo umount /local/samba_disk/

- 

