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
# 查看安装docker列表
```c
yum list docker-ce --showduplicates | sort -r
```

# 启动docker
```c
sudo systemctl start docker
```

# 使用docker的命令
```c
#查看docker的版本
docker -v

# 查看本地主机上已有镜像的基本信息。
docker images
```
