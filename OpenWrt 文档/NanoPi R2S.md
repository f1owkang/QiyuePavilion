# NanoPi R2S新版介绍

- NanoPi R2S（以下简称R2S）是友善电子团队最新推出的一款实现满速率双千兆的、完全开源的开发板。
- NanoPi R2S 使用RK3328 CPU，有两个千兆网络，1G DDR4内存，友善电子团队为NanoPi R2S专门移植了OpenWrt系统，支持Docker CE, 完全开源，用于企业物联网二次开发，个人定制NAS等。

# NanoPi R2S资源特性

- CPU: Rockchip RK3328, Quad-core Cortex-A53
- DDR4 RAM: 1GB
- Network：
- 10/100/1000M以太网口 x 1
- USB3.0转10/100/1000M以太网口 x 1
- USB2.0 Host: Type-A x1
- MicroSD Slot x 1
- Type-C USB: 供电和Slave功能
- Debug Serial Port: 3.3V TTL电平，3Pin 2.54mm间距排针
- LED: LED x 3
- KEY: KEY x 1 用户自定义功能
- PC Size: 55.6 x 52mm
- Power Supply: DC 5V/3A
- Temperature measuring range: 0℃ to 80℃
- OS/Software: U-boot，Ubuntu-Core，OpenWrt
- 实测网络速率

|  | TX | RX |
|:---:|:---:|:---:|
| WAN | 941 Mbps | 941 Mbps |
| LAN | 941 Mbps | 941 Mbps |
| Notes： | 1、测试工具：iperf（官方数据） | 2、使用独立IP地址段和PC机单向通讯测试 |

# 接口布局和尺寸

|Pin# | Name | Linux gpio |
|:-:|:---:|:---:|
| 1	| SYS_3.3V |  |
| 2 | VDD_5V |  |
| 3	| I2C0_SDA / GPIO2_D1 |	89 |
| 4	| VDD_5V |  |
| 5	| I2C0_SCL / GPIO2_D0 |	88 |
| 6	| GND |  |
| 7	| GPIO2_A2 / IR_RX | 66 |
| 8	| UART1_TX / GPIO3_A4 | 100 |
| 9 | GND |  |
| 10 | UART1_RX / GPIOG3_A6 | 102|