# Ubuntu
### **程序支持的Ubuntu版本**
#### Ubuntu 20.04 LTS (Focal Fossa) 
#### Ubuntu 18.04 LTS (Bionic Beaver)
*X86架构和ARM架构安装命令相同*
----------
## 程序安装方式

###  **1、获取公钥**
    sudo apt-key adv --fetch-keys http://ubox-deb.ucloud.cn/DEB-GPG-KEY-ubox                

###  **2、打开sources.list**
    sudo vim /etc/apt/sources.list

###  **3、编辑sources.list**
    deb http://ubox-deb.ucloud.cn/repos/deb/all focal ubox
在文本中另起一行插入：`deb http://ubox-deb.ucloud.cn/repos/deb/all focal ubox`，并保存

###  **4、更新软件包**
    sudo apt-get update

###  **5、安装 ubox-videocontroller**
    sudo apt-get install ubox-videocontroller
ubox-videocontroller用于rtmp推流控制

###  **6、安装 ubox-publisher**
    sudo apt-get install ubox-publisher
ubox-publisher用于硬件加速和rtmp推流

### **完成以上步骤则环境配置完成**
