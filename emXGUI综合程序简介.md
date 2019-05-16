emxGUI综合程序简介
------------------
emXGUI视频演示：<https://www.bilibili.com/video/av51804501>
## 

野火提供的emXGUI综合示例程序，是基于emXGUI图形软件库及RT-Thread/FreeRTOS操作系统制作的人机交互界面程序。该程序界面酷炫，性能卓越，非常适合作为嵌入式人机交互界面的参考示例，目前该程序已适配表格
1‑1中的野火系列开发板。

表格 1‑1 emXGUI综合示例程序适配的开发板

| 开发板                | 适配情况 | 图形库 | 操作系统                        |
|-----------------------|----------|--------|---------------------------------|
| F429_挑战者开发板_V1  | 已适配   | emXGUI | RT-Thread，后续会移植至FreeRTOS |
| F429_挑战者开发板_V2  | 已适配   | emXGUI | RT-Thread，后续会移植至FreeRTOS |
| H743_Pro开发板        | 已适配   | emXGUI | FreeRTOS                        |
| H750_Pro开发板        | 已适配   | emXGUI | FreeRTOS                        |
| i.MX RT1052系列开发板 | 正在开发 | emXGUI | FreeRTOS                        |

示例应用说明
------------

### 开机界面

emXGUI综合程序正式运行时，它在上电后会从板子上的SPI-FLASH中加载各种所需的资源文件到SDRAM，加速后续的运行，该过程在不同的开发板加载的时间不同，F429开发板大约为3秒，H743/750加载时间在0.5秒内。

