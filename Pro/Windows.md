
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

### Bandizip
#### taof  
- A***0385
