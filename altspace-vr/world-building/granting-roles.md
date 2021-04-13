---
title: 授予全局角色
description: 了解角色和能力系统，并获取在 AltspaceVR 世界中提供用户角色的分步说明。
ms.date: 03/11/2021
ms.topic: article
keywords: 角色
ms.openlocfilehash: f8cd55fbd8ede6cedd199724a3e6b2413c5bc3e6
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2021
ms.locfileid: "107211917"
---
# <a name="granting-world-roles"></a>授予全局角色

Altspace 具有角色和功能系统。 每个用户都可以拥有多个角色，并且其角色可能会不同，具体取决于它们所在的位置。 反过来，每个角色都提供了一个或多个功能。 例如，当你在自己的活动中时，会自动接收表示器和 **仲裁****者** 角色。 对于这两个角色，您可以启动循用户，也可以在阶段发布，也可以发布纸屑。 

1. 编辑您的世界，并向下滚动到 "VR" 部分 **中** ([如何管理世界](managing-worlds.md)) 

![在世界的 VR 部分更改角色](images/granting-roles.png)

2. 如果要向特定用户授予特定的角色，请编辑 " **角色** " 字段。 例如，如果你想要向我提供显示 **者**  +  **审查** 并为 Calen **版主** 提供，请添加以下并选择 "**保存**"。 每行的格式为 **{role}、{username 或 email}** 。 用户名不区分大小写。 

```
presenter,jimmy
moderator,jimmy
moderator,calen
```

3. 如果再次选择 " **编辑** "，则 "角色" 字段上会显示以下各项。 这就是您在数据库中更新的知识。

```
Presenters: jimmy
Moderators: jimmy,calen
```

* 为了使更改在 Altspace 中生效，你应重置世界，并强制每个人重新加入。 下面是一个完整的角色列表。

4. 如果要向加入你的世界的每一个角色授予角色，请编辑 " **上下文角色** " 字段。 例如，如果您想让人们飞入并使用扩音器，使其在很大程度上彼此听，请添加以下内容：

```
pilot,megaphone_only
```

选择 " **更新**" 后，重置世界。 这只会影响这种情况。 如果要将角色授予整个 Universe，请在 Universe 上编辑相同的字段。 

## <a name="roles"></a>角色 

* **演示者** 功能，如能够在舞台上
* **版主** 功能 **，如开始** 维护 decorum
* **Terraformer** -能够使用世界编辑器
* **试点** 功能-切换动态模式并生成6DOF 航班工具
* **Megaphone_only** 能够在世界各地的任何位置对用户的耳进行对话
* **Showcase_new_sdk** 生成 MRE sdk 应用的能力

## <a name="troubleshooting"></a>疑难解答

**能否删除角色？**
不是从窗体开始，因此，请在 help.altvr.com 中记录支持请求

**如果是从另一个领域导入，则会复制角色？**
否，不复制角色