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
# <a name="granting-world-roles"></a><span data-ttu-id="39979-104">授予全局角色</span><span class="sxs-lookup"><span data-stu-id="39979-104">Granting world roles</span></span>

<span data-ttu-id="39979-105">Altspace 具有角色和功能系统。</span><span class="sxs-lookup"><span data-stu-id="39979-105">Altspace has a Roles and Abilities system.</span></span> <span data-ttu-id="39979-106">每个用户都可以拥有多个角色，并且其角色可能会不同，具体取决于它们所在的位置。</span><span class="sxs-lookup"><span data-stu-id="39979-106">Each person can have multiple roles and their roles can be different depending on where they are.</span></span> <span data-ttu-id="39979-107">反过来，每个角色都提供了一个或多个功能。</span><span class="sxs-lookup"><span data-stu-id="39979-107">Each role, in turn, gives you one or more abilities.</span></span> <span data-ttu-id="39979-108">例如，当你在自己的活动中时，会自动接收表示器和 **仲裁\*\*\*\*者** 角色。</span><span class="sxs-lookup"><span data-stu-id="39979-108">For example, when you're in your own event, you automatically receive the **presenter** and **moderator** roles.</span></span> <span data-ttu-id="39979-109">对于这两个角色，您可以启动循用户，也可以在阶段发布，也可以发布纸屑。</span><span class="sxs-lookup"><span data-stu-id="39979-109">With those two roles you can kick unruly users, be on stage, and maybe release the confetti.</span></span> 

1. <span data-ttu-id="39979-110">编辑您的世界，并向下滚动到 "VR" 部分 **中** ([如何管理世界](managing-worlds.md)) </span><span class="sxs-lookup"><span data-stu-id="39979-110">Edit your World and scroll down to the **In VR** section ([How to manage Worlds](managing-worlds.md))</span></span>

![在世界的 VR 部分更改角色](images/granting-roles.png)

2. <span data-ttu-id="39979-112">如果要向特定用户授予特定的角色，请编辑 " **角色** " 字段。</span><span class="sxs-lookup"><span data-stu-id="39979-112">Edit the **Roles** field if you want to grant specific roles to specific users just for this World.</span></span> <span data-ttu-id="39979-113">例如，如果你想要向我提供显示 **者**  +  **审查** 并为 Calen **版主** 提供，请添加以下并选择 "**保存**"。</span><span class="sxs-lookup"><span data-stu-id="39979-113">For example, if you want to give me **presenter** + **moderator** and give Calen **moderator**, you would add the following and select **Save**.</span></span> <span data-ttu-id="39979-114">每行的格式为 **{role}、{username 或 email}** 。</span><span class="sxs-lookup"><span data-stu-id="39979-114">The format is **{role},{username or email}** on each line.</span></span> <span data-ttu-id="39979-115">用户名不区分大小写。</span><span class="sxs-lookup"><span data-stu-id="39979-115">Username is case-insensitive.</span></span> 

```
presenter,jimmy
moderator,jimmy
moderator,calen
```

3. <span data-ttu-id="39979-116">如果再次选择 " **编辑** "，则 "角色" 字段上会显示以下各项。</span><span class="sxs-lookup"><span data-stu-id="39979-116">If you select **Edit** again, you should see the following above the Roles field.</span></span> <span data-ttu-id="39979-117">这就是您在数据库中更新的知识。</span><span class="sxs-lookup"><span data-stu-id="39979-117">That's how you know updated in the database.</span></span>

```
Presenters: jimmy
Moderators: jimmy,calen
```

* <span data-ttu-id="39979-118">为了使更改在 Altspace 中生效，你应重置世界，并强制每个人重新加入。</span><span class="sxs-lookup"><span data-stu-id="39979-118">In order for the change to take effect in Altspace, you should reset the world, forcing everyone to rejoin.</span></span> <span data-ttu-id="39979-119">下面是一个完整的角色列表。</span><span class="sxs-lookup"><span data-stu-id="39979-119">There's a full list of roles below.</span></span>

