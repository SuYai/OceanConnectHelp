## 背景说明

	跟我学LiteOS调测OneLight


## LiteOS调测OneLight

* [1.获取源代码](#1)
* [2.Huawei LiteOS目录介绍](#2)
* [3.开发板硬件连接](#3)
* [4.打开MDK523项目](#4)
* [5.编译工程](#5)
* [6.下载运行](#6)
* [7.LOG打印输出](#7)
* [8.查看OceanConnect平台数据](#8)
* [9.OceanCOnnect下发命令](#9)


<h3 id="1">1.获取源代码</h3>

	华为IoT开发者生态峰会LiteOS_NB-IoT_OceanConnect
	链接：https://pan.baidu.com/s/1bIo0hkfgy_KWQx_Xi_BX3Q 
	密码：lyyh
	【注意】下载源代码，安装MDK523，安装STLINK驱动，安装CH340驱动等。

<h3 id="2">2.Huawei LiteOS目录介绍</h3>

![](./meta/20180522/liteos/SUYAI02337.png)

![](./meta/20180522/liteos/SUYAI02338.png)

![](./meta/20180522/liteos/SUYAI02339.png)

![](./meta/20180522/liteos/SUYAI02340.png)

![](./meta/20180522/liteos/SUYAI02341.png)

<h3 id="3">3.开发板硬件连接</h3>

![](./meta/20180522/liteos/suyai_liteos_board.jpg)

- 【注意】P12短接端子。烧写器的接线方式。

![](./meta/20180522/liteos/SUYAI02343.png)

![](./meta/20180522/liteos/suyai_liteos_board_1.jpg)

<h3 id="4">4.打开MDK523项目</h3>

- 进入targets\STM32L431RxTx_IoTClub\MDK-ARM，打开STM32L431RxTx.uvprojx

![](./meta/20180522/liteos/SUYAI02344.png)

<h3 id="5">5.编译工程</h3>

![](./meta/20180522/liteos/SUYAI02345.png)

<h3 id="6">6.下载运行</h3>

![](./meta/20180522/liteos/SUYAI02345_1.png)

- 【注意】下面的工程设置参数。

![](./meta/20180522/liteos/SUYAI02346.png)
![](./meta/20180522/liteos/SUYAI02347.png)
![](./meta/20180522/liteos/SUYAI02348.png)
![](./meta/20180522/liteos/SUYAI02349.png)
![](./meta/20180522/liteos/SUYAI02350.png)
![](./meta/20180522/liteos/SUYAI02351.png)
![](./meta/20180522/liteos/SUYAI02352.png)
![](./meta/20180522/liteos/SUYAI02353.png)
![](./meta/20180522/liteos/SUYAI02354.png)
![](./meta/20180522/liteos/SUYAI02355.png)
![](./meta/20180522/liteos/SUYAI02356.png)

<h3 id="7">7.LOG打印输出</h3>

- 先登陆OceanConnect平台。

![](./meta/20180522/liteos/SUYAI02357.png)

- 【注意】此时串口调试助手，已经打印输出AT指令发送OK的信息。查看OC平台。

![](./meta/20180522/liteos/SUYAI02360.png)

<h3 id="8">8.查看OceanConnect平台数据</h3>

![](./meta/20180522/liteos/SUYAI02360_1.png)
![](./meta/20180522/liteos/SUYAI02361.png)

<h3 id="9">9.OceanCOnnect下发命令</h3>

![](./meta/20180522/liteos/SUYAI02362.png)
![](./meta/20180522/liteos/SUYAI02363.png)
![](./meta/20180522/liteos/SUYAI02364.png)
![](./meta/20180522/liteos/SUYAI02365.png)
![](./meta/20180522/liteos/SUYAI02366.png)

- 至此，完成LiteOS调测OneLight。

附：
此次LiteOS提供的4合1 Demo，其中包括 OneButton, OneSmoke, OneGPS, OneLight。
可以根据下面的宏定义，选择合适的传感器，即可完成Demo的调测。

![](./meta/20180522/liteos/SUYAI02368.png)



