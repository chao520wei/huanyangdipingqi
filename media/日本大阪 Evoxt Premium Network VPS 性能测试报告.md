# 日本大阪 Evoxt Premium Network VPS 性能测试报告

## 购买信息

本次测试的 VPS 配置如下：

- **规格**: 1 vCore / 512MB 内存 / 5GB 存储 / 250GB 月流量
- **价格**: 每月仅需 2.99 美元
- **优惠码**: AFF160-jam114514

这款配置性价比极高，适合预算有限但对性能有一定要求的用户。购买详情可参考官方渠道。

## 性能评价

Evoxt 近期对其设备进行了升级，采用了 AMD EPYC Genoa 处理器，性能表现令人满意。网络方面，上游依然接入 xTom，回程线路为软银（SoftBank）。从测试结果来看，网络稳定性与速度均表现优秀，尤其适合需要日本本地化服务的场景。

## 测试数据详解

以下是针对 Evoxt 日本大阪 Premium Network VPS 的详细测试数据，涵盖系统信息、硬件性能、网络速度等多个维度。

### 系统信息

plaintext
CPU 型号: AMD EPYC-Genoa 处理器
CPU 缓存: L1: 32.00 KB / L2: 1.00 MB / L3: 32.00 MB
CPU 规格: 1 vCPU
虚拟化类型: KVM
内存使用: 79.59 MiB / 460.47 MiB
磁盘使用: 2.03 GiB / 4.83 GiB
操作系统: Debian GNU/Linux 12 (bookworm) (x86_64)
内核版本: 6.12.13-x64v3-xanmod1
IPv4 地址: [JP] 166.88.2.64 (AS149440 - Evoxt Enterprise, 日本大阪)
IPv6 地址: [JP] 2400:8d60:8::6c2:2cb (AS149440 - Evoxt Enterprise, 日本大阪)

### 硬件性能

plaintext
CPU 单线程测试: 5495.74 分
磁盘性能 (4K 块):
  写速度: 235.85 MB/s (60377 IOPS)
  读速度: 362.32 MB/s (92753 IOPS)
磁盘性能 (128K 块):
  写速度: 3225.81 MB/s (25806 IOPS)
  读速度: 5263.16 MB/s (42105 IOPS)

硬件测试显示，Genoa 处理器赋予了 VPS 出色的计算能力，而磁盘读写速度也足以应对日常应用需求。

👉 [2025年最新Evoxt优惠码和云服务器方案套餐整理汇总](https://bit.ly/evoxt)

### 网络速度测试 (Speedtest)

- **大阪本地 (xTom)**:
  - 下载: 810.23 Mbps
  - 上传: 498.25 Mbps
  - 延迟: 16.23 ms
  - 丢包率: 9.6%

- **中国移动福建**:
  - 下载: 406.72 Mbps
  - 上传: 7.51 Mbps
  - 延迟: 198.03 ms

- **中国联通上海 5G**:
  - 下载: 576.12 Mbps
  - 上传: 700.94 Mbps
  - 延迟: 57.35 ms
  - 丢包率: 19.3%

- **中国电信江苏 5G**:
  - 下载: 544.25 Mbps
  - 上传: 807.31 Mbps
  - 延迟: 38.22 ms

从结果来看，大阪本地网络表现出色，而对中国大陆的连接速度和延迟表现也较为稳定，尤其是电信和联通线路。

### iperf3 网络测试

- **IPv4**:
  - Leaseweb (新加坡): 发送 753 Mbps / 接收 503 Mbps / 延迟 179 ms
  - Clouvider (洛杉矶): 发送 657 Mbps / 接收 213 Mbps / 延迟 106 ms

- **IPv6**:
  - Leaseweb (纽约): 发送 591 Mbps / 接收 585 Mbps / 延迟 153 ms
  - Clouvider (伦敦): 发送 316 Mbps / 接收 194 Mbps / 延迟 221 ms

IPv4 和 IPv6 的全球连接性能均衡，适合跨区域使用。

### 流媒体解锁情况

- **IPv4**:
  - Netflix: 支持 (日本区)
  - Disney+: 支持 (日本区)
  - YouTube Premium: 支持 (日本区)
  - Amazon Prime Video: 支持 (日本区)

- **IPv6**:
  - Netflix: 支持 (日本区)
  - YouTube Premium: 支持 (日本区)
  - 部分服务暂不支持 IPv6

流媒体测试表明，该 VPS 可有效解锁日本本地内容，满足影音娱乐需求。

### 路由追踪 (Traceroute)

- **中国电信 (上海)**:
  - 延迟: 147.94 ms (22 跳)
  - 路径: SoftBank → 中国电信上海

- **中国联通 (上海)**:
  - 延迟: 59.49 ms (21 跳)
  - 路径: SoftBank → 中国联通上海

- **中国移动 (上海)**:
  - 延迟: 70.90 ms (19 跳)
  - 路径: SoftBank → 中国移动上海

路由测试显示，软银回程线路优化良好，连接中国大陆的延迟和稳定性表现不错。