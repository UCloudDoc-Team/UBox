# X86架构 CentOS 8 配置过程如下


## 在终端依次执行以下指令

### - **指令1**
    cd /etc/yum.repos.d && wget  https://ubox-repo.ucloud.cn/repos/rpm/rhel8/ubox.repo

输入:`cd /etc/yum.repos.d && wget  https://ubox-repo.ucloud.cn/repos/rpm/rhel8/ubox.repo`                          
执行结果如下：
  ![](../images/centos8_x86_1.png)

### - **指令2**
    yum install modem_manager

输入：`yum install modem_manager` 安装过程中需要输入两次y
执行结果如下：
  ![](../images/centos8_x86_2.png)

### **完成以上步骤则环境配置完成**