4. <span data-ttu-id="39979-120">如果要向加入你的世界的每一个角色授予角色，请编辑 " **上下文角色** " 字段。</span><span class="sxs-lookup"><span data-stu-id="39979-120">Edit the **Contextual Roles** field if you want to grant a role to every one that joins your World.</span></span> <span data-ttu-id="39979-121">例如，如果您想让人们飞入并使用扩音器，使其在很大程度上彼此听，请添加以下内容：</span><span class="sxs-lookup"><span data-stu-id="39979-121">For example, if you want to let people fly and use the megaphone so they can hear each other while far part, add the following:</span></span>

```
pilot,megaphone_only
```

<span data-ttu-id="39979-122">选择 " **更新**" 后，重置世界。</span><span class="sxs-lookup"><span data-stu-id="39979-122">After you select **Update**, reset the World.</span></span> <span data-ttu-id="39979-123">这只会影响这种情况。</span><span class="sxs-lookup"><span data-stu-id="39979-123">This will only affect this World.</span></span> <span data-ttu-id="39979-124">如果要将角色授予整个 Universe，请在 Universe 上编辑相同的字段。</span><span class="sxs-lookup"><span data-stu-id="39979-124">If you want to grant roles to an entire Universe, edit the same fields on the Universe.</span></span> 

## <a name="roles"></a><span data-ttu-id="39979-125">角色</span><span class="sxs-lookup"><span data-stu-id="39979-125">Roles</span></span> 

* <span data-ttu-id="39979-126">**演示者** 功能，如能够在舞台上</span><span class="sxs-lookup"><span data-stu-id="39979-126">**Presenter** - abilities like being able to be on stage</span></span>
* <span data-ttu-id="39979-127">**版主** 功能 **，如开始** 维护 decorum</span><span class="sxs-lookup"><span data-stu-id="39979-127">**Moderator** - abilities like **kick** to maintain decorum</span></span>
* <span data-ttu-id="39979-128">**Terraformer** -能够使用世界编辑器</span><span class="sxs-lookup"><span data-stu-id="39979-128">**Terraformer** - ability to use the World Editor</span></span>
* <span data-ttu-id="39979-129">**试点** 功能-切换动态模式并生成6DOF 航班工具</span><span class="sxs-lookup"><span data-stu-id="39979-129">**Pilot** - ability to toggle fly mode and spawn the 6DOF flight tool</span></span>
* <span data-ttu-id="39979-130">**Megaphone_only** 能够在世界各地的任何位置对用户的耳进行对话</span><span class="sxs-lookup"><span data-stu-id="39979-130">**Megaphone_only** - ability to speak into users' ears wherever they are in the World</span></span>
* <span data-ttu-id="39979-131">**Showcase_new_sdk** 生成 MRE sdk 应用的能力</span><span class="sxs-lookup"><span data-stu-id="39979-131">**Showcase_new_sdk** - ability to spawn MRE SDK apps</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="39979-132">疑难解答</span><span class="sxs-lookup"><span data-stu-id="39979-132">Troubleshooting</span></span>

<span data-ttu-id="39979-133">**能否删除角色？**</span><span class="sxs-lookup"><span data-stu-id="39979-133">**Can I delete roles?**</span></span>
<span data-ttu-id="39979-134">不是从窗体开始，因此，请在 help.altvr.com 中记录支持请求</span><span class="sxs-lookup"><span data-stu-id="39979-134">Not from the form right now so file a Support request at help.altvr.com and we'll take care of it for you</span></span>

<span data-ttu-id="39979-135">**如果是从另一个领域导入，则会复制角色？**</span><span class="sxs-lookup"><span data-stu-id="39979-135">**Are roles copied when a World is importing from another?**</span></span>
<span data-ttu-id="39979-136">否，不复制角色</span><span class="sxs-lookup"><span data-stu-id="39979-136">No, roles aren't copied</span></span>