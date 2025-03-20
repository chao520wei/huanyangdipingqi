# 香港 Evoxt VPS 性能测评与分析

> 香港 Evoxt VPS 托管于 Mega2 机房，共享 100Mbps 带宽，配备 3.5 GHz 高频 CPU，性能表现值得关注。

## 服务器位置与 IP 信息

香港 Evoxt VPS 提供多个地区的服务器节点，以下是部分 IP 地址信息：

- **美国**：`103.179.142.254`
- **马来西亚**：`193.57.57.254`
- **香港**：`154.91.202.254`

## 测试套餐概览

本次测评选用香港 VM-3 套餐，定价为每月 **11.99 美元**，适合中小型网站托管或个人开发者使用。以下为详细性能分析。

## 基本配置参数

香港 Evoxt VPS 的基础配置如下：

plaintext
CPU 型号         : QEMU Virtual CPU version 2.5+
CPU 核心         : 4 核 @ 3593.246 MHz
CPU 缓存         : 512 KB
AES-NI           : ✘ 未启用
VM-x/AMD-V       : ✘ 未启用
硬盘容量         : 1.5 GB / 29.8 GB
内存大小         : 71.2 MB / 3.8 GB
系统运行时间     : 0 天 0 小时 23 分钟
系统负载         : 0.00, 0.00, 0.00
操作系统         : Debian GNU/Linux 11 x86_64 (64 位)
内核版本         : 5.10.0-8-amd64
TCP 拥塞控制     : cubic
虚拟化技术       : KVM

此配置适用于轻量级应用场景，如搭建个人博客或小型 API 服务。

👉 [2025年最新Evoxt优惠码和云服务器方案套餐整理汇总](https://bit.ly/evoxt)

## CPU 性能表现

基于 sysbench 的 CPU 测试结果如下：

plaintext
单线程测试      : 4040 分
四线程测试      : 16103 分

香港 Evoxt VPS 的 CPU 性能在多线程任务中表现出色，适合需要并行计算的应用。

## 内存性能测试

内存读写速度测试结果如下：

plaintext
单线程读取速度  : 48147.62 MB/s
单线程写入速度  : 15673.12 MB/s

内存性能优异，能够满足高吞吐量的需求，如数据库缓存或静态文件服务。

## 硬盘读写性能

### DD 测试结果

plaintext
测试项          写入速度                读取速度
10MB-4K 块     65.0 MB/s              30.6 MB/s
10MB-1M 块     1.8 GB/s               1.3 GB/s
100MB-4K 块    58.8 MB/s              25.3 MB/s
100MB-1M 块    2.1 GB/s               2.0 GB/s
1GB-4K 块      59.6 MB/s              27.5 MB/s
1GB-1M 块      2.1 GB/s               2.1 GB/s

### FIO 测试结果

plaintext
块大小 | 读取速度 (IOPS)       | 写入速度 (IOPS)       | 总速度 (IOPS)
4k     | 464.49 MB/s (116.1k) | 465.71 MB/s (116.4k) | 930.20 MB/s (232.5k)
64k    | 1.68 GB/s (26.2k)    | 1.69 GB/s (26.4k)    | 3.37 GB/s (52.6k)
512k   | 2.08 GB/s (4.0k)     | 2.19 GB/s (4.2k)     | 4.28 GB/s (8.3k)
1m     | 2.09 GB/s (2.0k)     | 2.23 GB/s (2.1k)     | 4.33 GB/s (4.2k)

硬盘性能在较大块测试中表现突出，适合需要快速读写的大型文件处理任务。

## 网络性能分析

### 基本网络信息

plaintext
IP 地址         : 154.91.202.183
组织            : AS149440 Evoxt Enterprise
地理位置        : 香港 / HK
区域            : 中西区

### SpeedTest.net 测速结果

以下为部分节点的网络测试数据：

plaintext
节点名称            上传速度    下载速度    延迟
Speedtest.net      48.97 Mbps  20.89 Mbps  47.08 ms
TW, Chunghwa       13.41 Mbps  60.00 Mbps  79.34 ms
HK, i3D.net        35.22 Mbps  82.44 Mbps  8.61 ms
SG, i3D.net        17.16 Mbps  83.03 Mbps  39.44 ms

香港 Evoxt VPS 的网络延迟低，尤其在亚太地区表现优异，适合面向亚洲用户的服务部署。

## 流媒体解锁能力

香港 Evoxt VPS 的流媒体解锁测试结果如下：

- **Netflix**：仅支持原创内容
- **YouTube Premium**：支持 (地区: 马来西亚)
- **Amazon Prime Video**：支持 (地区: 香港)
- **Disney+**：不支持
- **HBO GO Asia**：支持 (地区: 香港)

对于流媒体爱好者，香港节点在部分主流平台上具有一定的解锁能力，但支持范围有限。