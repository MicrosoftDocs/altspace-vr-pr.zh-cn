---
title: 上传自定义工具包
description: 了解如何在 AltspaceVR 中设置、生成和上传自己的自定义工具包，以及故障排除帮助。
ms.date: 03/11/2021
ms.topic: article
keywords: 工具包， 上传， 故障排除
ms.openlocfilehash: 9a90bff2360d854dc398a35501f07cddcbce5c6c66ef8230f2e412a022f8aed0
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/11/2021
ms.locfileid: "119125508"
---
# <a name="uploading-custom-kits"></a>上传自定义工具包

世界编辑器包含工具包Artifacts可生成到你的世界。 例如 [，"Campfire Kit"](https://account.altvr.com/kits/993516233267609824) 具有多种类型的树-每种类型的树都是一个"项目"。 若要创建自己的工具包，必须创建 Unity AssetBundles 并上传包含每个项目的 Unity 预制件的 .zip 文件，并在我们的网站上注册每个项目。 幸运的是，社区驱动的 Unity 上传程序可自动执行大部分工作流。 上传后，可以从自己的工具包在"世界"中生成对象，其他用户可以自动看到它们。 稍后，可以与好友共享工具包，甚至可以通过特别推荐Community整个工具包。

## <a name="prerequisites"></a>必备条件

1. [安装 Unity Hub 和 Unity](world-building-toolkit-getting-started.md)
2. 下载最新版本的 Unity [上传程序](https://altvr.com/download-latest-unity-uploader/)

## <a name="setup"></a>安装 

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-my-own-Kits-Part-1-Setup/player]

1. 在 Worlds > [Kits 网站上创建工具包](https://account.altvr.com/kits)
2. 将工具包 ID 从浏览器的地址栏复制到剪贴板 (在上传程序版本 0.9 及以上版本中，此步骤会) 
3. 创建新的 Unity Project
4. 通过双击包导入 Unity 上传程序

![导入的 unity 上传程序包](images/custom-kits-img-01.png)

5. 使用 Altspace 电子邮件和密码登录到上传程序

![Unity 中的 AltspaceVR 登录接口](images/custom-kits-img-02.png)

## <a name="generate-and-upload-your-kit"></a>生成并上传工具包

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-my-own-Kits-Part-2/player]

1. 在 **"工具包文件夹** 名称"中填写"工具包 ID"作为前缀和主题 (例如，1137484494681408069_pirates) 填写"工具包资产名称"，将工具包 ID作为前缀。 所有资产都需要具有此前缀。

![Unity 中具有工具包文件夹名称的 AltspaceVR 接口](images/custom-kits-img-03.png)

2. 对于每个项目或一组Artifacts：
* 将源预制 () "层次结构"选项卡
* 选择要包括在一个集合中的产品，例如五种类型的桶
* 更新 **工具包资产名称**
* 选择 **"将 GameObject (") 工具包预制件**
* 验证"Assets/Prefabs"文件夹中是否创建了新的预制项和屏幕截图

![Unity 中的 AltspaceVR 接口，已选择项目](images/custom-kits-img-04.png)

> [!NOTE]
> 如果要对生成的预制文件进行任何修改，请将其拖回到"层次结构"中，进行更改，然后单击"检查器"选项卡中的"应用"以更新预制。 

3. 准备就绪后，向下滚动"上传程序"选项卡，准备使用资产捆绑生成 zip 文件
4. 为了加快迭代速度，请取消选中"适用于 **Android 的生成工具包？"。** 请记得在稍后完成访问或想要共享/启用工具包时，为 Android 生成和上传版本。 
5. 选择 **"加载工具包预制件目录"**
6. 选择 **"工具包** 文件夹名称"旁边的"生成"。 从同一 Unity 项目生成多个工具包很常见。 这可能需要一段时间，具体取决于工具包的大小。 完成后，包含 zip 文件的文件夹将自动打开。 
7. 转到网站，编辑之前创建的工具包，并上传生成的 zip 文件。 此上传可能需要一段时间，具体取决于文件大小。
    * 如果成功，你将在左侧的"上传"下看到文件大小，以及电脑和 Android 的文件大小以及上次更新时间
    * 如果失败，请确保没有任何脚本，我们不支持脚本，我们会检查这些脚本的安全性，然后重试。

祝贺你！ 你已准备好使用自己的工具包构建世界！

## <a name="troubleshooting"></a>疑难解答 

**是否有限制？**
尚没有硬性限制，但请记住，即使只使用了一个 Artifact，用户也需要下载整个工具包的平台的 AssetBundle。 尝试将每个平台的下载内容保留为 5 MB 或更少。 为此，一种方式是将内容拆分为较小的工具包。 例如，200 个属性应拆分为一半。 

**看到"拆分眼睛"？**
重新导入最新的上传程序，获取正确的呈现设置

**更新/更改未反映出来？**
    * 在"工具包"页上检查更新时间
    * 重新访问世界将不起作用 -- 重启客户端。 即使这样，更新也可能需要几分钟时间
    * 请确保文件夹名称或预制名中没有空格，例如 **"party_favors"与"party favors"**

**它一直说我有一个脚本，但没有** AssetBundle 浏览器有时会自动包含文件。 尝试隔离要引入的模型。 例如，当它是另一个预制件的一部分时，请不要将其拖入

**粒子系统和动画呢？**
对于这些对象，接下来将它们放在原点位置的 1x1x1 立方体下，并禁用网格渲染和冲突。 粒子系统应启用循环， **并且缩放** 应设置为 **"** 层次结构"，以便我们可以在 Altspace 中正确缩放它们。 生成所有动画的预制件后，请禁用每个动画 **的冲突** 对象上的冲突。

**颜色Artifacts深色** 是否将模型的材料着色器设置为 **"移动/顶点仅照明"方向光**？

**项目未以正确的方式出现** 旋转 **模型和****碰撞体** 并更新预制件。 轮换父级不会执行任何忽略的。 可以使用"旋转 **替代"** 字段轻松完成此操作。

**这些Artifacts与 SDK 的 **CreateFromLibrary 函数一起** 使用吗？**
是