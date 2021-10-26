---
title: Altspace 上传程序介绍
description: 了解如何通过 Altspace Uploader 使用 Unity 场景模板设置和上传 AltspaceVR 世界。
ms.date: 09/29/2021
ms.author: v-vtieto
ms.topic: article
keywords: toolkit、Altspace、uploader
ms.openlocfilehash: 8d71551fe552159c0078105307802774f44c0d47
ms.sourcegitcommit: 8c58f9f9ad1a3f9534141dee2c78e32792d0db7a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/25/2021
ms.locfileid: "130298783"
---
# <a name="introducing-the-altspace-uploader"></a>Altspace 上传程序介绍

> [!NOTE]
> - 如果感兴趣，请加入官方 [AltspaceVR 即为用户](https://discordapp.com/invite/altspacevr) #world频道。  
> - 如果尝试恢复旧空间，请参阅升级 [指南](upgrading-old-unity-projects.md)。 

通过上传程序，可以使用 Unity 场景作为世界模板。 你可以引入一个适合其内部装饰的房屋，也可以从 我的世界。 如果可以将它导入 Unity，可以这样将其导入 Altspace。 下面是一些[示例 World。](https://account.altvr.com/worlds/1046572460192825569)

![示例世界](images/unity-uploader-img-01.png)

## <a name="setup"></a>设置

1. 加入 [官方 AltspaceVR 中，](https://discordapp.com/invite/altspacevr) 访问#world频道。 朋友不会让朋友单独构建世界。
2. 阅读 [我们的世界入门](world-building-getting-started.md) 指南了解基础知识
3. [安装 Unity Hub](https://unity3d.com/get-unity/download)和 **Unity 2020.3.9。** 除非完全匹配此版本，否则上传程序将不起作用。 如果没有 Unity 帐户，则需要一个免费的 Unity 帐户。 在安装过程中，选择"个人 (，因为这样做是有趣的！) 并确保执行以下操作：
    * 包括 **Android 生成支持** 模块。
    * 在Windows，包括 Mono (**的 Mac** 生成) 模块。
    * 在 Mac 上，包括 **Mono Windows 生成 (支持)** 模块。
4. [下载 AltspaceVR 上传程序](https://aka.ms/AvrUrpUploader)
5. [在我们的网站上](https://account.altvr.com/space_templates/new) 创建模板。 将名称 **Hello World模板 。**
6. [创建一个"世界](https://account.altvr.com/worlds/my)**"，并** Hello World。 选择 **Hello World模板** "作为模板。

![已创建世界屏幕](images/unity-uploader-img-02.png)

## <a name="upload-your-scene"></a>Upload场景

> [!NOTE]
> 可在此处找到更详细的分步 [指南](https://buildingthemetaverse.medium.com/how-to-make-your-own-altspace-templates-and-kits-unity-2020-3-9-uploader-2-x-5b40e92bb759)。

1. 打开 Unity 中心并创建新的 Unity 2020.3.9 项目。 对于模板，请选择"**通用呈现管道"。**

    ![选择 URP Unity 模板](images/001-unity-templates.png)

1. 导航到将 Altspace Uploader 下载到的文件夹，然后将它从该文件夹复制或移动到新 Unity 项目的根文件夹。
1. 在菜单栏上的 Unity 中，选择"**窗口**  >  **程序包管理器&quot; 。**
1. 在程序包管理器栏中，选择加号下拉列表 (&quot;+") ，然后选择"**从 tarball 添加包"。**
1. 导航到包含 Altspace Uploader 的文件夹，选择"上传程序"，然后单击"打开 **"。**  加载包后 **，AltspaceVR** 将显示在菜单栏上：

    ![菜单栏上的 AltspaceVR](images/002-altspacevr-on-menu-bar.png)

> [!NOTE]
> 需要将 Altspace Uploader 包导入到要与 Altspace 一起使用的每一个 Unity 项目中。
1. 在菜单栏上，选择 **"AltspaceVR >模板"。**
1. 在 **"Altspace VR 模板** "对话框中，使用 Altspace 帐户凭据登录。  (MSA 登录名即将推出。 如果只是使用密码登录 Altspace Microsoft 帐户，则需要使用网站上"忘记了密码"选项创建密码。) 
1. 单击"**选择模板"** 下拉列表，然后选择 **"Hello World模板"。**
1. 选择场景：单击"选择 **.unity** 文件"省略号按钮 (三个点) ，导航到项目中的"资产场景"文件夹，然后选择  >  **"SampleScene.unity"** 并打开它。
1. 在 **"平台生成"下**：，**确保Windows"** 。 目前，不应选择其他两个选项 **（Android****和****Mac）。** 希望用户访问后，应针对所有平台生成并上传。"
1. 选择"**生成& Upload** 按钮。 此过程可能需要一两分钟。
1. 启动 Altspace，然后选择"**主菜单"，** 然后在菜单栏上选择"**我的世界"。**
1. 导航到 **Hello World，** 然后打开它。

    场景应类似于在 Unity 编辑器中看到的情况。

## <a name="whats-supported"></a>支持的操作

* 是：模型、碰撞、动画、粒子效果、音频、天盒等。
* 否：脚本。 出于安全考虑，将拒绝包含脚本的上传。
* 可能：动态全球照明等花式内容。
* Upload或一起为不同平台创建场景。
* 请参阅 [特别推荐世界](https://account.altvr.com/worlds/featured)。 许多是使用上传程序构建的。

## <a name="tips"></a>提示

* 加入 [官方 AltspaceVR 用户](https://discordapp.com/invite/altspacevr)。
* 在左侧的"模板"页上，我们按平台显示最新上传内容。 如果成功，则会看到 **1-2 分钟前**。 

!["模板"面板打开，突出显示了上传](images/template-upload-list.png)

* 更新时，你可以是"世界内"。 上传者说 **"Upload完成**"时，可以重置"世界"以查看更改。
* 使用简单的场景仅为电脑生成时，在 Altspace 中查看更改应该不到一分钟。
* 将"世界"设置为"专用"和"未列出"，以避免干扰。
* 将多维数据集放在原点，以便可以看到用户默认生成的位置。 上传时隐藏多维数据集。

## <a name="troubleshooting"></a>故障排除

**我崩溃或无法远程传送到任何内容** 需要向对象添加冲突，以将其传送至这些对象。

**没有任何更改**
    * 你是否在 Unity 中保存了场景？
    * 是否选择了要测试的平台？
    * 你在正确的世界吗？ 你是否在"上传者"和"世界"窗体中选择了正确的模板？
    * 是否检查了"模板"页统计信息？

**Upload失败或时间过长**
    * 最常见的上传错误由 Unity 版本错误导致。 必须与所需版本完全匹配。
    * 上传可能太大。 尝试将电脑场景< 100 MB。 从小规模开始，然后进行构建。 优化、优化、优化。
    * 尝试使用包含简单多维数据集的新项目。
    * 请勿在生成期间强制退出 -它可能会损坏场景。 尝试重新上传。

**这是一个缓慢的过程**
    * 建议仅在访问时为电脑生成 ，在以后针对 Android 进行生成。
    * 请尝试删除未使用的文件。 出于任何原因，Unity 有时都会过度使用。

**无法使用 Altspace 凭据登录**
    * 电子邮件区分大小写。
    * 尝试使用新项目。
    * 确保 Altspace 帐户运行良好。

## <a name="see-also"></a>请参阅

* [Unity Learn](https://unity3d.com/learn)
* [Unity 论坛](https://forum.unity.com)  
