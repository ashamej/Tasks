# 

|                             问题                             |                          原因                          |                      解决方案 (from AI)                      |
| :----------------------------------------------------------: | :----------------------------------------------------: | :----------------------------------------------------------: |
| **初始化步骤出现syntax error near unexpected token `newline'** | 执行远程仓库的关联相关的代码中**出现了其余字符**，如<> |                       删去多余特殊字符                       |
| **传输文件时出现error：src retspec main aoes not match any** | **初始化时的分支命名与传输分支名的不同导致的传输失败** | 使用**git branch -m 初始化分支名 传输分支** 重命名初始化分支 |
| **传输文件时出现[relected]      main -> main (ftetch first)** | **本地分支 `main` 和远程仓库的 `main` 分支历史不一致** | 1. 强制推送使本地分支覆盖远程分支，即使用**git push -u origin main --force** 命令                                                                                                                             2.**拉取远程 `main` 分支并合并到本地**，即使用**git pull origin main --allow-unrelated-histories** |

