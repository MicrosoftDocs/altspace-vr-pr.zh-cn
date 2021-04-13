---
title: Unity 上载者帮助
description: 随时了解最新的 AltspaceVR Unity 上载程序问题和解决方案。
ms.date: 02/10/2021
ms.topic: article
keywords: 帮助，常见问题解答
ms.openlocfilehash: 814ff293cb98490900cd929f33477d15d3d668ae
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212047"
---
# <a name="unity-uploader-help"></a>Unity 上载者帮助

**1. 此工具多么棒？**

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/cheyenne-mountain-gate-room-v1/player]

这就是我的 Stargate Unity 场景，其中的 SDK 应用支持入口和 DND

**2. 我是视频学习器，我的视频在哪里？**

[查看我们的视频](https://youtu.be/km9CnVYPzoM)

**3. 在哪里可以找到示例？**

重要的是入门[领域](https://account.altvr.com/worlds/featured)和[Jimmy 的示例](https://account.altvr.com/worlds/1046572460192825569)

**4. 这是否适用于工具包和新的 SDK？**
是的，如果需要，你可以将所有工具一起使用。 我们正在努力开发它们，以便无缝协作。

**5. 它是否支持粒子效果？**

![雪粒子效果的 GIF](images/uploader-faq-img-01.gif)

**6. 我是否可以获取 spatialized 音频？**
目前不是，但你可以将音频源放在本地化区域中。 

**7. 融入照明是否起作用？**
是，但你的灯光必须设置为 "融入" 而不是 "mixed"

**8. 全局照明是否起作用？**
是

**9. 是否始终需要重置世界？**
是的。 每次都必须重新加载 Unity 资产包。 

**10. 我是否可以使用我自己的自定义材料和着色器？**

![自定义材料和着色器的 GIF](images/uploader-faq-img-02.gif)

**11. 我只能上传到一个平台吗？**
是，使用上载工具。 但是，在你为其平台上传场景之前，Android 上的用户不会看到任何内容。 

**12. 是否允许脚本？**
不能，出于安全原因，我们无法允许脚本或脚本引用。 如果上传包含脚本或脚本引用，则会拒绝该引用。 如果你需要编写脚本，请查看新的 SDK。 

**13. 我可以上传的场景有多大？**
建议你开始使用小型，并注意 Altspace 中没有怪物电脑的人员。 也就是说，我们已经让游戏进入了用于实时流的地图 (例如，) 

![AltspaceVR 中的 VR 游戏屏幕截图](images/uploader-faq-img-03.png)

**14. 我是否必须承载场景文件？**
不可以，Altspace 在上载文件后正在为其提供服务

**15. 是否允许阴影？**
是

**16. 可以使用上载上载的速度有多快？**
如果你已在世界各地，则可以在上载程序中按 "上传"，重置世界，并在10秒内查看更新的场景。 通常，你会看到从30秒到几分钟的循环，具体取决于场景的复杂性。 有一个饮料，您应该为它提供世界上！

**17. 从何处获得3D 模型？**
Sketchfab、Sketchup、Minecraft、Unity 资产存储区等。

**18. 它是否支持动画？**

![自定义动画的 GIF 运行](images/uploader-faq-img-04.gif)

**19. 如何设置空间音频？** 导入所选的 wav 文件，在场景中创建一个空游戏对象，并选择此对象。 将导入的声音拖放到对象的检查器中，它将创建音频源。 然后，将音量调整为不超过0.5，将空间混合更改为3D，并调整最小和最大距离以创建适当的声音区域。 默认情况下，它显示为球，如 colliders。 若要获取真正的拖放功能，您需要根据自己的喜好调整下拉曲线。 [ 通过 @IsThatToasted)  (](https://www.youtube.com/watch?v=ktb2vAAwknw&list=PLGmYIROty-5bpzKQNK3mRMi4pmh_LinV4&t=642s&index=29)

**20. 我如何查看跨 eyed/问题？**
有时上载程序并不能成功地重写您的呈现设置。 "请参阅编辑 > 项目设置 > Player"。 请确保选中 "XR 设置 > 虚拟现实支持"，并将 "立体声呈现方法" 为 "单一传递" 或 "单一传递 (预览) " 以用于 PC 和 Android (选择 "机器人" 图标) "。 之后再重新生成并重新上传。 