---
title: Unity 上传程序帮助
description: 随时了解 AltspaceVR Unity 上传程序的最新常见问题和解决方案。
ms.date: 02/10/2021
ms.topic: article
keywords: 帮助、常见问题解答
ms.openlocfilehash: cb983ba4e23186f7cc62043f75e7ea1b2969e92b6bd30b132f1733b5e25e92dd
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/11/2021
ms.locfileid: "119125678"
---
# <a name="unity-uploader-help"></a>Unity 上传程序帮助

**1.此工具有多出色？**

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/cheyenne-mountain-gate-room-v1/player]

这是我的 Stargate Unity 场景，其 SDK 应用支持入口和 DND

**2.我是视频学习者，我的视频在哪里？**

[查看我们的视频](https://youtu.be/km9CnVYPzoM)

**3.在哪里可以找到示例？**

[特色世界](https://account.altvr.com/worlds/featured) 和 [Jimmy 的示例](https://account.altvr.com/worlds/1046572460192825569) 是一个不错的起点

**4.这能与工具包和新 SDK 一起使用吗？**
是的，如果需要，可以一起使用所有工具。 我们正在努力开发它们，以无缝协同工作。

**5.它是否支持粒子效果？**

![雪花粒子效果的 GIF](images/uploader-faq-img-01.gif)

**6.能否获取空间化音频？**
目前不会，但可以将音频源放在本地化区域播放。 

**7.烘焙照明是否正常工作？**
是，但灯必须设置为"烘焙"，而不是"混合"

**8.全局照明是否正常工作？**
是

**9.是否始终必须重置世界？**
正确。 我们必须每次重新加载 Unity 资产捆绑包。 

**10.我可以使用自己的自定义材料与着色器吗？**

![自定义材料与着色器 GIF](images/uploader-faq-img-02.gif)

**11.能否仅上传到一个平台？**
是，使用上传程序工具。 但是，在 Android 上的人在上传其平台的场景之前，不会在你的世界看到任何内容。 

**12.是否允许脚本？**
否，出于安全原因，我们不允许脚本或脚本引用。 如果上传内容包含脚本或脚本引用，将被拒绝。 如果需要编写脚本，请看一看新 SDK。 

**13.可以上传多少场景？**
我们建议你从小开始，注意 Altspace 中没有小电脑的人。 也就是说，我们让游戏引入其实时流地图，例如 (VR 步手游戏"开始") 

![AltspaceVR 中的 VR 游戏的屏幕截图](images/uploader-faq-img-03.png)

**14.是否必须托管场景文件？**
否，Altspace 在上传文件后会提供这些文件

**15.是否允许阴影？**
是

**16.使用上传程序进行访问有多快？**
如果已在"世界"中，可以在上传器中按Upload，重置"世界"，在 10 秒后查看更新后的场景。 通常，你会看到 30 秒到几分钟的循环，具体取决于场景的复杂性。 有一个饮料，你值得它作为一名 World-Builder！

**17.在哪里获取 3D 模型？**
Sketchfab、Sketchup、我的世界、Unity 资产存储等。

**18.它是否支持动画？**

![正在运行的自定义动画的 GIF](images/uploader-faq-img-04.gif)

**19.如何设置空间音频？** 导入选择的 wav 文件，在场景中创建一个空游戏对象，然后选择此对象。 将导入的声音拖放到 对象的检查器，它将创建音频源。 然后，将音量调整为不超过 0.5，将空间混合更改为 3D，并调整最小和最大距离以创建适当的声音区域。 默认情况下，这显示为球体（如碰撞体）。 若要获得真正的下降，需要根据需要调整下拉曲线。 [ (@IsThatToasted) ](https://www.youtube.com/watch?v=ktb2vAAwknw&list=PLGmYIROty-5bpzKQNK3mRMi4pmh_LinV4&t=642s&index=29)

**20.为什么看到交叉眼睛/异常？**
有时，上传程序不会成功覆盖呈现设置。 "转到编辑> Project 设置 >播放器"。 确保选中"支持 XR 设置 > 虚拟现实"，对于电脑和 Android，"立体声渲染方法"为"单通道"或"单通道 (预览版) " (请选择机器人图标) 。 然后再次生成 + 上传并重置你的世界。 