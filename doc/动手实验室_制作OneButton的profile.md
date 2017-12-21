## 背景说明

	快速开发OneButton的profile。

## 开发步骤

* [1.制作profile](#1)
* [2.button服务](#2)
* [3.Temp服务](#3)
* [4.Beep服务](#4)
* [5.Network服务](#5)
* [6.Alarm服务](#6)
* [7.完成制作profile](#7)
* [8.导入profile](#8)

<h3 id="1">1.制作profile</h3>

- 点击左侧导航栏。Profile开发 -> 产品。

![](./meta/20171117/SUYAI00012.png)

- 可以自定义产品，也可以直接导入Profile文件。点击“自定义产品”。

![](./meta/20171117/SUYAI00013.png)

- 点击“创建全新产品”。

- 创建全新产品。设备类型，选 other，填入 OneButton（注意：关于产品类型、型号，大家也可以按照自己的想法来填写，此处仅仅是示范）。

- 【注意】创建全新产品时，请以参赛序号为后缀。如：IOTBTN00。如果你是3组，那么命名为IOTBTN03。以此类推。

![](./meta/20171221/SUYAI00498.png)
![](./meta/20171221/SUYAI00500.png)

- 点击确定后，添加产品成功！

![](./meta/20171117/SUYAI00016.png)

- 在我的产品中，有新添加的产品。点击此产品。

![](./meta/20171221/SUYAI00501.png)

- 右下角点击“新建服务”。服务是描述了产品是什么、能做什么以及如何控制该产品的信息。
- 点击链接 [设备profile文件](http://developer.huawei.com/ict/cn/site-oceanconnect_doc?doc=oceanconnect_dev_overview_portal%2Fzh-cn_topic_0073931585) 查看更详细介绍。

![](./meta/20171221/SUYAI00502.png)

- 咱们给OneButton规划一些功能，然后把这些功能列表转换为profile属性列表，如下图。

![](./meta/20171221/SUYAI00503.png)

<h3 id="2">2.button服务</h3>

- 服务名：Button。点击“新增属性”。属性是对这项服务进行详细参数定义。

![](./meta/20171221/SUYAI00504.png)
![](./meta/20171221/SUYAI00505.png)
![](./meta/20171221/SUYAI00506.png)

- 目前已经完成button服务的创建。button拥有一个属性buttonState，它的具体值，可以指明当前按钮的状态。创建效果如下：

![](./meta/20171221/SUYAI00507.png)
![](./meta/20171221/SUYAI00508.png)

- 右上角点击“新建服务”，开始创建Temp服务。

![](./meta/20171221/SUYAI00509.png)

<h3 id="3">3.Temp服务</h3>

- 创建Temp服务。Temp拥有一个属性tempValue，它的具体值，指示当前的环境温度。

![](./meta/20171221/SUYAI00510.png)
![](./meta/20171221/SUYAI00511.png)
![](./meta/20171221/SUYAI00512.png)
![](./meta/20171221/SUYAI00513.png)

<h3 id="4">4.Beep服务</h3>

- 创建Beep服务。Beep拥有一个属性beepState，它的具体值，指示当前蜂鸣器状态。

- Beep拥有一个命令：SET_BEEP_ON。命令字段为：beepOnValue。这样可以通过IoT云平台给OneButton下发控制命令。


![](./meta/20171221/SUYAI00514.png)
![](./meta/20171221/SUYAI00515.png)
![](./meta/20171221/SUYAI00516.png)
![](./meta/20171221/SUYAI00517.png)
![](./meta/20171221/SUYAI00518.png)
![](./meta/20171221/SUYAI00519.png)
![](./meta/20171221/SUYAI00520.png)
![](./meta/20171221/SUYAI00521.png)
![](./meta/20171221/SUYAI00522.png)


<h3 id="5">5.Network服务</h3>

- 创建Network服务。Network拥有3个属性CSQ、SNR、CELLID。都是指明NB-IoT网络状态。

![](./meta/20171221/SUYAI00523.png)
![](./meta/20171221/SUYAI00524.png)
![](./meta/20171221/SUYAI00525.png)
![](./meta/20171221/SUYAI00526.png)
![](./meta/20171221/SUYAI00527.png)
![](./meta/20171221/SUYAI00528.png)
![](./meta/20171221/SUYAI00529.png)
![](./meta/20171221/SUYAI00530.png)
![](./meta/20171221/SUYAI00531.png)
![](./meta/20171221/SUYAI00532.png)
![](./meta/20171221/SUYAI00533.png)


<h3 id="6">6.Alarm服务</h3>

- 创建Alarm服务。Alarm拥有2个属性highTempAlarm、lowTempAlarm。都是指明当前是否有高温报警（火警）、低温报警。

- Alarm有2个命令。SET_HIGHTEMP_TH。命令字段为：highTempTH。这样可以通过IoT云平台给OneButton设置 高温报警阈值。SET_LOWTEMP_TH。命令字段为：lowTempTH。这样可以通过IoT云平台给OneButton设置 低温报警阈值。

![](./meta/20171221/SUYAI00534.png)
![](./meta/20171221/SUYAI00535.png)
![](./meta/20171221/SUYAI00536.png)
![](./meta/20171221/SUYAI00537.png)
![](./meta/20171221/SUYAI00538.png)
![](./meta/20171221/SUYAI00539.png)
![](./meta/20171221/SUYAI00540.png)
![](./meta/20171221/SUYAI00541.png)
![](./meta/20171221/SUYAI00542.png)
![](./meta/20171221/SUYAI00543.png)
![](./meta/20171221/SUYAI00544.png)
![](./meta/20171221/SUYAI00545.png)
![](./meta/20171221/SUYAI00546.png)
![](./meta/20171221/SUYAI00547.png)
![](./meta/20171221/SUYAI00548.png)
![](./meta/20171221/SUYAI00549.png)
![](./meta/20171221/SUYAI00550.png)


<h3 id="7">7.完成制作profile</h3>

- OneButton的profile制作完了，下面是总览图，大家可以对比一下设置内容。

![](./meta/20171221/SUYAI00551.png)

<h3 id="8">8.导入profile</h3>

- 左侧导航栏，点击“导入Profile”。

![](./meta/20171117/SUYAI00030.png)

- Profile文件下载链接： 【此处不在提供下载，请大家动手完成所有开发】 下载后，点击导入。

![](./meta/20171221/SUYAI00552.png)
![](./meta/20171221/SUYAI00553.png)
![](./meta/20171221/SUYAI00554.png)
