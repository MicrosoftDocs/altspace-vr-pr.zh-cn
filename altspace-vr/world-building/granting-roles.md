---
title: 授予全局角色
description: 了解角色和能力系统，并获取在 AltspaceVR 世界中提供用户角色的分步说明。
ms.date: 04/14/2021
ms.topic: article
keywords: 角色
ms.openlocfilehash: 3a1d0f138b29fe545f52d851ff00062f156a860e
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/25/2021
ms.locfileid: "112923186"
---
# <a name="granting-world-roles"></a><span data-ttu-id="b8180-104">授予全局角色</span><span class="sxs-lookup"><span data-stu-id="b8180-104">Granting world roles</span></span>

<span data-ttu-id="b8180-105">Altspace 具有角色和功能系统。</span><span class="sxs-lookup"><span data-stu-id="b8180-105">Altspace has a Roles and Abilities system.</span></span> <span data-ttu-id="b8180-106">每个用户都可以拥有多个角色，并且其角色可能会不同，具体取决于它们所在的位置。</span><span class="sxs-lookup"><span data-stu-id="b8180-106">Each person can have multiple roles and their roles can be different depending on where they are.</span></span> <span data-ttu-id="b8180-107">反过来，每个角色都提供了一个或多个功能。</span><span class="sxs-lookup"><span data-stu-id="b8180-107">Each role, in turn, gives you one or more abilities.</span></span> <span data-ttu-id="b8180-108">例如，当你在自己的活动中时，会自动接收 **主机** 和 **仲裁** 者角色。</span><span class="sxs-lookup"><span data-stu-id="b8180-108">For example, when you're in your own event, you automatically receive the **host** and **moderator** roles.</span></span> <span data-ttu-id="b8180-109">对于这两个角色，您可以启动循用户，也可以在阶段发布，也可以发布纸屑。</span><span class="sxs-lookup"><span data-stu-id="b8180-109">With those two roles you can kick unruly users, be on stage, and maybe release the confetti.</span></span>

1. <span data-ttu-id="b8180-110">编辑您的世界，查看 **上下文角色** 的右侧专栏 ([如何管理世界](managing-worlds.md)) </span><span class="sxs-lookup"><span data-stu-id="b8180-110">Edit your World and look over to the right column for **Contextual Roles** ([How to manage Worlds](managing-worlds.md))</span></span>

![在世界的上下文角色部分更改角色](images/granting-roles.png)

2. <span data-ttu-id="b8180-112">如果要向特定用户授予特定的角色，请在 "**上下文角色**" 字段下单击 "**添加用户**"。</span><span class="sxs-lookup"><span data-stu-id="b8180-112">Click **Add User** under the **Contextual Roles** field if you want to grant specific roles to specific users just for this World.</span></span> <span data-ttu-id="b8180-113">例如，如果想要向我提供 **主机**  +  **仲裁** 者，请添加上述并选择 "**保存**"。</span><span class="sxs-lookup"><span data-stu-id="b8180-113">For example, if you want to give me **host** + **moderator**, you would add the above and select **Save**.</span></span> <span data-ttu-id="b8180-114">格式为 **用户名**，用户名不区分大小写，请从下拉菜单中选择 " **Terraformer**" 角色，单击 "多次添加用户" 以保持添加更多用户，然后单击 " **更新**"。</span><span class="sxs-lookup"><span data-stu-id="b8180-114">The format is **username**, username is case-insensitive, choose the role from the dropdown menu **Terraformer**, click Add User multiple times to keeping adding more users and then click **Update**.</span></span>

* <span data-ttu-id="b8180-115">为了使更改在 Altspace 中生效，你应该重置世界上强制每个人重新加入的空间，或使每个用户具有新的角色重新加入世界。</span><span class="sxs-lookup"><span data-stu-id="b8180-115">In order for the change to take effect in Altspace, you should Reset Space the world forcing everyone to rejoin or have each user with a new role rejoin the world.</span></span>

