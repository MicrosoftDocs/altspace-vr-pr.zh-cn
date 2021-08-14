---
title: 导入 glTF 模型
description: 了解如何将 3D glTF 模型正确导入 AltspaceVR 体验并排查任何问题。
ms.date: 03/11/2021
ms.topic: article
keywords: models， glTF， 导入， sketchfab， 故障排除
ms.openlocfilehash: 527c38fc49028258fa432445fe14a355710a18be65ee74252a8c39bc1bfe5190
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/11/2021
ms.locfileid: "119127028"
---
# <a name="importing-gltf-models"></a>导入 glTF 模型

> [!NOTE]
> 此功能目前适用于早期访问计划中的选定用户。

将 3D 模型和场景引入 Altspace 的一种方式是使用 [glTF 标准](https://en.wikipedia.org/wiki/GlTF)。 可以将 .glb 文件 (打包的 glTF) 创建模型，稍后可在"世界编辑器"中生成该模型。 它是上传自己的 [工具包 的替代方法](uploading-custom-kits.md)。 建议创建模型进行快速演示，因为当你想要最大程度地提高性能和可再使用性时，无需使用 Unity 和 Kits。 

1. 查找一些 glTF 3D 资产。 搜索位置之一是 Sketchfab (尝试筛选 **可下载** 的模型，) 。 [](https://sketchfab.com/search?features=downloadable&q=low+poly+wolf&sort_by=-pertinence&type=models) 找到它后，选择 **"下载三维模型"：**

![Sketchfab 中的 3D 狗模型](images/importing-models-img-01.png)

2. 将链接复制到模型并阅读许可要求。 
3. 下载 **glTF (自动转换)** 格式

![Sketchfab 下载选项，突出显示了自动转换格式](images/importing-models-img-02.png)

4. 打开 [GLB Packer 站点，](https://glb-packer.glitch.me)并选中"将 PNG 转换为 **JPEG** (beta) 
5. 解压缩下载的 glTF 文件，并将其一次拖动到 GLB Packer 浏览器选项卡中

![显示模型解压缩的窗口](images/importing-models-img-03.png)

6. 根据文件的数量和大小，可能需要一段时间处理。 处理完成后， **将下载 out.glb** 文件。 将该文件重命名为一些信息性信息- 这将是世界上对象的名称 (例如 **Low Poly 一**) 
7. 导航到 ["altvr.com >模型>并选择](https://account.altvr.com/users/sign_in) "创建 **"**
8. 指定 .glb 文件的位置，并确保将 Sketchfab 链接复制到说明中以用于归因。 如果需要，可以指定预览映像，然后选择"**创建模型"：**

![AltspaceVR 中的模型预览](images/importing-models-img-04.png)

9. 选择 **"复制到剪贴板"**
10. 使用 GLTF 打开"世界编辑器> **Altspace >基础知识>"**
11. 粘贴 URL，然后选择"确认 **"**

恭喜！ 你刚刚生成了第一个模型。

## <a name="troubleshooting"></a>故障排除

**单击"确认 **没有** 发生任何情况"**
    * 我们目前具有 10 万个多边形限制。 如果失败，请删除 对象，以避免用户加入你的世界时出现潜在问题
    * 资产可能有其他问题。 尝试将资产与尽可能少的多边形一同使用。
    * 引入的模型可能很小或很大。 尝试增加/减少缩放或移动头像，你可能位于模型内部！

**加载速度缓慢** 世界上的其他用户加载它的速度取决于其连接速度。 它也不像工具包资产一样进行缓存。 如果将一个模型放在"主页"中，则每次加入时都会重新下载相同的模型，这一点并不大。

**没有冲突** 默认情况下，不会对按此方式导致的对象发生冲突

**当我生成它时，我丢失了六个 DOF** 上的控件，或者我位于内部，因此很难对其进行操作是的，我们已了解这些问题，并希望尽快解决这些问题。  