---
title: 使用 Interactables Spawner
description: 了解如何创建、使用和自定义 interactables spawner，以便将项放入 AltspaceVR 空间。
ms.date: 02/10/2021
ms.topic: article
keywords: spawner，交互，自定义
ms.openlocfilehash: 7f4b87591b2e11b2084af4d2bf83748ed51fd193
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212088"
---
# <a name="using-the-interactables-spawner"></a>使用 Interactables Spawner

可以通过 Interactables Spawner 将种不可交互项放置在事件、世界或主空间中。 此功能当前是 [早期访问计划](../world-building/early-access.md) 的一部分，除非你已在主菜单中选择了，否则此功能将不可用。

> [!NOTE]
> 尽管我们继续试点此功能，但请注意，生成太多 interactables 可能会影响环境或事件的性能。 

## <a name="creating-an-interactable"></a>创建种不可交互

若要将对象转换为种不可交互对象，请执行以下操作：

1. 将对象放入空间。
2. 然后，在 "对象" 列表中找到条目，然后选择它旁边的 **齿轮图标** 以打开其设置：

![显示突出显示对象列表的世界编辑器打开](images/interactables-spawner-img-01.png)

在 "设置" 页上，你将看到一个新的复选框 **"对象 spawner"**，它用于使其成为种不可交互对象。

1. 选中此框，然后选择 " **确认**"。
2. 在编辑模式下，可以在空间中的对象的生成位置周围移动。
3. **退出编辑模式** 以启用项交互。

![在 AltspaceVR 应用中打开 "更新项目" 窗口](images/interactables-spawner-img-02.png)

## <a name="other-customizations"></a>其他自定义

当你返回到该对象的属性后，启用 **"Object spawner"** 后，将有额外的设置可应用于生成的对象的行为方式。

> [!NOTE]
> 种不可交互对象比例：这会在选取对象时设置对象的小数位数，而 "小数位数" 是指对象在世界上第一次选取之前的显示比例。

包制造商可能会注意到，在 AltspaceVR 运行时对你的工具包所做的更改不会生效，直到你重新启动 AltspaceVR。

最近，我们已在 " **中等设置** " 选项卡下添加一个名为 " **重新加载**" 的按钮。 单击此按钮将导致 (您) 重新输入空间，重新加载所有工具包，这将只下载在 AltspaceVR 时更新的工具包的新版本。

![在 AltspaceVR 应用中打开适中的设置面板](images/interactables-spawner-img-03.png)