## Folding
| Keyboard   | Function                                                     |
| ---------- | ------------------------------------------------------------ |
| zo         | Open one fold under the cursor.When a count is given, that many folds deep will be opened. |
| zO         | Open all folds under the cursor recursively.                 |
| zc         | Close one fold under the cursor. When a count is given, that many folds deep are closed.<br />折叠命令，e.g. 在括号内任意位置run可以折叠括号 |
| zC         | Close all folds under the cursor recursively.                |
| za         | When on a closed fold: open it. When on an open fold: close it and set 'foldenable'.<br />使用shift + v 选择要折叠的行，za 折叠 |
| zR         | Open all folds. This sets 'foldlevel' to highest fold level. |
| zf         | 折叠命令, 可以使用v 来选取要折叠的行，也可以用鼠标选择       |
| zf{count}j | 折叠命令, zf5j 向下折叠5行                                   |
| zf%        | 折叠命令，在括号出可以折叠括号内所有部分                     |
| zM         | 折叠所有，配合命令，zM  zo，打开最外的一层，zR 打开所有折叠  |


# VScode Native
## Edit
- Alt+上方向键: 使用vim visual mode选择 或者 使用鼠标选择


## vscode system  
首选项： 打开键盘快捷方式  
Preference： Open Keybaord Shortcuts  
Ctrl K  Ctrl  S


### smart selection
Windows/Linux:  shift alt left/right arrows  
Mac:            command ctrl shift left/right arrows



## 工作区切换
终端： 聚焦到终端        
资源管理器：             CTRL + SHIFT + E  
切换工作区：             CTRL + 1  


## plugin

### Bookmarks
Ctrl + ALT +  K    bookmarks on/off  
Ctrl + ALT +  J  
Ctrl + ALT +  L    jump next

## 光标移到

|              |                          |
|--------------|--------------------------|
|      w       | 下一个单词开头            |
|      b       | 本单词或上一个单词开头     |
|      e       | 本单词或下一个单词结尾     |
|      ge      | 上一个单词结尾            |
|      0       | 行首                     |


## 折叠
- 键入 v ， 开始选择要折叠的行，键入 zf
- 

## 文本处理
- 在visual mode [输入v]选择文本，读到文本宽度，例如80
- 然后输入 set textwidth=80
- gqq
