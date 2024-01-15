# VScodeVim
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
- Alt+上方向键(UpArrow): 向上移动行, 可以使用vim visual mode选择 或者 使用鼠标选择
```bash
{
  "key": "alt+up",
  "command": "editor.action.moveLinesUpAction",
  "when": "editorTextFocus && !editorReadonly"
}
```

## Multi
- 按 Alt 键，鼠标点击不同位置
- 按 Ctrl + Alt , 按键盘 向上或者向下 的键
- 选中一段文字，按shift+alt+i，可以在每行末尾出现光标
- 光标放在一个地方，按ctrl+shift+L或者ctrl+f2，可以在页面中出现这个词的不同地方都出现光标
- 按shift+alt，再使用鼠标拖动，也可以出现竖直的列光标，同时可以选中多列
- 任何光标操作，可以按Ctrl + U取消

## Move
- Ctrl + 9 : 查看: 打开组中最后一个编辑器
```bash
 {
  "key": "ctrl+9",
  "command": "workbench.action.lastEditorInGroup"
 }
```

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

## 选中
- 分别更改这些配对标点符号中的文本内容
  ci’、ci”、ci(、ci[、ci{、ci< -

- 分别删除这些配对标点符号中的文本内容
  di’、di”、di(或dib、di[、di{或diB、di< -

- 分别复制这些配对标点符号中的文本内容
  yi’、yi”、yi(、yi[、yi{、yi< -

- 分别选中这些配对标点符号中的文本内容
  vi’、vi”、vi(、vi[、vi{、vi< -
