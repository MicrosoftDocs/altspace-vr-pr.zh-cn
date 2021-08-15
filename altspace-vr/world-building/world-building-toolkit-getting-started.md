---
title: 引入世界建筑 Toolkit
description: 了解如何在世界大楼 Toolkit 中使用 Unity 场景模板来设置和上传 AltspaceVR。
ms.date: 03/11/2021
ms.topic: article
keywords: 工具包
ms.openlocfilehash: 8b66e35509060e00b2e52d3770380d009d7060339003f534d23fdd47372a57f0
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/11/2021
ms.locfileid: "119125388"
---
# <a name="introducing-the-world-building-toolkit"></a>引入世界建筑 Toolkit

> [!NOTE]
> 构建 Toolkit 是由我们的出色朋友[Anthony Madden](https://twitter.com/chigamesstudio)运行的社区项目，并支持我们的支持。 如果你感兴趣，请加入 [官方 AltspaceVR Discord](https://discordapp.com/invite/altspacevr) ，并访问 #world 构建渠道。 目前有一个 Mac 试用版试用版， [更多详细信息](https://altvr.com/altspacevr-mac)

使用上载程序，你可以使用 Unity 场景作为你的世界的模板。 你可以从我的世界中引入万圣节或你最喜欢的创建 haunted。 如果可以将其导入到 Unity 中，则可能会以这种方式将其导入 Altspace。 下面是几个 [示例](https://account.altvr.com/worlds/1046572460192825569)。

![示例世界](images/unity-uploader-img-01.png)

## <a name="setup"></a>安装

1. 加入 [官方 AltspaceVR Discord](https://discordapp.com/invite/altspacevr) 并访问 #world 构建渠道-朋友不让朋友单独构建。
2. 阅读我们的 [世界构建入门指南](world-building-getting-started.md) 以了解基础知识
3. [安装 Unity 中心](https://blogs.unity3d.com/2018/01/24/streamline-your-workflow-introducing-unity-hub-beta) 并安装 **unity 2020.3.9**。 除非完全匹配此版本，否则上载不起作用。 如果你没有帐户并选择 " **个人** "，你将需要一个免费的 Unity 帐户，因为这样做有乐趣！ 在安装过程中，请确保选中 " **Android 生成** " 选项并禁用自动更新。
4. [下载最新 Unity 上载者](upgrading-content-to-the-latest-unity.md#altspacevr-uploader-v090-upgrade-guide)
5. 在我们的网站上[创建模板](https://account.altvr.com/space_templates/new)。 将其命名为 **模板 Hello World**。
6. [创建一个世界](https://account.altvr.com/worlds/my) ，并将其命名为 **Hello World**。 选择 " **Hello World 模板** " 作为模板。

![已创建世界屏幕](images/unity-uploader-img-02.png)

## <a name="upload-your-scene"></a>Upload 场景

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-a-Template/player]

1. 打开 Unity 中心并创建新的 Unity 2020.3.9 项目。
2. 打开项目后，通过双击下载的文件（ (它是 Unity 包) 导入上载程序。 现在应会看到一个名为 " **AltspaceVR**" 的新选项卡。 需要为每个要与 Altspace 一起使用的 Unity 项目导入包
3. 打开 **菜单 > AltspaceVR > 生成设置**
4. 用你的 Altspace 帐户凭据登录
5. 选择 " **加载模板** "，然后选择 " **Hello World 模板**
6. 将多维数据集添加到场景并保存。
7. 检查 **生成是否适用于 Windows？** 
8. 选择“上传”。 大约一分钟后，你应该会看到 **Upload** 完成。
9. 通过从菜单 > 中启动 Altspace 和进入来加入 **Hello World** **> 我的世界**
10. 从 **菜单 > 设置 > 适中 > 重置空间** 重置世界
11. 应会看到多维数据集。 如以上视频所示，如以上视频所示，你可以在很少10秒内看到更改。

## <a name="whats-supported"></a>支持的操作

* 是：模型、冲突、动画、粒子效果、音频、skyboxes 等
* No：脚本。 出于安全考虑，包含脚本的上载将被拒绝
* 可能：动态全局照明等别致的内容
* 单独或同时为不同平台 Upload 场景
* 请参阅 [特色世界](https://account.altvr.com/worlds/featured)，其中许多都是使用上载器生成的

## <a name="tips"></a>提示

* 加入 [官方 AltspaceVR Discord](https://discordapp.com/invite/altspacevr)。
* 在左侧的 "模板" 页上，我们会显示平台的最新上载。 如果成功，则会看到 **1-2 分钟前**。Screen_Shot_2019-01-11 _at_1.21.04_AM.png

![突出显示了上传的模板面板打开](images/unity-uploader-img-03.png)

* 你可以在中进行更新。 上载者显示 **Upload 完成**，你可以重置世界来查看所做的更改。
* 使用简单场景构建仅适用于 PC 的时间应不到1分钟才能看到 Altspace 的变化
* 将世界设置为 "专用"，以避免干扰。
* 将多维数据集放在源位置，以便可以看到用户在默认情况下将生成的位置。 上载时隐藏多维数据集。

## <a name="troubleshooting"></a>疑难解答

**我会落下来或无法传送任何东西** 需要向要传送到对象的对象添加冲突。

**无更改**
    * 是否在 Unity 中保存了场景？
    * 选择了要测试的平台吗？
    * 你是否在正确的领域？ 是否在上载者和世界窗体中选择了正确的模板？
    * 是否检查了模板页统计信息？

**Upload 失败或超时**
    * 最常见的上传错误是具有错误的 Unity 版本。 它必须与所需的版本完全匹配。
    * 上传可能太大。 尝试将 PC 场景保持 < 100 MB。 从小开始，然后生成。 优化、优化、优化。
    * 尝试使用简单的多维数据集的新项目。
    * 请不要在生成过程中强制退出-它会损坏场景。 尝试 reuploading。

**这是缓慢的过程**
    * 建议仅在循环访问时，为 PC 构建。
    * 尝试删除未使用的文件。 出于任何原因，Unity 有时会过度。

**我无法用我的 Altspace 凭据登录**
    * 电子邮件区分大小写。
    * 尝试新的项目。
    * 确保 Altspace 帐户处于良好地位。

## <a name="see-also"></a>另请参阅

* [Unity 学习](https://unity3d.com/learn)
* [Unity 论坛](https://forum.unity.com)
