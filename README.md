# IoT-Refrigerator
An refrigerator with Wechat APP

本项目是2023年嵌入式大赛海思赛道AI计算机视觉选题的作品，使用海思Hi3861V100核心板作为主控板，负责联网、检测温度和温度控制；使用Hi3516主控板负责摄像头识别检测。（你说你没见过这些板子？我的建议是别碰，会变得不幸QAQ）

本项目需要搭配海思开发环境使用，详情请见https://developer.hisilicon.com/postDetail?tid=0206112326723530001下的第二章《开发环境搭建》和第三张《运行第一个程序》。本项目核心内容的温度检测部分由4.5.3, 4.5.4改编而来，如有需要请查看教程内的对应章节，教程里的描述更加清楚。

在使用前请先按照教程4.5.3中的配置小程序的部分申请并配置自己的小程序。本项目白嫖的腾讯云服务器将在不久后到期，请使用自己的服务器。

在配置好海思开发环境后，需要将本目录下的三个demo文件夹copy到/app文件下，参考教程更改iot_config以及iot_main中的配置（wifi、小程序id等），然后用本目录下的BUILD.gn文件替换/app目录下的BUILD，接着rebuild、upload后即可使用。烧录成功后打开monitor，开发板联网、连接服务器需要大约40s左右，使用微信小程序点击照明，若照明成功则连接成功。
![IMG20230719225513](https://github.com/electric-noob/IoT-Refrigerator/assets/123061577/f5966e9b-c2a4-4ae6-892f-691872d674fb)
