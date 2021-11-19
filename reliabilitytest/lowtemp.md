# 低温运行测试

#### 实验目的：

1. 检验试件能否在长期的低温环境中储藏、操纵控制。
2. 确定军民用设备在低温条件下储存和工作的适应性及耐久性以及低温下材料物理化学性能。

#### 参考标准：
IEC 60068-2-1:2007《电工电子产品环境试验 第1部分 试验A：低温》
注：IEC标准是 ( International Electrotechnical Commission)国际电工委员会标准的简称。

#### 测试日期：
2021.10.26～2021.10.27

#### 试验场地：
苏州源控电子科技有限公司-硬件可靠性实验室

实验室环境：温度: 25±10℃   湿度: 50±25 % RH

#### 测试设备：
温湿度实验箱 (YK-04)  设备品牌：庆声科技股份有限公司   设备模型: KTHE-615TBS 

#### 测试条件：

1. 测试温度：-30℃
2. 温度变化率：1℃/分钟 
3. 系统状态：运行 
4. 测试时长：-30℃运行24小时 

#### 测试照片：
![low1](../images/low1.png)
## CPU温度分析

###### 环境温度数据来源：温湿度实验箱(YK-04)
![low3](../images/low3.png) 
上图为UBox所处环境的温度数据，UBox在-30摄氏度环境温度中运行24小时。

###### CPU温度数据来源：UBox控制台
![low3](../images/low4.png) 
上图为UBox在的温湿度实验箱中随环境温度变化而变化的CPU温度数据。

数据分析：在环境温度为-30℃时，UBox稳定运行，CPU温度稳定在-8℃。
## 网络信号分析

###### 双卡4G信号数据来源：UBox控制台
![low3](../images/low5.png) 

上图为UBox在低温测试过程中（25℃>> -30℃ >> 25℃）的双卡4G信号，SIM卡1为中国移动4G物联网卡，SIM卡2为中国电信4G物联网卡。

数据分析：整个实验过程中两张SIM信号都保持稳定，环境温度与SIM卡信号强度无直接关系。
## 网络延迟分析
UBox通过ping指定ip来获取延迟数据。以此来判断网络质量好坏。测试期间ping两个指定ip的延迟数据，ping每个ip各3万次。

###### Ping 114.114.114.114（国内）延迟数据来源：UBox数据库
![low3](../images/low6.png) 
###### Ping 8.8.8.8（全球）延迟数据来源：UBox数据库
![low3](../images/low7.png) 
数据分析：整个测试过程中，ping 114.114.114.114延迟集中在60ms左右，ping 8.8.8.8延迟集中在90ms左右，网络延迟与温度无直接关系。

## 性能分析
UBox采集各项数据并写入本地，分指标统计每3s左右的插入量。以此项来判断盒子性能是否正常。
###### 常温（环温+23℃）环境下数据来源：UBox本地数据
![low3](../images/low8.png) 
###### 低温（环温-30℃）环境下数据来源：UBox本地数据库
![low9](../images/low9.png) 
数据分析：环境温度为-30℃时，CPU温度稳定在-8℃左右。此时UBox性能未受明显影响。数据采集、写入本地的速率与常温环境无明显差距。 

## 综合分析

###### 硬件实验室测试分析：

 1. 硬件功能未受损。
 2. 硬件未发现退化。
 3. 性能保持不变，未见不可逆的物理损坏或退化。

###### UCloud功能测试分析：

 1. UBox网络功能未受-30℃环境温度影响。
 2. 4G网络信号未受-30℃环境温度影响。
 3. 4G网络延迟未受-30℃环境温度影响。
 4. UBox性能未受-30℃环境温度影响。
