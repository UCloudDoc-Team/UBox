# ubox-videocontroller 安装指南

软件支持

|  arch / paltform   |  arm64 |   amd64  | x86_64  | i386  |
|  :----  | :----  | :---- | :----  | :----  |
|  Ubuntu 20.04 LTS Focal  | 支持 | 支持 | 支持 | 不支持 |
|  Ubuntu 18.04 LTS Bionic  | 支持 | 支持 | 支持 | 不支持 |
| centos7  | 支持 | 支持 | 支持 | 不支持 |
| centos8  | 支持 | 支持 | 支持 | 不支持 |
 
## CentOS 7 程序安装方式

1、下载ubox.repo到/etc/yum.repos.d

    curl -sL https://ubox-repo.ucloud.cn/repos/rpm/7/ubox.repo | sudo tee /etc/yum.repos.d/ubox.repo

ubox.repo的md5值为 7143e9bad3423a4363e91962193a39d7 可输入 md5sum ubox.repo 进行验证

2、安装epel源

    yum install epel-release

3、安装rpmfusion源  (国内、国外选其一即可)

（1）国内源利用脚本下载安装（下载较快）

   \*下载脚本  

    wget https://github.com/ucloud/ubox-publisher/raw/master/util/add_rpmfusion_cn_mirror.sh

   \*为脚本添加执行权限  

    chmod +x add_rpmfusion_cn_mirror.sh

   \*执行脚本  

    ./add_rpmfusion_cn_mirror.sh

（2）国外源直接下载安装（下载较慢）

    yum localinstall --nogpgcheck https://download1.rpmfusion.org/free/el/rpmfusion-free-release-8.noarch.rpm

4、安装 ubox-videocontroller

    yum install ubox-videocontroller

用于硬件加速、RTMP推流和推流控制。安装过程中，因为首次使用ubox仓库，所以yum会先导入ubox仓库的公钥  

----------


## CentOS 8 程序安装方式

1、下载ubox.repo到/etc/yum.repos.d

    curl -sL https://ubox-repo.ucloud.cn/repos/rpm/7/ubox.repo | sudo tee /etc/yum.repos.d/ubox.repo

ubox.repo的md5值为 7143e9bad3423a4363e91962193a39d7 可输入 md5sum ubox.repo 进行验证

2、安装epel源

    dnf install epel-release

3、安装rpmfusion源   (国内、国外选其一即可)

（1）国内利用脚本下载安装（下载较快）

   \*下载脚本  

    wget https://github.com/ucloud/ubox-publisher/raw/master/util/add_rpmfusion_cn_mirror.sh

   \*为脚本添加执行权限  

    chmod +x add_rpmfusion_cn_mirror.sh

   \*执行脚本  

    ./add_rpmfusion_cn_mirror.sh

（2）国外直接下载安装（下载较慢）

    dnf localinstall --nogpgcheck https://download1.rpmfusion.org/free/el/rpmfusion-free-release-8.noarch.rpm

4、安装 ubox-videocontroller

    dnf install ubox-videocontroller

用于硬件加速、RTMP推流和推流控制。安装过程中，因为首次使用ubox仓库，所以dnf会先导入ubox仓库的公钥  


## Ubuntu 程序安装方式
1、配置sources

   \*定义REPO变量  

    REPO=$(lsb_release -cs)                

   \*添加ubox.list

    echo "deb http://ubox-deb.ucloud.cn/repos/deb/all $REPO ubox" | sudo tee /etc/apt/sources.list.d/ubox.list

2、获取公钥

    curl -sL http://ubox-deb.ucloud.cn/DEB-GPG-KEY-ubox | gpg --dearmor | sudo tee /etc/apt/trusted.gpg.d/ubox.gpg


3、更新软件包

    sudo apt-get update

4、安装 ubox-videocontroller

    sudo apt-get install ubox-videocontroller
    
用于硬件加速、RTMP推流和推流控制。安装过程中，因为首次使用ubox仓库，所以yum会先导入ubox仓库的公钥。 