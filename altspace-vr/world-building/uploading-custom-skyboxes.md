---
title: 上传自定义 Skyboxes
description: 获取有关在 AltspaceVR 体验中上载和排查自定义 skyboxes 的分步说明。
ms.date: 03/11/2021
ms.topic: article
keywords: skyboxes，故障排除
ms.openlocfilehash: 02d5bc762dc36d4195100e8155d6250789e833f7
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212018"
---
# <a name="uploading-custom-skyboxes"></a>上传自定义 Skyboxes

Skybox 是一种为世界创建 **背景** 的方式，使体验更具沉浸。 Skyboxes 有不同种类，但目前支持 **equirectangular**。 下面是使用360照相机创建的示例 (更多示例[) ：](http://moments.mankindforward.com/) 

![360 equirectangular 的视图](images/custom-skyboxes-img-01.jpeg)

你还可以使用 [Unity 上载](world-building-toolkit-getting-started.md) ，但此方法更简单。

1. 导航到 " [世界 > Skyboxes](https://account.altvr.com/skyboxes) "，然后按右侧的 " **创建** " 按钮

![世界网站页面打开到 skyboxes 面板](images/custom-skyboxes-img-02.png)

2. 填写名称并指定360映像。 这不一定是一张照片，有一些程序可以让你自行绘制，或者可以搜索一些在线。 准备就绪后，选择“创建”。 

![Skybox 创建窗体](images/custom-skyboxes-img-03.png)

3. 您可以选择上传 **预览** 图像，以便您可以轻松识别此 skybox。 你还可以上载 WAV 格式的环境音频。 

> [!IMPORTANT]
> 建议你在上载360映像后分别上传预览图像和环境音频。 如果将这些文件上传到一起，则文件大小可能会足够大以使进程停止。 [Jetsons World](https://account.altvr.com/worlds/1004174988393054363/spaces/1084431533181240311) 是如何使用带有环境音频的 Skybox 的一个很好的示例。 请注意，世界构建器如何保持音频音量低、听听声音非常小，使人们不会收到厌恶。 

4. 输入您的世界并打开 "世界" 编辑器。 在 "Skyboxes" 下，选择新的 Skybox。 几秒钟后，天空会按原义发生变化。 世界上的其他人也会看到天空发生变化。 若要切换回来，请选择同一列表中的 **默认** skybox。 

## <a name="troubleshooting"></a>疑难解答

**天空中有接缝或直线：- (。** 这是我们即将解决的 bug

**上载失败**
    * 尝试自行仅上载360映像
    * 尝试使用另一个较小的文件作为测试

**我找不到360照片**
    * Flickr 是良好的源 (更改筛选器以查找创造性的 commons) 
    * 自行学习！ 我们已成功完成了 Ricoh 的相机。 
**天空看起来有纹理或 blocky** 可能需要查找更高分辨率的图像。 通常约 2-5 MB，~ 5000 px x 2000 px

**这会影响我世界的帧速率！**
映像可能太大。 某些生成的 skyboxes 可能是8k。 它们通常附带移动友好的2k 版本--使用该版本。

**帮助我了解环境音频**
    * 使用 Audacity 等免费软件来降低音量或创建自己的循环。 请记住，音频会重复并在人们的耳中播放，因此保持较低且不令人讨厌
    * [免费音响](https://freesound.org/) 是合理的免版税声音来源
