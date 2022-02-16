# 程序支持 CentOS 7 和 CentOS 8
&nbsp;
# X86架构和ARM架构安装命令相同
&nbsp;
## ** CentOS 7 程序安装方式如下 **

###  **1、输入如下指令**
    cd /etc/yum.repos.d && wget https://ubox-repo.ucloud.cn/repos/rpm/rhel8/ubox.repo

输入:`cd /etc/yum.repos.d && wget https://ubox-repo.ucloud.cn/repos/rpm/rhel8/ubox.repo`  下载文件                        

###  **2、输入如下指令**
    yum install ubox-videocontroller

输入：`yum install ubox-videocontroller` 安装 ubox-videocontroller。安装过程中，因为是首次使用ubox仓库，所以yum会先导入ubox仓库的公钥

###  **3、输入如下指令**
    yum install ubox-publisher

输入：`yum install ubox-publisher` 安装 ubox-publisher。

### **完成以上步骤则环境配置完成**

&nbsp;
&nbsp;
&nbsp;

## ** CentOS 8 程序安装方式如下 **

###  **1、输入如下指令**
    cd /etc/yum.repos.d && wget  https://ubox-repo.ucloud.cn/repos/rpm/rhel8/ubox.repo

输入:`cd /etc/yum.repos.d && wget  https://ubox-repo.ucloud.cn/repos/rpm/rhel8/ubox.repo`  下载文件                        

###  **2、输入如下指令**
    dnf install ubox-videocontroller

输入：`dnf install ubox-videocontroller` 安装 ubox-videocontroller。安装过程中，因为是首次使用ubox仓库，所以yum会先导入ubox仓库的公钥

###  **3、输入如下指令**
    dnf install ubox-publisher

输入：`dnf install ubox-publisher` 安装 ubox-publisher。

### **完成以上步骤则环境配置完成**