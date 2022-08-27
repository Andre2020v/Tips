# Tips

## ubuntu
### First
- sudo apt update
- sudo apt -y install linux-oem
- sudo apt-get install gcc
- sudo apt install make
- sudo apt-get install git
- sudo apt-get install openssh-server

### grub
#### 1.disable for NVIDIA
sudo vim /etc/default/grub
  ```bash
   GRUB_CMDLINE_LINUX_DEFAULT="quiet splash nomodeset"
  ``` 
sudo update-grub

- sudo vim /etc/modprobe.d/blacklist.conf
  blacklist nouveau
- sudo update-initramfs -u

- cat /boot/grub/grub.cfg | grep memuentry

### Driver
- sudo ./NVIDIA-Linux-x86_64-515.65.01.run

### samba
- sudo apt-get install -y smbclient cifs-utils
- sudo mount -t cifs -o user=username  //ip_address/study  /local/samba_disk/
- sudo umount /local/samba_disk/



