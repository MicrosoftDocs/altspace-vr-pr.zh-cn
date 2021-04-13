---
title: 上传自定义工具包
description: 了解如何在 AltspaceVR 中设置、生成和上传自己的自定义工具包以及故障排除帮助。
ms.date: 03/11/2021
ms.topic: article
keywords: 工具包，上传，故障排除
ms.openlocfilehash: e5a1b9c2ef5339db0cb821cb6f7d21a930416451
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212077"
---
# <a name="uploading-custom-kits"></a>上传自定义工具包

世界编辑器包含可在世界中生成的项目。 例如， [Campfire 工具包](https://account.altvr.com/kits/993516233267609824) 有多种类型的树，每种类型的树都是一个项目。 若要创建自己的工具包，必须创建 Unity AssetBundles 并上载包含每个项目的 Unity Prefab 的 .zip 文件，并在我们的网站上注册每个项目。 幸运的是，社区驱动的 Unity 上载程序可自动执行大部分工作流。 上传后，你可以在世界中从自己的工具包生成对象，其他用户可以自动查看它们。 稍后，你可以与朋友分享你的工具包，甚至可以通过功能来与整个社区共享你的工具包。

## <a name="prerequisites"></a>先决条件

1. [安装 Unity 中心和 Unity](world-building-toolkit-getting-started.md)
2. 下载最新版本的[Unity 上载](https://altvr.com/download-latest-unity-uploader/)者

## <a name="setup"></a>设置 

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-my-own-Kits-Part-1-Setup/player]

1. 在我们的网站上的[世界 >](https://account.altvr.com/kits)套件中创建工具包
2. 将工具包 ID 从浏览器的地址栏复制到剪贴板 (此步骤在第) 版上载程序中更容易
3. 创建新的 Unity 项目
4. 通过双击包导入 Unity 上载程序

![导入 unity 上载程序包](images/custom-kits-img-01.png)

5. 用你的 Altspace 电子邮件和密码登录到上载程序

![Unity 中的 AltspaceVR 登录接口](images/custom-kits-img-02.png)

## <a name="generate-and-upload-your-kit"></a>生成和上传工具包

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-my-own-Kits-Part-2/player]

1. 使用你的工具包 ID 作为前缀和主题 (填写 **工具包文件夹名称** ，例如 **1137484494681408069_Pirates**) ，并使用你的工具包 Id 作为前缀填写 **包资产名称** 。 所有资产都需要具有此前缀。

![Unity 中的 AltspaceVR 接口，套件文件夹名称](images/custom-kits-img-03.png)

2. 对于每个项目或一组项目：
* 将源 Prefab (s) 拖到 "层次结构" 选项卡
* 选择要包含在集合中的 barrels，例如五种类型的
* 用 **桶** 更新 **工具包资产名称**
* 选择 "**将 GameObject (s) 转换为包 Prefab** "
* 验证是否在 "资产/Prototyping" 文件夹中创建了新的 Prototyping 和屏幕截图

![Unity 中的 AltspaceVR 接口，并选择了项目](images/custom-kits-img-04.png)

> [!NOTE]
> 如果要对生成的 Prefab 进行任何修改，请将其拖回层次结构，进行更改，然后在 "检查器" 选项卡中单击 " **应用** " 以更新 Prefab。 

3. 准备就绪后，在 "上载程序" 选项卡中向下滚动，并准备使用资产捆绑生成 zip 文件
4. 若要加快迭代速度，请取消勾选 **适用于 Android 的生成工具包？**。 请记住，稍后在完成迭代或想要共享/功能包时，将生成并上载适用于 Android 的版本。 
5. 选择 **负载套件 Prefab 目录**
6. 选择与工具包文件夹名称匹配的版本旁边的 " **生成** "。 通常从同一 Unity 项目生成多个包。 此过程可能需要一段时间，具体取决于你的工具包大小。 完成后，包含 zip 文件的文件夹将自动打开。 
7. 请参阅网站，编辑之前创建的工具包，并上传生成的 zip 文件。 此上传可能需要一段时间，具体取决于文件大小。
    * 如果成功，你会在 "上传" 文件的大小、电脑和 Android 上以及上次更新的时间显示在左侧
    * 如果不成功，请确保没有任何脚本，我们不支持脚本，我们将检查它们的安全性，然后重试。

恭喜！ 你已准备好通过自己的工具包构建世界！

## <a name="troubleshooting"></a>疑难解答 

**是否有限制？**
尚无硬性限制，但请记住，即使只使用了一个项目，用户也需要为整个工具包下载其平台的 AssetBundle。 尝试将每个平台的下载保持在 5 MB 或更少。 实现此目的的一种方法是将其拆分为较小的工具包。 例如，200属性应分成一半。 

**看到 "分割眼睛"？**
重新导入最新的上载者以获取正确的呈现设置

**更新/更改未反映？**
    * 检查工具包页上的更新时间
    * 重新进入世界将无法正常工作-重新启动客户端。 甚至可能需要几分钟的时间来更新
    * 请确保文件夹名称或 prefab 名称中没有空格 **，例如 "party_favors" 与 "参与方优先"**

虽然 **我有一个脚本，但** AssetBundle 浏览器有时会自动包含文件。 尝试隔离正在引入的模型。 例如，请勿将其拖放到其他 Prefab 的一部分

**如何处理粒子系统和动画？**
对于这些情况，接下来，将在1x1x1 多维数据集下定位到网格呈现并禁用冲突。 粒子系统应启用循环并且应将其 **缩放** 设置为 **层次结构** ，以便能够正确地在 Altspace 中进行缩放。 为所有动画生成 prototyping 后，对每个动画的 **冲突** 对象禁用冲突。

**项目很暗** 您是否已将模型的材料着色器设置为 **仅限点即点即点光**？

**项目不是正确的方法** 旋转 **模型** 和 **碰撞** 器并更新 Prefab。 旋转父级不会执行任何操作，这会被忽略。 您可以使用 " **旋转覆盖** " 字段轻松完成此操作。

**这些项目是否可以与 SDK 的 **CreateFromLibrary** 函数一起使用？**
是