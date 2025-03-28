# ColoCrossing 纽约美东黑五特惠VPS全面评测

作为老牌IDC服务商，ColoCrossing近年来开始拓展零售业务。其纽约机房提供无限流量方案，但需注意邻居滥用可能影响性能。

## 服务器配置详情

初始分配的服务器存在Debian系统兼容性问题且速度缓慢，经客服更换后性能显著改善：

bash
Uptime     : 5 days, 5 hours, 41 minutes
Processor  : Intel(R) Xeon(R) CPU E5-2683 v4 @ 2.10GHz
CPU cores  : 2 @ 2099.996 MHz
AES-NI     : ✔ Enabled
VM-x/AMD-V : ✔ Enabled
RAM        : 1.9 GiB
Swap       : 2.5 GiB
Disk       : 36.8 GiB
Distro     : Debian GNU/Linux 11 (bullseye)
Kernel     : 5.10.0-23-amd64
VM Type    : KVM
IPv4/IPv6  : ✔ Online / ❌ Offline

> 注：该机型未配备IPv6，且处理器性能中等。论坛反馈显示部分用户分配到了至强金牌处理器。

👉 [【点击查看】2025年最新 ColoCrossing 优惠码及特价云服务器方案汇总](https://bit.ly/ColoCrossing)

## 存储性能测试

通过fio工具进行混合读写测试，结果如下：

bash
fio Disk Speed Tests (Mixed R/W 50/50) (Partition /dev/vda1):
---------------------------------
Block Size | 4k            (IOPS) | 64k           (IOPS)
  ------   | ---            ----  | ----           ---- 
Read       | 2.63 MB/s      (658) | 39.05 MB/s     (610)
Write      | 2.64 MB/s      (661) | 39.32 MB/s     (614)
Total      | 5.28 MB/s     (1.3k) | 78.38 MB/s    (1.2k)
           |                      |                     
Block Size | 512k          (IOPS) | 1m            (IOPS)
  ------   | ---            ----  | ----           ---- 
Read       | 184.85 MB/s    (361) | 251.18 MB/s    (245)
Write      | 194.68 MB/s    (380) | 267.91 MB/s    (261)
Total      | 379.54 MB/s    (741) | 519.09 MB/s    (506)

## 全球网络性能测试

### 国际节点测速

bash
iperf3 Network Speed Tests (IPv4):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping           
-----           | -----                     | ----            | ----            | ----           
Clouvider       | London, UK (10G)          | 672 Mbits/sec   | 183 Mbits/sec   | 80.1 ms        
Scaleway        | Paris, FR (10G)           | 653 Mbits/sec   | 322 Mbits/sec   | 89.1 ms        
NovoServe       | North Holland, NL (40G)   | 467 Mbits/sec   | 493 Mbits/sec   | 93.6 ms        
Uztelecom       | Tashkent, UZ (10G)        | 349 Mbits/sec   | 174 Mbits/sec   | 180 ms         
Clouvider       | NYC, NY, US (10G)         | 949 Mbits/sec   | busy            | 9.93 ms        
Clouvider       | Dallas, TX, US (10G)      | 303 Mbits/sec   | 67.0 Mbits/sec  | 154 ms         
Clouvider       | Los Angeles, CA, US (10G) | 569 Mbits/sec   | 116 Mbits/sec   | 71.4 ms

### 中国大陆连接测试
（测试数据待补充）