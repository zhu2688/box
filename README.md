# vagrant box 
vagrant box php7开发环境

## box 文件保存在file分支
github上超过100M大文件必须用[LFS](https://git-lfs.github.com) 来上传

## 下载box后本地安装
- 下载box [https://github.com/zhu2688/vagrant_box/raw/file/centos/centos-6.9-x64.box](https://github.com/zhu2688/vagrant_box/raw/file/centos/centos-6.9-x64.box) 
- 下载Vagrantfile [Vagrantfile](https://raw.githubusercontent.com/zhu2688/vagrant_box/php7/centos/Vagrantfile)
- 下载centos69.sh [centos69.sh](https://raw.githubusercontent.com/zhu2688/vagrant_box/php7/centos/centos69.sh)


```shell
## 把上面三个脚本放到当前目录
vagrant box add php7 centos-6.9-x64.box
vagrant up
```

## 软件环境
-  vagrant 2.0.1
-  VirtualBox 5.1.30
-  GuestAdditions 5.1.30

## 简介
  vagrant 一个完整的box文件都特别大,所以使用base文件加上provision来初始化开发环境

```shell
  ├── centos
  │   ├── centos-6.9-x64.box  基本box
  │   ├── centos69.sh    初始化脚本
  │   ├── Vagrantfile    Vagrantfile 文件
```
  
## php环境

```shell
* Php7.2
* Mysql 5.6
* Redis 3.2
* Tengine 2.2.2
```