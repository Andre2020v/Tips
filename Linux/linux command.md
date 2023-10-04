## find 

```bash
find -type f -name '*.c' | xargs grep 'chart'
```



## fd 命令用法

```bash
# List all files
fd . /path/to/dir

# 查看包含关键字的文件
fd   "words"

# 搜索特定的文件后缀
fd   -e    json

# 在当前目录及其子目录中搜索所有以 .cpp、.cxx、.h 和 .hpp 结尾的文件，并排除包含字符串 'std::cout' 的文件
fd   -e cpp   -e cxx    -e h   -e  hpp   -X   rg 'std::cout'
```


