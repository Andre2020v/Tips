# Tips
## pacman
pacman -Su
pacman -Sy base-devel
pacman -Sy mingw-w64-x86_64-toolchain

## Python
- pip install PyExifTool
- pip install exiv2

## Anaconda
- conda update -n base -c defaults conda
- conda create -n py39 python=3.9
- conda activate py39
- conda install scikit-image numpy matplotlib pillow  tqdm scipy notebook pandas openpyxl seaborn GitPython pyserial humanize
- conda env create -f environment.yml 
- conda remove --name env_name --all
- C:\ProgramData\anaconda3\
| 操作        | 命令                                     |
| --------- | -------------------------------------- |
| 查看所有环境    | `conda env list` 或 `conda info --envs` |
| 删除某个环境    | `conda remove -n 环境名 --all`            |
| 导出环境配置    | `conda env export > environment.yml`   |
| 用配置文件重建环境 | `conda env create -f environment.yml`  |



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



## hash

da29b9b1b7e081f55b9e33b703988c4d

518245f9ddef0c511d8e84a16eb00670
