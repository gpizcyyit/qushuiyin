# Evoxt 日本东京 VPS 性能测评与流媒体解锁分析

## 测试 IP 与 Looking Glass

Evoxt 日本东京 VPS 的测试 IP 为 `23.27.52.101`，位于日本东京数据中心，为用户提供稳定的网络连接。

## 流媒体解锁能力

Evoxt 日本东京 VPS 在流媒体解锁方面表现出色，以下是 IPv4 和 IPv6 的测试结果：

### IPv4 解锁测试

- **网络信息**: Evoxt Enterprise (23.27.*.*)
- **解锁详情**:
  - **Dazn**: 支持 (地区: 日本)
  - **Disney+**: 支持 (地区: 日本)
  - **Netflix**: 支持 (地区: 日本)
  - **YouTube Premium**: 支持 (地区: 日本)
  - **Amazon Prime Video**: 支持 (地区: 日本)
  - **TVBAnywhere+**: 支持
  - **Spotify 注册**: 支持 (地区: 日本)
  - **Instagram 授权音频**: 不支持
  - **ChatGPT**: 支持
  - **Google Gemini**: 支持 (地区: 日本)
  - **YouTube CDN**: 新加坡
  - **Netflix 优选 CDN**: 香港
  - **Steam 货币**: 日元 (JPY)

### IPv6 解锁测试

- **网络信息**: Evoxt Enterprise (2400:8d60:10:*:*)
- **解锁详情**:
  - **Dazn**: IPv6 当前不支持
  - **Disney+**: IPv6 当前不支持
  - **Netflix**: 支持 (地区: 日本)
  - **YouTube Premium**: 支持 (地区: 日本)
  - **Amazon Prime Video**: IPv6 当前不支持
  - **TVBAnywhere+**: IPv6 当前不支持
  - **Spotify 注册**: 支持 (地区: 马来西亚)
  - **ChatGPT**: 测试失败 (网络连接问题)
  - **Google Gemini**: 支持 (地区: 日本)
  - **YouTube CDN**: 台北
  - **Netflix 优选 CDN**: 香港

通过以上数据可以看出，Evoxt 的 IPv4 解锁能力更全面，尤其适合需要解锁日本地区流媒体的用户，而 IPv6 支持范围相对有限。

👉 [2025年最新Evoxt优惠码和云服务器方案套餐整理汇总](https://bit.ly/evoxt)

## TCP 回程路由测试

以下是 Evoxt 日本东京 VPS 的回程路由测试结果，覆盖多个国内线路：

### 上海 CN2 / 广东东莞 CN2

1   10.1.1.21       RFC1918                  0.24 ms
4   63.216.142.10   中国香港 pccwglobal.com  47.46 ms
7   59.43.22.5      中国上海 chinatelecom.cn  81.51 ms
24  58.32.32.1      中国上海 chinatelecom.cn  79.66 ms

- **特点**: 通过香港中转，延迟较低，适合华东和华南用户。

### 上海电信

1   10.1.1.21       RFC1918                  0.33 ms
7   140.222.5.71    美国加州 chinatelecom.cn 104.12 ms
13  61.152.71.38    中国上海 chinatelecom.cn 306.18 ms

- **特点**: 经美国中转，延迟稍高，适合对电信线路有需求的场景。

### 广州移动

1   10.1.1.21       RFC1918                  0.24 ms
4   63.223.17.90    中国香港 pccwglobal.com  47.82 ms
15  120.196.2.50    中国广东 gd.10086.cn    197.45 ms

- **特点**: 香港中转至广州，移动用户体验良好。

## 网络速度与延迟表现

Evoxt 日本东京 VPS 的网络性能测试结果如下：

Node Name      Upload Speed  Download Speed  Latency
Speedtest.net  689.54 Mbps   788.91 Mbps     97.12 ms
Singapore SG   939.62 Mbps   3754.18 Mbps    72.13 ms
Tokyo JP       1455.55 Mbps  553.35 Mbps     27.70 ms
USA US         686.11 Mbps   2542.21 Mbps    108.81 ms

- **分析**: 东京本地延迟仅 27.70 ms，下载速度高达 553.35 Mbps，适合亚洲地区用户，尤其是日本本地访问。

## YABS 性能测试

以下是 Evoxt VPS 的硬件性能测试结果：

CPU Model: AMD EPYC-Genoa Processor
CPU Cores: 1
Total Disk: 4.9 GB (1.3 GB 已使用)
Total Mem: 457 MB (86 MB 已使用)
I/O Speed: 平均 1536.0 MB/s
OS: Debian GNU/Linux 12

- **亮点**: I/O 速度表现优秀，适合轻量级应用或小型网站托管。

## IPv6 路由建议

由于 IPv6 路由因地区差异较大，建议用户根据实际需求自行测试，以确保最佳性能。

## 总结

Evoxt 日本东京 VPS 在流媒体解锁、网络延迟和性能表现上均有优异表现，尤其是对日本地区的内容访问支持尤为出色。无论是追剧、游戏还是日常使用，这款 VPS 都能满足大部分用户的需求。