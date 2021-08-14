---
title: 使用 teleporter
description: 了解如何在 AltspaceVR 中使用 teleporter 从一个事件或世界传播到另一个事件。
ms.date: 03/11/2021
ms.topic: article
keywords: teleporter
ms.openlocfilehash: 79c5b09e1643a70939ba1e967a948ac6c80c2b615bce9eef598d0e07b7722ea3
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/11/2021
ms.locfileid: "119126173"
---
# <a name="using-the-teleporter"></a>使用 teleporter

从一个事件或世界传播到另一个事件是您和社区浏览 AltspaceVR 必须提供的所有内容的好办法。

## <a name="the-short-version"></a>短版本

![Teleporting 步骤从编辑器面板到设置 teleportation 目标](images/teleporter.png)

## <a name="the-slightly-longer-version"></a>略长版本

首先，请确保你已在 Homespace 中，在你创建或已在中获得 Terraformer 角色的活动或世界。 如果处于2D 模式，并且在 UI 右下方看不到 "世界编辑器" 按钮，则右键单击鼠标按钮可切换到 "开/关"。 如果仍然看不到 "世界编辑器" 按钮，则可能是其他人的空间。 如果是这种情况，请要求主机为你授予 Terraformer 角色。

它还有助于： 
1. 首先创建事件或世界
2. 如果要在其中生成 Teleporter，则可在 Teleporter 目标面板中填充事件/世界，使你能够更快、更轻松地将其连接起来。

帮助您在2D 模式下使用 Teleporters 进行导航的另一项技巧是使用 Ctrl + 空格键。 它将显示命令提示符，你可以键入： back，这会返回到你的最后一个空间！ 

现在，转到要生成 Teleporter 的位置，并选择 "在世界上编辑器/编辑器" 面板/"基本"/"Teleporter"。

这会显示 Teleporter 目标面板。 你将看到三个类别可供选择：

* **我的空间** -已创建的世界列表。
* **最新** -已有的最近事件列表。 如果你想要旅行到某个事件，则使用此选项，这是将你转到某个事件的唯一选项，另一个2只允许你在世界之间旅行。 注意：如果要连接已导入世界的前行事件，请参阅下面的 "高级"，需要在导入的环境中生成并设置 Teleporters，而不是在实际事件中进行。
* **特色** -可以将 Teleporter 设置为旅行到的特色领域列表。

选择要使用的事件或世界，这将生成 Teleporter，并使事件或世界名称的文本标签略微滞后一些。 因此，可以选择 "现有对象" 部分中的齿轮图标来更改标签名称。

你可以使用光标在 Teleporter 上进行选择 (系统会询问你是否可以转到该位置（如果是 misclick，则为) ）或将你的头像直接移到 Teleporter 和 presto。 告诉我们！

## <a name="advanced-features"></a>高级功能

如果要使用自定义世界 (的前一行来创建会议、峰会或更大的事件，例如，基础世界、Unity 上载程序空间模板 Re-Import 世界) 需要在基础世界中设置 Teleporter，而不是在实际事件中设置。 请确保将 Teleporter 设置为到达正确的事件 (必须来自你的基础世界) 的 "最新列表"，然后在事件中 Re-Import 世界，使 Teleporters 显示在所有前行事件空间中。

## <a name="faqs"></a>常见问题

**错误： ' 对不起，我们喜欢，但我们只是**

事件可能有一个附加到它的组，因此只有该组中的用户名可以进入该 Teleporter，以便访问该专用组事件。

**一个空间中可以使用多少个 teleporters？**

Teleporters 正在将透明纹理与动画粒子效果结合使用，因此，最好不要在同一点/重叠中包含太多的，因为这可能会影响性能。 如果在空间中全部分散，请不要在同一区域中尝试使用超过4个，如果它们都在空间中，则不能超过10个。