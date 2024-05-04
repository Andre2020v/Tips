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
- cp opengrok/dist/doc/logging.properties opengrok/etc
- cp opengrok/dist/lib/source.war  apache-tomcat-10.1.11/webapps/
- cp ~/work/opengrok/dist/tools/opengrok-tools.tar.gz   .
- sudo apt install python3.10-venv
- python3 -m venv env
- . ./env/bin/activate
- pip install opengrok-tools.tar.gz
- opengrok-deploy -c opengrok/etc/configuration.xml     opengrok/dist/lib/source.war apache-tomcat-10.1.11/webapps/
- opengrok-indexer     -J=-Djava.util.logging.config.file=opengrok/etc/logging.properties     -a opengrok/dist/lib/opengrok.jar --     -c /usr/local/bin/ctags     -s opengrok/src -d opengrok/data -H -P -S -G     -W opengrok/etc/configuration.xml -U http://localhost:8080/source
- mkdir work/tools
- git clone --depth 1 https://github.com/junegunn/fzf.git ~/.fzf  ;  ~/.fzf/install
- sudo apt install fd-find
- ln -s $(which fdfind) ~/.local/bin/fd
- sudo apt-get install ripgrep



## fd 命令用法



|                      |                                                              |
| -------------------- | ------------------------------------------------------------ |
| List all files       | fd   .   /path/to/dir                                        |
| 查看包含关键字的文件 | fd   "words"                                                 |
| 搜索特定的文件后缀   | fd   -e    json                                              |
|                      | fd   -g    '*.py'    -X   code                               |
|                      | fd   -g    '*.py'    -X   vim                                |
|                      | fd   -e cpp   -e cxx    -e h   -e  hpp   -X   rg 'std::cout' |
