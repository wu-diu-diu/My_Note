# vscode配置远程服务器踩坑分享

## 1.按照网上标准步骤操作
- 安装remote-ssh插件
- 添加远程服务器(ip地址，用户名，密码)
- 添加完之后连接，卡在**Downloading Server**不动了
- 如果没有卡在上面这一步，那么按照教程很快就能配置好

## 2.网络原因
1. 国内网络原因导致在服务器上下载vscode-server缓慢甚至失败  
2. 采用本地下载(如果本地有VPN)，再scp到服务器
3. 或者先ssh连接服务器，再在服务器上手动下载
## 3.commit_id  
- 在vscode的问题日志内上找到commit_id  
- 使用使用**`curl`**工具从`vscode`官方服务器下载vscode-server的tar.gz 压缩包。
- 用scp工具将压缩包上传到服务器
- ssh连接远程服务器，将压缩包解压到指定文件夹下即可
## 4.具体命令详见CSDN
[链接1](https://blog.csdn.net/zhaxun/article/details/120568402)
[链接2](https://blog.csdn.net/wpqgt/article/details/143838069)
[链接3](https://blog.csdn.net/JACKLJ1998/article/details/120019742)