---
title: 使用 Interactables Spawner
description: 了解如何创建、使用和自定义可交互的生成程序，以将项放在 AltspaceVR 空间中。
ms.date: 02/10/2021
ms.topic: article
keywords: spawner， 交互， 自定义项
ms.openlocfilehash: abeddec5c2b50e0612db5efb6bc2e3c5bd9de4a8b67c50b19afee18b17c5e746
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/11/2021
ms.locfileid: "119127382"
---
# <a name="using-the-interactables-spawner"></a>使用 Interactables Spawner

使用 Interactables Spawner，可以在事件、世界或家庭空间中放置可交互的项。 此功能目前属于我们的早期访问计划[](../world-building/early-access.md)，除非已选择通过主菜单启用，否则此功能不可用。

> [!NOTE]
> 在继续试用此功能时，请注意，生成过多的可交互对象可能会影响环境或事件的性能。 

## <a name="creating-an-interactable"></a>创建可交互的

若要将对象转换为可交互对象，请：

1. 将 对象放在空间中。
2. 然后，在对象列表中找到条目，然后选择它旁边的 **齿轮** 图标以打开其设置：

![世界编辑器打开，突出显示对象列表](images/interactables-spawner-img-01.png)

在设置页上，你将找到一个新复选框" **对象生成** 程序"，它用于使其成为可交互的对象。

1. 选中该框并选择"确认 **"。**
2. 在编辑模式下，可以在空间中围绕对象的生成位置移动。
3. **退出编辑模式** 以启用项交互。

![在 AltspaceVR 应用中打开更新项目窗口](images/interactables-spawner-img-02.png)

## <a name="other-customizations"></a>其他自定义

在返回 **该对象的属性时** 启用"对象生成程序"后，将存在一个额外的设置，可以应用于生成的对象的行为方式。

> [!NOTE]
> 可交互的对象缩放：与"小数位"（即首次选取对象之前对象在世界中的显示方式）相比，这将设置对象在选取时的规模。

工具包制造商可能会注意到，在 AltspaceVR 运行时对工具包所做的更改在重新启动 AltspaceVR 之前不会生效。

最近，我们在"中等"选项卡下添加了一个 **设置"重新加载世界工具包"按钮**。 单击此按钮 (你) 重新进入空间，再次重新加载所有工具包，这将仅下载在 AltspaceVR 中更新的工具包的新版本。

![在 AltspaceVR 应用中打开审查设置面板](images/interactables-spawner-img-03.png)