# ubox-videocontroller 安装指南

软件支持

|  x86   |  arm64 | 
|  :----  | :----  | 
| 支持 | 待支持 | 

目前推流仅支持 YUYV 像素格式，启动前需先使用 V4L2 把摄像头 pixelformat 设置为 YUYV

查看摄像头是否支持 YUYV :

    v4l2-ctl -d1 --list-formats

若支持 YUYV 则将摄像头 pixelformat 设置为 YUYV

    v4l2-ctl --device /dev/video0 --set-fmt-videos=pixelformat=YUYV

安装 ubox-videocontroller  

   \*创建挂载日志目录
   
    mkdir -p /var/log/ubox-videocontroller /var/log/ubox-publisher/publisher/

   \*安装需要root权限
   
    docker container run -v /dev:/dev -v /sys/class:/sys/class -v /var/log/ubox-videocontroller:/var/log/ubox-videocontroller -v /var/log/ubox-publisher:/opt/ucloud/ubox-videocontroller/log --net host -d --privileged ucloudubox/ubox-videocontroller:latest




参数详解：
-v /dev,/sys/class 用来识别 v4l2 摄像头 

--net host 使用 hosts 模式启动，程序启动需要与外部通信，为保证网络可用性，最好设置为 host 模式 

-d daemon 模式 

--privileged 程序读摄像头需要权限 
