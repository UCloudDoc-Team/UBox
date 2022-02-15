<!--
 * @Descripttion: 
 * @version: 
 * @Author: irene.wang
 * @Date: 2021-11-17 14:47:20
 * @LastEditors: irene.wang
 * @LastEditTime: 2021-11-19 09:49:15
-->
# 概览

无人化智能盒子是基于智能硬件的一站式上云方案。

支持以下功能：

- 能通过 4G/5G接入Internet，同时支持双4G链路聚合，提升带宽
- 在客观条件的极限下，通过各种软件保证传输网络的稳定
- 快速组网，搭建加密局域网络
- 搭配UCloud自研云联网技术，封装加密隧道，简单配置后即可加密上云
- 支持多地域接入，支持全球网络加速
- 提供实时监控app，数据查看至赫兹级别


#### <center>[ 功能介绍](#1功能介绍)   |   [可靠性分析](#可靠性分析)   ｜    [操作指南](#3操作指南)  |     [应用场景](#4应用场景)  |     [推流端环境配置](#5推流端环境配置) </center>



## 1.功能介绍

* [网络稳定性保障](/UBox/function/stability.md)
* [自动容灾](/UBox/function/recovery.md)

## 2.可靠性分析

* [总测试](UBox/reliabilitytest/overview.md) 
* [低温运行测试](/UBox/reliabilitytest/lowtemp.md)
* [高温运行测试](/UBox/reliabilitytest/hightemp.md)
* [正弦振动测试](/UBox/reliabilitytest/sinevibration.md)
* [随机振动测试](/UBox/reliabilitytest/randomvibration.md)
* [冲击试验 (关机状态测试)](/UBox/reliabilitytest/impacttest.md)


## 3.操作指南

* 无人化智能盒子  
     * [购买](/UBox/guide/buy)
     * [激活](/UBox/guide/activate)
     * [配置内网](/UBox/guide/LAN.md)
* 监控数据
     * [查看]( /UBox/guide/check)
     * [下载](/UBox/guide/download)
     * [如何查询是否双卡](/UBox/guide/dual-sim.md)
     * [如何查询双卡信号值](/UBox/guide/signal.md)

## 4.应用场景

* [无人化港口场景](/UBox/strategy/port.md)
* [电商应用场景](/UBox/strategy/ecommerce.md)


## 5.推流端环境配置

* [CentOS]
    * [CentOS7](/UBox/config/CentOS7.md)
    * [CentOS8](/UBox/config/CentOS8.md)
* [Ubuntu]
    * [Ubuntu18](/UBox/config/Ubuntu18.md)
    * [Ubuntu20](/UBox/config/Ubuntu20.md)
* [Windows]
    * [Windows](/UBox/config/Windows.md)