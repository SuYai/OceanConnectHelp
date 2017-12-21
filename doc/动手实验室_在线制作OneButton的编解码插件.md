## 背景说明

	在线生成编解码插件。

- 点击链接 [编解码库开发与升级指南](http://developer.huawei.com/ict/cn/site-oceanconnect_doc?doc=oceanconnect_utility_portal%2Fzh-cn_topic_0072974881)  详细了解编解码插件。

## 开发步骤

* [1.BTN_DATA_RPT 消息上报](#1)
* [2.EXT_DATA_RPT 消息上报](#2)
* [3.ALARM_RPT 消息上报](#3)
* [4.SET_HIGHTEMP_TH 命令下发](#4)
* [5.SET_LOWTEMP_TH 命令下发](#5)
* [6.SET_BEEP_ON 命令下发](#6)
* [7.保存、部署编解码插件](#7)

- 点击插件开发。点击开始设计。

![](./meta/20171117/SUYAI00035.png)

- 点击新建插件。下面有一些插件的模版，大家可以点进去查看参考，也可以基于模版直接进行开发。

![](./meta/20171117/SUYAI00036.png)

- 选择profile文件。

![](./meta/20171221/SUYAI00555.png)

![](./meta/20171221/SUYAI00644.png)

<h3 id="1">1.BTN_DATA_RPT 消息上报</h3>

- 新建一个数据上报信息BTN_DATA_RPT。就是上报环境温度	Button状态，Temp温度，Beep状态

![](./meta/20171221/SUYAI00556.png)
![](./meta/20171221/SUYAI00557.png)

- 此时可以保存一下，制作编解码插件时，也要注意保存。

![](./meta/20171221/SUYAI00561.png)
![](./meta/20171221/SUYAI00562.png)
![](./meta/20171221/SUYAI00563.png)

- 此处开始增加BTN_DATA_RPT的编解码字段。共4个字段。messageId，buttonState，tempValue，beepState。


![](./meta/20171221/SUYAI00564.png)
![](./meta/20171221/SUYAI00565.png)
![](./meta/20171221/SUYAI00566.png)
![](./meta/20171221/SUYAI00567.png)
![](./meta/20171221/SUYAI00568.png)
![](./meta/20171221/SUYAI00569.png)
![](./meta/20171221/SUYAI00570.png)
![](./meta/20171221/SUYAI00571.png)
![](./meta/20171221/SUYAI00572.png)



- 此处开始把编解码字段，与profile字段进行对应。使用拖拉的方法。

![](./meta/20171221/SUYAI00573.png)
![](./meta/20171221/SUYAI00574.png)
![](./meta/20171221/SUYAI00575.png)
![](./meta/20171221/SUYAI00576.png)

<h3 id="2">2.EXT_DATA_RPT 消息上报</h3>

- 新建一个数据上报信息EXT_DATA_RPT。就是上报网络质量	CSQ、SNR、CELLID。

- 【注意】SNR是2字节。CELLID是4字节。

![](./meta/20171221/SUYAI00579.png)
![](./meta/20171221/SUYAI00580.png)
![](./meta/20171221/SUYAI00581.png)
![](./meta/20171221/SUYAI00582.png)
![](./meta/20171221/SUYAI00583.png)
![](./meta/20171221/SUYAI00585.png)
![](./meta/20171221/SUYAI00586.png)
![](./meta/20171221/SUYAI00587.png)
![](./meta/20171221/SUYAI00588.png)
![](./meta/20171221/SUYAI00589.png)
![](./meta/20171221/SUYAI00590.png)


<h3 id="3">3.ALARM_RPT 消息上报</h3>

- 新建一个数据上报信息ALARM_RPT。就是上报火灾报警（高温报警），低温报警	。

![](./meta/20171221/SUYAI00591.png)
![](./meta/20171221/SUYAI00592.png)
![](./meta/20171221/SUYAI00593.png)
![](./meta/20171221/SUYAI00594.png)
![](./meta/20171221/SUYAI00595.png)
![](./meta/20171221/SUYAI00596.png)
![](./meta/20171221/SUYAI00597.png)
![](./meta/20171221/SUYAI00598.png)
![](./meta/20171221/SUYAI00599.png)

<h3 id="4">4.SET_HIGHTEMP_TH 命令下发</h3>

- 新建一个命令下发信息SET_HIGHTEMP_TH。平台控制OneButton的高温报警阈值。

![](./meta/20171221/SUYAI00600.png)
![](./meta/20171221/SUYAI00601.png)
![](./meta/20171221/SUYAI00602.png)
![](./meta/20171221/SUYAI00603.png)
![](./meta/20171221/SUYAI00604.png)
![](./meta/20171221/SUYAI00605.png)
![](./meta/20171221/SUYAI00606.png)


<h3 id="5">5.SET_LOWTEMP_TH 命令下发</h3>

- 新建一个命令下发信息SET_LOWTEMP_TH 。平台控制OneButton的低温报警阈值。


![](./meta/20171221/SUYAI00607.png)
![](./meta/20171221/SUYAI00608.png)
![](./meta/20171221/SUYAI00609.png)
![](./meta/20171221/SUYAI00610.png)
![](./meta/20171221/SUYAI00611.png)
![](./meta/20171221/SUYAI00612.png)
![](./meta/20171221/SUYAI00613.png)

<h3 id="6">6.SET_BEEP_ON 命令下发</h3>

- 新建一个命令下发信息SSET_BEEP_ON 。平台控制OneButton的寻物响铃，间隔响状态。

![](./meta/20171221/SUYAI00614.png)
![](./meta/20171221/SUYAI00615.png)
![](./meta/20171221/SUYAI00616.png)
![](./meta/20171221/SUYAI00617.png)
![](./meta/20171221/SUYAI00618.png)
![](./meta/20171221/SUYAI00619.png)
![](./meta/20171221/SUYAI00620.png)

<h3 id="7">7.保存、部署编解码插件</h3>

![](./meta/20171221/SUYAI00621.png)
![](./meta/20171221/SUYAI00622.png)
![](./meta/20171221/SUYAI00623.png)
![](./meta/20171221/SUYAI00624.png)