![启动界面1](https://raw.githubusercontent.com/wiki/Embdefire/emXGUI/images/emXGUI综合程序/启动界面1.jpg)

![启动界面2](https://raw.githubusercontent.com/wiki/Embdefire/emXGUI/images/emXGUI综合程序/启动界面2.jpg)

![启动界面3](https://raw.githubusercontent.com/wiki/Embdefire/emXGUI/images/emXGUI综合程序/启动界面3.jpg)

### APP应用列表界面

资源加载完成后，会进入APP应用列表界面，它包含GUI基础应用、MP3播放器、视频播放器、RGB彩灯、摄像头、图片浏览器等应用，更多的应用在持续开发中。

![应用列表界面1](https://raw.githubusercontent.com/wiki/Embdefire/emXGUI/images/emXGUI综合程序/应用列表界面1.jpg)

通过滑动或点击APP应用列表界面的左右箭头可以切换至不同的APP列表界面。

![应用列表界面2](https://raw.githubusercontent.com/wiki/Embdefire/emXGUI/images/emXGUI综合程序/应用列表界面2.jpg)

### emXGUI介绍界面

点击APP应用列表界面的下方，会弹出emXGUI的介绍。

![emXGUI介绍界面](https://raw.githubusercontent.com/wiki/Embdefire/emXGUI/images/emXGUI综合程序/emXGUI介绍界面.jpg)

### GUI应用界面

点击GUI应用，可进入另一种形式的APP列表界面，该界面下的APP主要包含了独立于硬件的GUI示例，如图形加速器、虚拟示波器、仪表盘等应用。

![emXGUI应用界面1](https://raw.githubusercontent.com/wiki/Embdefire/emXGUI/images/emXGUI综合程序/emXGUI应用界面1.jpg)

![emXGUI应用界面2](https://raw.githubusercontent.com/wiki/Embdefire/emXGUI/images/emXGUI综合程序/emXGUI应用界面2.jpg)

### 智能家居示例界面

RGB彩灯应用包含了智能家居示例界面，通过滑动屏幕上的控制栏，可以控制开发板中的RGB彩灯呈现不同的颜色，模拟智能家居中的台灯调光系统。

![智能家居示例界面1](https://raw.githubusercontent.com/wiki/Embdefire/emXGUI/images/emXGUI综合程序/智能家居示例界面1.jpg)

![智能家居示例界面2](https://raw.githubusercontent.com/wiki/Embdefire/emXGUI/images/emXGUI综合程序/智能家居示例界面2.jpg)

### MP3播放器界面

MP3播放器应用支持播放SD卡中的MP3、WAV文件，该应用包含有实时歌词显示、音乐列表、音量进度的播放控制等功能。

![MP3播放界面1](https://raw.githubusercontent.com/wiki/Embdefire/emXGUI/images/emXGUI综合程序/MP3播放界面1.jpg)

![MP3播放界面2](https://raw.githubusercontent.com/wiki/Embdefire/emXGUI/images/emXGUI综合程序/MP3播放界面2.jpg)

![MP3播放界面3](https://raw.githubusercontent.com/wiki/Embdefire/emXGUI/images/emXGUI综合程序/MP3播放界面3.jpg)

![MP3播放界面4](https://raw.githubusercontent.com/wiki/Embdefire/emXGUI/images/emXGUI综合程序/MP3播放界面4.jpg)

### 视频播放器界面

视频播放器应用支持播放SD卡中特定格式的AVI文件，不同的开发板支持的视频分辨率及播放帧率不同，应用中包含视频列表、音量和进度控制等功能。

![视频播放界面1](https://raw.githubusercontent.com/wiki/Embdefire/emXGUI/images/emXGUI综合程序/视频播放界面1.jpg)

![视频播放界面2](https://raw.githubusercontent.com/wiki/Embdefire/emXGUI/images/emXGUI综合程序/视频播放界面2.jpg)

![视频播放界面3](https://raw.githubusercontent.com/wiki/Embdefire/emXGUI/images/emXGUI综合程序/视频播放界面3.jpg)

![视频播放界面4](https://raw.githubusercontent.com/wiki/Embdefire/emXGUI/images/emXGUI综合程序/视频播放界面4.jpg)

![视频播放界面5](https://raw.githubusercontent.com/wiki/Embdefire/emXGUI/images/emXGUI综合程序/视频播放界面5.jpg)

### 图片浏览器界面

图片浏览器应用支持显示SPI-FLASH、SD卡中的图片文件，支持的图片类型包括BMP、JPEG、PNG以及GIF格式。

![图片浏览器界面1](https://raw.githubusercontent.com/wiki/Embdefire/emXGUI/images/emXGUI综合程序/图片浏览器界面1.jpg)

![图片浏览器界面2](https://raw.githubusercontent.com/wiki/Embdefire/emXGUI/images/emXGUI综合程序/图片浏览器界面2.jpg)

![图片浏览器界面3](https://raw.githubusercontent.com/wiki/Embdefire/emXGUI/images/emXGUI综合程序/图片浏览器界面3.jpg)

![图片浏览器界面4](https://raw.githubusercontent.com/wiki/Embdefire/emXGUI/images/emXGUI综合程序/图片浏览器界面4.jpg)

![图片浏览器界面5](https://raw.githubusercontent.com/wiki/Embdefire/emXGUI/images/emXGUI综合程序/图片浏览器界面5.jpg)

![图片浏览器界面6](https://raw.githubusercontent.com/wiki/Embdefire/emXGUI/images/emXGUI综合程序/图片浏览器界面6.jpg)

![图片浏览器界面7](https://raw.githubusercontent.com/wiki/Embdefire/emXGUI/images/emXGUI综合程序/图片浏览器界面7.jpg)

![图片浏览器界面8](https://raw.githubusercontent.com/wiki/Embdefire/emXGUI/images/emXGUI综合程序/图片浏览器界面8.jpg)

### 图形加速器示例

图形加速器示例包含有显示文字、图片以及纯色矩形等内容，它可用于对比不同开发板的性能，根据不同的主控芯片，还可以控制是否使用专用的图形加速器功能。

![图形加速器界面1](https://raw.githubusercontent.com/wiki/Embdefire/emXGUI/images/emXGUI综合程序/图形加速器界面1.jpg)

### 波形显示示例

波形显示示例非常适合用于展示数据采集、示波器等应用，本示例中虚拟出一些波形数据，显示在界面上，该应用包含不同的波形数据、不同的量程和时间单位变换时的数据展示。

![波形显示界面1](https://raw.githubusercontent.com/wiki/Embdefire/emXGUI/images/emXGUI综合程序/波形显示界面1.jpg)

![波形显示界面2](https://raw.githubusercontent.com/wiki/Embdefire/emXGUI/images/emXGUI综合程序/波形显示界面2.jpg)

![波形显示界面3](https://raw.githubusercontent.com/wiki/Embdefire/emXGUI/images/emXGUI综合程序/波形显示界面3.jpg)

![波形显示界面4](https://raw.githubusercontent.com/wiki/Embdefire/emXGUI/images/emXGUI综合程序/波形显示界面4.jpg)

### 刷FLASH资源界面

当emXGUI更新SPI-FLASH资源时，会显示刷FLASH资源界面，它可以把emXGUI运行时需要的内容从SD卡拷贝到板子上的SPI-FLASH。

![刷FLASH资源界面1](https://raw.githubusercontent.com/wiki/Embdefire/emXGUI/images/emXGUI综合程序/刷FLASH资源界面1.jpg)

如何运行emXGUI综合程序
----------------------

野火emXGUI综合程序提供开源代码，用户可编译并下载该程序到开发板上运行。

### 所需要的环境

#### 硬件环境

emXGUI综合程序所需要的硬件运行环境如下：

-   配套的野火开发板，目前支持如下开发板：

1.  野火STM32F429_挑战者开发板_V1

2.  野火STM32F429_挑战者开发板_V2

3.  野火STM32H743_Pro开发板

4.  野火STM32H750_Pro开发板

-   5寸液晶屏

-   DAP下载器

-   SD卡及读卡器

-   OV5640摄像头（可选）

-   耳机（可选）

#### 软件环境

emXGUI综合程序所需要的电脑软件环境主要包括编译器和USB转串口驱动，关于这些具体参考野火的《STM32库开发实战指南》相关的教程，建议先通过该教程掌握STM32开发再进行实验。

-   Keil（5.23版本以上即可），用于编译和下载程序

-   USB CH340转串口驱动，用于接收开发板的串口输出

-   串口调试助手，用于查看程序输出，了解程序运行情况

### emXGUI综合程序资料

找到野火提供的emXGUI综合程序资料，资料中主要包含有各配套开发板的“emXGUI综合示例程序”源代码和“sd卡资源文件”。

### 准备SD卡资源文件

emXGUI示例程序运行需要SD卡资源文件，实验前需要准备一张SD卡，并使用读卡器在电脑上把它格式化成FAT32或FAT格式，然后把emXGUI综合程序资料中的“sd卡资源”下的所有内容拷贝至SD卡的根目录，参考下图，图中的资源内容可能会变动，根据资料里提供的内容全部拷贝至SD卡即可。


![拷贝sd资源到SD卡根目录](https://raw.githubusercontent.com/wiki/Embdefire/emXGUI/images/emXGUI综合程序/拷贝sd资源到SD卡根目录.jpg)


把拷贝好资源的SD卡插入到配套开发板的SD卡槽。

### 准备开发板

请按如下步骤准备开发板：

-   给开发板插入包含“sd资源”的SD卡

-   给开发板接上配套的5寸屏幕

-   使用USB线连接开发板的USB转串口接口，另一端连接至电脑

-   使用DAP下载器连接开发板，另一端连接至电脑

-   打开开发板的电源开关

-   若需要听MP3或视频的声音需要接入耳机

-   若需要使用摄像头应用需要接入野火OV5640摄像头

### 编译并下载程序

找到资料里配套自己开发板的程序，编译并使用DAP下载器把程序下载到开发板即可，由于emXGUI综合程序非常复杂，且在持续开发中，所以程序编译后可能会提示很多“Warning”，只要编译后没有提示“Error”，忽略即可。

### 第一次运行

emXGUI综合程序在第一次运行时，会要求从SD卡中拷贝各种资源文件，类似界面如下图。

![刷FLASH资源界面1](https://raw.githubusercontent.com/wiki/Embdefire/emXGUI/images/emXGUI综合程序/刷FLASH资源界面1.jpg)


根据其提示，点击“Click me to load
resources”按钮，等待烧录完成即可，烧录完成后可点击界面的复位按钮或开发板的复位按键复位开发板。

若烧录正常，复位后即可看到程序正式运行时的开机界面和APP应用界面。若出现错误，可使用串口调试助手查看开发板返回的运行日志，串口使用的波特率为115200。
