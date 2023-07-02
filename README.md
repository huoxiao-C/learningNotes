# 腾讯云Centos7系统konga部署

## 代码下载
git clone https://github.com/pantsel/konga.git

## 安装konga
cd konga 
npm i 

**note**
npm安装过程中可能存在的问题：
1）python使用的版本为python3，实际需要的版本为python2.7，那么在安装时需要指定python版本，将`npm i`命令改为`npm i -python=python2.7`
2）centos7的gnu版本过低（4.8.5），在安装时通常报如下的错误：error: unrecognized command line option ‘-std=gnu++14，该问题需要升级centos7系统的gnu版本，升级方法如博文https://blog.csdn.net/weixin_42744102/article/details/107219137所示，在升级完gnu版本过后，需要将/usr/bin目录下的gnu命令指向新安装的gnu版本，新安装的gnu版本存储在/opt目录下
3）在升级完gnu的版本过后，仍可能报如下错误：named 'remove_cv_t' in namespace 'std'，通过将`npm i`命令更改为`CXXFLAGS="--std=c++14" npm i`即可解决。

