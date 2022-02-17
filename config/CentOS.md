## **程序支持的CentOS版本**
### CentOS 7 
### CentOS 8
### *X86架构和ARM架构安装命令相同*
----------
## **CentOS 7 程序安装方式**

### 1、下载ubox.repo到/etc/yum.repos.d
    cd /etc/yum.repos.d && wget https://ubox-repo.ucloud.cn/repos/rpm/rhel8/ubox.repo


### 2、安装 ubox-videocontroller
    yum install ubox-videocontroller
ubox-videocontroller用于rtmp推流控制
安装过程中，因为首次使用ubox仓库，所以yum会先导入ubox仓库的公钥

### 3、安装 ubox-publisher
    yum install ubox-publisher
ubox-publisher用于硬件加速和rtmp推流

### **完成以上步骤则环境配置完成**

----------

## **CentOS 8 程序安装方式**

### 1、下载ubox.repo到/etc/yum.repos.d
    cd /etc/yum.repos.d && wget https://ubox-repo.ucloud.cn/repos/rpm/rhel8/ubox.repo

### 2、安装 ubox-videocontroller
    dnf install ubox-videocontroller
ubox-videocontroller用于rtmp推流控制
安装过程中，因为首次使用ubox仓库，所以yum会先导入ubox仓库的公钥

### 3、安装 ubox-publisher
    dnf install ubox-publisher
ubox-publisher用于硬件加速和rtmp推流

### **完成以上步骤则环境配置完成**