# Linux 命令速记（实验一）

## 目录操作
- `ls` 列出目录内容
- `cd <dir>` 切换目录
- `mkdir <dir>` 创建目录
- `rm -r <dir>` 删除目录
- `pwd` 显示当前路径

## 文件查看
- `cat <file>` 从头显示文件
- `head -n 5 <file>` 只看前 5 行
- `tail <file>` 只看末尾几行
- `less <file>` 分页查看

## Git 常用
- `git init` 初始化仓库
- `git add .` 添加全部到暂存区
- `git commit -m "说明"` 提交
- `git push origin master` 推送

## SSH 443 方案（2026-11-04 配置）
- 22 端口被网络屏蔽时，改走 `ssh.github.com:443`
- 密钥副本位置：`C:\Users\Public\ssh\id_rsa`
- 测试命令：`ssh -T -i C:/Users/Public/ssh/id_rsa -o HostName=ssh.github.com -p 443 git@github.com`
- 仓库级配置：`git config core.sshCommand "ssh -i C:/Users/Public/ssh/id_rsa -o HostName=ssh.github.com -p 443"`
