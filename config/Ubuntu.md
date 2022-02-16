# 程序支持 
### Ubuntu 20.04 LTS (Focal Fossa) 
### Ubuntu 18.04 LTS (Bionic Beaver)
&nbsp;
# X86架构和ARM架构安装命令相同
&nbsp;
## 程序安装方式如下

###  **1、输入如下指令**
    sudo apt-key adv --fetch-keys http://ubox-deb.ucloud.cn/DEB-GPG-KEY-ubox
输入`sudo apt-key adv --fetch-keys http://ubox-deb.ucloud.cn/DEB-GPG-KEY-ubox`获取公钥                   

###  **2、输入如下指令**
    sudo vim /etc/apt/sources.list
输入`sudo vim /etc/apt/sources.list`配置 source

###  **3、按“i”打开编辑模式，加入以下内容,编辑结束后wq保存**
    deb http://ubox-deb.ucloud.cn/repos/deb/all focal ubox
在文末输入`deb http://ubox-deb.ucloud.cn/repos/deb/all focal ubo`，编辑后保存

###  **4、输入如下指令**
    sudo apt-get update
输入`sudo apt-get update`更新软件包

###  **5、输入如下指令**
    sudo apt-get install ubox-videocontroller
输入`sudo apt-get install ubox-videocontroller`安装/升级软件包

###  **6、输入如下指令**
    sudo apt-get install ubox-publisher
输入`sudo apt-get install ubox-publisher`安装/升级软件包

### **完成以上步骤则环境配置完成**
