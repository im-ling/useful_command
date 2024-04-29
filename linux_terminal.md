### 查找文件
find . -name symbolicatecrash

### 解压
tar -xzvf file.tar.gz

### 压缩
tar -czvf file.tar.gz file

### 架构
arch


### 查看进程
ps aux

### screen 命令

screen -ls

screen -S new_window_name

11723.3156.audio_server (Detached)

screen -r 3156.audio_server

screen -d -r 3156.audio_server

`exit` 退出当前window


### ssh key 生成
ssh-keygen -t ed25519 -C "test@example.com"

### git 配置
git config --global user.email "test@example.com"
git config --global user.name "ling"