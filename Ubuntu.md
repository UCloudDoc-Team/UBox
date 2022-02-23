# Ubuntu
程序支持的Ubuntu版本
Ubuntu 20.04 LTS (Focal Fossa)  
Ubuntu 18.04 LTS (Bionic Beaver)  
X86架构和ARM架构安装命令相同  
## 程序安装方式

1、获取公钥

    sudo apt-key adv --fetch-keys http://ubox-deb.ucloud.cn/DEB-GPG-KEY-ubox                

2、打开sources.list

    sudo vim /etc/apt/sources.list

3、编辑sources.list

    deb http://ubox-deb.ucloud.cn/repos/deb/all focal ubox

在文本中另起一行插入以上内容并保存

4、更新软件包

    sudo apt-get update

5、安装 ubox-videocontroller

    sudo apt-get install ubox-videocontroller
    
用于硬件加速、RTMP推流和推流控制。安装过程中，因为首次使用ubox仓库，所以yum会先导入ubox仓库的公钥。 

