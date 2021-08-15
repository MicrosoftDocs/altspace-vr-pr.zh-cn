---
title: 使用 FrontRow 功能缩放受众
description: 了解如何使用 FrontRow 功能启用、故障排除和缩放 AltspaceVR 受众。
ms.date: 03/11/2021
ms.topic: article
keywords: 缩放，前行
ms.openlocfilehash: 3b6a518a463fc373439f411d4ae75352a0343304b1fb73c8848d3bfd5fa19973
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/11/2021
ms.locfileid: "119128053"
---
# <a name="scaling-your-audiences-with-frontrow-feature"></a>使用 FrontRow 功能缩放受众

## <a name="what-is-frontrow"></a>什么是 FrontRow？

FrontRow 是一种 AltspaceVR 技术，允许跨多个实例"镜像"整个事件。 FrontRow 允许将受众缩放到超出单个房间上限，并可用于在单个活动中容纳大量受众。 如果没有 FrontRow，则受众大小将限制为主环境的空间上限。

## <a name="how-does-it-work"></a>它是如何工作的？

FrontRow 为主机体验添加了额外的特性和功能，让你可以最大限度地控制事件和受众。 

* **On-Air** 工具将添加到主机面板。
    * 使用 **On-Air，** 你可以选择"镜像"对象 (例如：演示者、执行者、面板成员、受众成员等) FrontRow 还会在所有房间中"镜像"内容。 因此，如果你有一个扬声器面板和一个幻灯片演示文稿，可以在所有 FrontRow 房间中"镜像"说话人与演示文稿。
* 来宾 **面板** 中会打开"房间"选项卡。
    * 此面板提供一目了然的概述，其中概述了你有多少个房间、每个房间有多少位来宾以及这些来宾是谁。 在此处，还可以选择"添加房间"或"删除房间"，以便管理最适合事件的设置大小。
    * 可以从房间到房间进行远程传送，并轻松地在空间之间分发审查器。
* 反应式受众分布
    * 当来宾开始进入空间时，FrontRow 会直观地分发它们。 可以配置为一次填充一个房间，或同时填充多个房间，以更均匀地分配受众。

## <a name="when-to-enable-frontrow"></a>何时启用 FrontRow

需要超出环境空间容量进行缩放时，请转换为 FrontRow。

* 官方 AltspaceVR 模板环境允许每个空间最多 50 个头像。 如果希望受众超过 50 个，请使用 FrontRow 创建 50 个头像的多个房间。
* 自定义 (Unity 上传器/自定义空间模板) ，如果用作事件环境，则每个空间最多允许 50 个头像。 如果希望受众超过 50 人，请使用 FrontRow 创建多个 30 个头像房间。

## <a name="how-to-enable-frontrow"></a>如何启用 FrontRow

1. [创建事件](https://account.altvr.com/events/new)。
2. 输入事件。
3. 进入事件后，打开 **右下角** 的"主机工具"。
4. 在"参与 **面板"按钮上** 选择。
5. 导航到" **房间"** 选项卡，可在此处 **添加房间**
    * 请注意，生成另一个房间可能需要 30 秒。 
6. 新房间打开后，你将看到它显示在"房间 **"选项卡** 中。 

## <a name="how-to-use-frontrow"></a>如何使用 FrontRow

将事件转换为 FrontRow 事件会向主机面板添加一些额外的工具和功能。 最值得注意的是，将显示" **房间"** 选项卡。 在此选项卡中，可以：

* **添加房间** - 向活动添加额外的房间。 
* **删除房间** - 从活动中删除整个房间。
* **重置空间** - 重置所选房间。 这会导致来宾重新访问同一空间。
* **重新分发** - 将一个房间中当前的所有来宾重新分发到其他房间。  (适合使用 0.) 
* **Teleport** - 转到另一个房间。

在 FrontRow 事件中，主机还将看到一些其他工具和功能，例如 **On-Air**。 此按钮位于"主机工具"旁边，允许主机或审查器镜像受众成员和其他参与者，以便它们可以跨所有空间可见。  (作为主机，你可能还希望自己使用 **On-Air。**  (Pro提示：[使用主机区域](https://altvr.com/holiday2020/)自动为 zone.) 

请查看 [FrontRow 事件的](../tutorials/host-tools-for-events.md) 主机工具概述一文，全面深入地了解 FrontRow 事件中主机可用的每个特性和功能。

![主机面板工具概述](images/scaling-audiences.png)

如果需要一起处理，请通过以下方法向支持团队提交 altvr.com/eventsupport [](https://help.altvr.com/hc/en-us/requests/new?ticket_form_id=360001833313)

* 包括事件 ID URL (例如 [https://account.altvr.com/events/1461193283454632537](https://account.altvr.com/events/1461193283454632537) ：) 
    * 为此，可以登录到我们 www.altvr.com，然后访问"事件/我的事件/你的事件"，然后复制浏览器地址栏中的 URL，或单击"共享"按钮获取 URL。
    * 票证响应可能需要 3-5 个工作日，因此请尽可能提前提交请求。
 
## <a name="how-will-i-know-when-frontrow-is-on"></a>如何知道 FrontRow 何时打开？

一旦开始看到添加到"房间"选项卡的其他房间，就会知道事件 **已** 转换。如果需要帮助， 
 
## <a name="can-i-turn-off-frontrow"></a>能否关闭 FrontRow？

你确实可以。 可以 **像添加房间** 一样轻松地删除 **房间。** " **删除房间** "按钮位于"房间"选项卡中每个 **房间的** 旁边。删除其中有人的房间时，FrontRow 会通知他们删除内容，并将其重新分发到其他活动房间。 通过一直将事件缩减到一个房间，可以有效地关闭 FrontRow。 
 
## <a name="any-pro-tips-or-helpful-hints-to-be-aware-of"></a>任何需要注意的 Pro 提示或有用提示？

事件的设置取决于不同的因素。 虽然没有确切的成功公式，但以下是在 AltspaceVR 中托管事件或 (FrontRow) 提示和有用提示：
* 考虑受众的体验，并执行可针对所有内容进行优化。 例如，如果环境不方便移动，则可能会破坏移动头戴显示设备中的某人的体验。 为了增加受众，你需要留下很好的第一印象。
* 熟能生巧。 在托管直播活动之前，请执行尽可能多的运行。 请确保你随时熟悉所有工具，以便当你处于光灯下时，可以感到自信。 如果活动有 (说话人/执行) 也将其包括在运行中。
* 避免最后一分钟更改。 在开始时间之前添加或重新排列事件设置的分钟数似乎很容易;但你可能被错误单击，无法进行中断性变更。 
* 不要忘记审核。 查看审查工具 (、报告、阻止、静音) ，分配审查器以帮助关注事件，与来宾共享事件规则。 请记住，不太了解 VR 的人可能并不总是知道虚拟集会的社交要求是什么。