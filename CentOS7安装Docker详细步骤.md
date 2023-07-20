# 安装docker依赖包
```c
#安装所需资源包
sudo yum install -y yum-utils
#设置docker下载地址
sudo yum-config-manager \
    --add-repo \
    https://download.docker.com/linux/centos/docker-ce.repo
    
#安装docker
sudo yum install docker-ce docker-ce-cli containerd.io
```
