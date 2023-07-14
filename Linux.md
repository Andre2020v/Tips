## ubuntu install
- sudo apt install open-vm-tools (*)
- sudo apt-get install gcc
- sudo apt install make
- sudo apt-get install autoconf
- sudo apt-get install pkg-config
- sudo apt-get install autotools(*)
- sudo apt-get install git
- sudo apt-get install openssh-server
- sudo apt install net-tools
- sudo apt install python2.7
- sudo apt install python3-virtualenv
- sudo apt install python2-pip-whl
- sudo apt install python2-setuptools-whl
- virtualenv -p /usr/bin/python2.7 python27
- pip install formatter ( source python27/bin/activate )
- sudo apt install repo
- sudo apt install default-jdk
- git clone https://github.com/universal-ctags/ctags.git
- ./autogen.sh
- ./configure
- sudo make install
- tar zxvf apache-tomcat-10.1.11.tar.gz
- cd apache-tomcat-10.1.11/bin ; ./startup.sh
- mkdir opengrok
- mkdir opengrok/{src,data,dist,etc,log}
- tar -C opengrok/dist --strip-components=1 -xzf  opengrok-1.12.12.tar.gz
- 



## fd 命令用法



|                      |                                                              |
| -------------------- | ------------------------------------------------------------ |
| List all files       | fd   .   /path/to/dir                                        |
| 查看包含关键字的文件 | fd   "words"                                                 |
| 搜索特定的文件后缀   | fd   -e    json                                              |
|                      | fd   -g    '*.py'    -X   code                               |
|                      | fd   -g    '*.py'    -X   vim                                |
|                      | fd   -e cpp   -e cxx    -e h   -e  hpp   -X   rg 'std::cout' |
