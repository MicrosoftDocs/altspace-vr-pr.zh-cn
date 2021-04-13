---
title: 使用混合现实扩展
description: 了解如何使用混合现实扩展并对其进行故障排除，从而扩展和改编你的 AltspaceVR。
ms.date: 03/11/2021
ms.topic: article
keywords: 混合现实，扩展，故障排除
ms.openlocfilehash: 498e71c48f7c67abc40ce4f4667c9eeac4c4e73b
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2021
ms.locfileid: "107211733"
---
# <a name="using-a-mixed-reality-extension"></a>使用混合现实扩展

[混合现实扩展](https://developer.altvr.com/) (MREs) 是可以在世界中将 [Helmets](https://account.altvr.com/mres/1173667287173955931) 用于工作 [Stargate](https://account.altvr.com/mres/1152987031857529562)的应用。 这就是具有编程经验的社区成员如何扩展 Altspace，而单向世界建筑者可以使其世界更加交互。 虽然世界上的任何人都可以使用 MREs，但只有世界大楼计划的人员才能浏览和生成 MREs。 

1. 浏览 [网站](https://account.altvr.com/mres)的 MRE 部分。 默认情况下，你会看到你自己的 MREs，因此请选择 " **Altspace** " 以查看官方 MREs 和 **特色** ，以查看来自社区的 MREs。 在世界范围内使用之前，先熟悉所有 MRE。 
2. 导航到 [Helmets](https://account.altvr.com/mres/1173667287173955931) MRE，并选择 " **复制到剪贴板**"。 
3. 进入你的世界，并打开世界编辑 **> SDK 应用的基本知识**。 将 Helmets 的 URL 粘贴到 "目标 URI" 字段中，然后选择 " **确认**"。 应显示 MRE 对象，并尝试连接到在云中运行的 MRE。 现在，你应该会看到一些 helmets，你可以单击它。
4. 移动/旋转/缩放 MRE，就像处理任何其他世界对象一样。

恭喜！ 现在正在使用 MREs--非常酷！

## <a name="troubleshooting"></a>疑难解答

**MRE 显示了一个哭表情符号** 
    * 请验证 URL 是否正确
    * 对象上的 "切换 **正在播放**" 选项，然后选择 "**确认**"
    * 尝试重新进入

**MRE 为滞后** 根据 MRE 的托管位置，可能会遇到某些网络延迟

**为什么必须粘贴 Url？**
将来，您可以管理和生成 MREs，就像从工具包中进行项目一样。 到现在为止，我们将继续使用 Url