3. <span data-ttu-id="b8180-116">如果要向加入你的世界的每一个角色授予角色，请在 "**在 VR** " 部分下编辑 "**默认上下文角色**" 字段。</span><span class="sxs-lookup"><span data-stu-id="b8180-116">Edit the **Default Contextual Roles** field, under the **In VR** section, if you want to grant a role to every one that joins your World.</span></span> <span data-ttu-id="b8180-117">例如，如果您想让人们飞入并使用扩音器，使其在很大程度上彼此听，请添加以下内容：</span><span class="sxs-lookup"><span data-stu-id="b8180-117">For example, if you want to let people fly and use the megaphone so they can hear each other while far part, add the following:</span></span>

```
pilot,megaphone_only
```

<span data-ttu-id="b8180-118">选择 " **更新**" 后，重置世界空间。</span><span class="sxs-lookup"><span data-stu-id="b8180-118">After you select **Update**, Reset Space in the World.</span></span> <span data-ttu-id="b8180-119">这只会影响这种情况。</span><span class="sxs-lookup"><span data-stu-id="b8180-119">This will only affect this World.</span></span> <span data-ttu-id="b8180-120">如果要将角色授予整个 Universe，请在 Universe 上编辑相同的字段。</span><span class="sxs-lookup"><span data-stu-id="b8180-120">If you want to grant roles to an entire Universe, edit the same fields on the Universe.</span></span> <span data-ttu-id="b8180-121">事件的相同之处是，如果你希望事件中的每个人都有这些角色，则需要将其添加到事件本身的 **默认 Contexual 角色** 。</span><span class="sxs-lookup"><span data-stu-id="b8180-121">The same goes for events, if you want everyone in your event to have these roles you'll need to add this to the **Default Contexual Roles** of the event itself.</span></span>

## <a name="roles"></a><span data-ttu-id="b8180-122">角色</span><span class="sxs-lookup"><span data-stu-id="b8180-122">Roles</span></span>

* <span data-ttu-id="b8180-123">**Megaphone_only** 能够在世界各地的任何位置对用户的耳进行对话</span><span class="sxs-lookup"><span data-stu-id="b8180-123">**Megaphone_only** - ability to speak into users' ears wherever they are in the World</span></span>
* <span data-ttu-id="b8180-124">**版主** 功能 **，如开始** 维护 decorum</span><span class="sxs-lookup"><span data-stu-id="b8180-124">**Moderator** - abilities like **kick** to maintain decorum</span></span>
* <span data-ttu-id="b8180-125">**试点** 功能-切换动态模式并生成6DOF 航班工具</span><span class="sxs-lookup"><span data-stu-id="b8180-125">**Pilot** - ability to toggle fly mode and spawn the 6DOF flight tool</span></span>
* <span data-ttu-id="b8180-126">**主机** 功能，如可以在阶段，扩音器</span><span class="sxs-lookup"><span data-stu-id="b8180-126">**Host** - abilities like being able to be on stage, have megaphone</span></span>
* <span data-ttu-id="b8180-127">**Terraformer** -可以使用世界编辑器 ([事件、世界、组和 AltspaceVR 中的角色](../getting-started/roles.md) 的详细信息) </span><span class="sxs-lookup"><span data-stu-id="b8180-127">**Terraformer** - ability to use the World Editor More information about ([Roles in events, worlds, groups, and in AltspaceVR](../getting-started/roles.md))</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="b8180-128">疑难解答</span><span class="sxs-lookup"><span data-stu-id="b8180-128">Troubleshooting</span></span>

<span data-ttu-id="b8180-129">**能否删除角色？**</span><span class="sxs-lookup"><span data-stu-id="b8180-129">**Can I delete roles?**</span></span>
<span data-ttu-id="b8180-130">是，编辑你的世界，单击你想要删除的角色下方的 "**删除**"，然后单击 "**更新**"</span><span class="sxs-lookup"><span data-stu-id="b8180-130">Yes, edit your world, click **Remove** below the role you'd like to delete and click **Update**</span></span>

<span data-ttu-id="b8180-131">**如果是从另一个领域导入，则会复制角色？**</span><span class="sxs-lookup"><span data-stu-id="b8180-131">**Are roles copied when a World is importing from another?**</span></span>
<span data-ttu-id="b8180-132">否，不复制角色</span><span class="sxs-lookup"><span data-stu-id="b8180-132">No, roles aren't copied</span></span>