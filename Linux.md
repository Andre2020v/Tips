## fd 命令用法



|                      |                                                              |
| -------------------- | ------------------------------------------------------------ |
| List all files       | fd   .   /path/to/dir                                        |
| 查看包含关键字的文件 | fd   "words"                                                 |
| 搜索特定的文件后缀   | fd   -e    json                                              |
|                      | fd   -g    '*.py'    -X   code                               |
|                      | fd   -g    '*.py'    -X   vim                                |
|                      | fd   -e cpp   -e cxx    -e h   -e  hpp   -X   rg 'std::cout' |
