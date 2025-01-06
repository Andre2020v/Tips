
Get-ExecutionPolicy -List

        Scope ExecutionPolicy
        ----- ---------------
MachinePolicy       Undefined
   UserPolicy       Undefined
      Process       Undefined
  CurrentUser    RemoteSigned
 LocalMachine       AllSigned

Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser

组策略	                        执行策略
允许所有脚本	                Unrestricted
允许本地脚本和远程签名脚本	RemoteSigned
仅允许签名脚本	                AllSigned

## 安装字体
- https://www.nerdfonts.com/font-downloads
- 下载FiraCode Nerd Font
- Windows 个性化> 字体， 浏览并安装字体 (通过搜索 字体设置 可以直达)
- 

## Cherry 键盘

FN 键常亮 ：  按Ctrl 后再按FN 可以取消


C:\Users\xxx\AppData\Roaming



## 操作无法完成因为文件已在中打开
打开 ‘任务管理器’——‘性能’——‘打开资源监视器’——‘CPU’——'关联的句柄’ 在‘关联的句柄’处检索刚刚删不掉的文件夹或文件的名称， 根据搜索结果，右键选择‘结束进程’，返回目录再次删除文件夹或文件即可成功删除


## Conda
C:\ProgramData\anaconda3\Scripts\conda.exe
