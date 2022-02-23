# CentOS

程序支持的CentOS版本  
CentOS 7  
CentOS 8  
X86架构和ARM架构安装命令相同  


## CentOS 7 程序安装方式

1、下载ubox.repo到/etc/yum.repos.d

    cd /etc/yum.repos.d && wget https://ubox-repo.ucloud.cn/repos/rpm/rhel8/ubox.repo

ubox.repo的md5值为 7143e9bad3423a4363e91962193a39d7 可输入 md5sum ubox.repo 进行验证

2、安装epel源

    yum install epel-release

3、安装rpmfusion源   (国内、国外选其一即可)  

（1）国内源利用脚本下载安装（下载较快）

   \*下载脚本  

    wget https://github.com/ucloud/ubox-publisher/raw/master/util/add_rpmfusion_cn_mirror.sh；

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

    cd /etc/yum.repos.d && wget https://ubox-repo.ucloud.cn/repos/rpm/rhel8/ubox.repo

ubox.repo的md5值为 7143e9bad3423a4363e91962193a39d7 可输入 md5sum ubox.repo 进行验证

2、安装epel源

    dnf install epel-release

3、安装rpmfusion源   (国内、国外选其一即可)  
（1）国内利用脚本下载安装（下载较快）

   \*下载脚本  

    wget https://github.com/ucloud/ubox-publisher/raw/master/util/add_rpmfusion_cn_mirror.sh；

   \*为脚本添加执行权限  

    chmod +x add_rpmfusion_cn_mirror.sh

   \*执行脚本  

    ./add_rpmfusion_cn_mirror.sh

（2）国外直接下载安装（下载较慢）

    dnf localinstall --nogpgcheck https://download1.rpmfusion.org/free/el/rpmfusion-free-release-8.noarch.rpm

4、安装 ubox-videocontroller

    dnf install ubox-videocontroller

用于硬件加速、RTMP推流和推流控制。安装过程中，因为首次使用ubox仓库，所以dnf会先导入ubox仓库的公钥  