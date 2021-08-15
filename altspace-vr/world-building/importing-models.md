---
title: 导入 glTF 模型
description: 了解如何将 3D glTF 模型正确地导入 AltspaceVR 体验，并解决任何问题。
ms.date: 03/11/2021
ms.topic: article
keywords: 模型，glTF，导入，sketchfab，故障排除
ms.openlocfilehash: 527c38fc49028258fa432445fe14a355710a18be65ee74252a8c39bc1bfe5190
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/11/2021
ms.locfileid: "119127028"
---
# <a name="importing-gltf-models"></a>导入 glTF 模型

> [!NOTE]
> 此功能在 "早期访问" 计划中可用于选择用户。

将三维模型和场景引入 Altspace 的一种方法是使用 [glTF 标准](https://en.wikipedia.org/wiki/GlTF)。 您可以上载 (打包的 glTF) 的 glb 文件，以创建以后在世界编辑器中生成的模型。 这是 [上传自己的工具包](uploading-custom-kits.md)的替代方法。 建议为快速演示创建模型，因为当你想要最大程度地提高性能和可重用性时，无需使用 Unity 和工具包。 

1. 查找一些 glTF 3D 资产。 要搜索的一个位置是 Sketchfab (尝试 [按如下所示筛选](https://sketchfab.com/search?features=downloadable&q=low+poly+wolf&sort_by=-pertinence&type=models)**可下载** 模型) 。 找到后，选择 " **下载3D 模型**"：

![Sketchfab 中的3D 狗模型](images/importing-models-img-01.png)

2. 将链接复制到模型并阅读许可要求。 
3. 下载 **Autoconverted 格式 (glTF)** 版本

![突出显示自动转换格式的 Sketchfab 下载选项](images/importing-models-img-02.png)

4. 打开 [GLB Packer](https://glb-packer.glitch.me) 网站并选中 " **将 PNG 转换为 JPEG (beta)**
5. 解压缩你下载的 glTF 文件，并将其一次性拖到 GLB Packer 浏览器选项卡中

![显示模型解压缩的窗口](images/importing-models-img-03.png)

6. 处理过程可能需要一段时间，具体取决于文件的数量和大小。 处理完成后，将下载 **glb** 文件。 将该文件重命名为信息性信息--这将是世界 (的对象的名称，例如 **Low Poly 狼. glb**) 
7. 导航到 [altvr.com > 更多 > 模型](https://account.altvr.com/users/sign_in)并选择 "**创建**"
8. 指定 glb 文件的位置，并确保将 Sketchfab 链接复制到 "归属说明"。 如果需要，可以指定预览图像，然后选择 " **创建模型**"：

![AltspaceVR 中的模型预览](images/importing-models-img-04.png)

9. 选择 "**复制到剪贴板**"
10. 打开 **世界编辑器 > Altspace > 基础知识 > GLTF**
11. 粘贴到 url，然后选择 "**确认**"

恭喜！ 你只是生成了第一个模型。

## <a name="troubleshooting"></a>疑难解答

**单击 " **确认** 没有发生"**
    * 目前有10万个多边形限制。 如果此操作失败，请删除对象，以避免在加入你的用户时出现潜在问题
    * 资产可能还有其他问题。 尝试使用尽可能少多边形的资产。
    * 要引入的模型可能很小，也可能很大。 尝试增加/减少规模，或四处移动您的头像，你可能会在模型中！

**加载速度缓慢** 世界上其他用户的负载速度将取决于其连接速度。 它也不缓存，如套件资产。 如果你将其放在家里，则每次加入时，最终都将 redownloading 相同的模型，这种情况并不好。

**无冲突** 默认情况下，不会对以这种方式引入的对象发生冲突

**当我生成控件时，我在六个 DOF 上失去了控制** 是的，我们意识到这些问题，希望尽快解决这些问题。  