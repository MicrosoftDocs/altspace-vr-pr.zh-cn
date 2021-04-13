---
title: 备份世界
description: 了解如何创建、管理 AltspaceVR 的备份快照，并对其进行故障排除。
ms.date: 03/11/2021
ms.topic: article
keywords: 正在保存
ms.openlocfilehash: fdef692c737bf2f92db315e04556831d60c2f377
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2021
ms.locfileid: "107211737"
---
# <a name="backing-up-your-worlds"></a><span data-ttu-id="6ba50-104">备份世界</span><span class="sxs-lookup"><span data-stu-id="6ba50-104">Backing up your worlds</span></span>

<span data-ttu-id="6ba50-105">备份是世界上某个特定时间点的所有对象的 "快照" 或记录。</span><span class="sxs-lookup"><span data-stu-id="6ba50-105">A Backup is a “snapshot” or record of all the objects in a World at a specific point in time.</span></span> <span data-ttu-id="6ba50-106">假设你正在构建梦想房子，而你意外删除了客厅。</span><span class="sxs-lookup"><span data-stu-id="6ba50-106">Suppose you’re building your Dream House and one day you accidentally deleted the living room.</span></span> <span data-ttu-id="6ba50-107">如果你之前创建了世界的备份，则可以还原该特定备份、重置世界，并避免出现紧急攻击。</span><span class="sxs-lookup"><span data-stu-id="6ba50-107">If you had created a Backup of your World the day before, you could restore that particular backup, reset your World, and avoid a panic attack.</span></span> <span data-ttu-id="6ba50-108">也许您每个季节都有一个客舱的版本，并且想要在每个季节之间来回切换，您可以使用备份来实现这一目的。</span><span class="sxs-lookup"><span data-stu-id="6ba50-108">Or perhaps you have a version of your cabin-in-the-woods for every season and you like to switch back and forth between them—you can do that with Backups.</span></span> <span data-ttu-id="6ba50-109">每个备份都是特定于单个环境的，不仅包含转换 (位置、旋转、缩放) ，还包含对象上的其他设置。</span><span class="sxs-lookup"><span data-stu-id="6ba50-109">Each Backup is specific to a single World and contains not only the transforms (position, rotation, scale) but also other settings on the objects.</span></span> <span data-ttu-id="6ba50-110">对于可为世界创建的备份数量没有限制。</span><span class="sxs-lookup"><span data-stu-id="6ba50-110">There's no limit to the number of Backups you can create for a World.</span></span>  

## <a name="whats-included-in-a-backup"></a><span data-ttu-id="6ba50-111">备份中包含哪些内容？</span><span class="sxs-lookup"><span data-stu-id="6ba50-111">What’s included in a Backup?</span></span>

<span data-ttu-id="6ba50-112">当前，备份包括可以使用世界编辑器生成的大多数内容：</span><span class="sxs-lookup"><span data-stu-id="6ba50-112">A Backup currently includes most things you can spawn with the World Editor:</span></span>
* <span data-ttu-id="6ba50-113">项目 (工具包对象) </span><span class="sxs-lookup"><span data-stu-id="6ba50-113">Artifacts (Kit objects)</span></span>
* <span data-ttu-id="6ba50-114">标签</span><span class="sxs-lookup"><span data-stu-id="6ba50-114">Labels</span></span>
* <span data-ttu-id="6ba50-115">Teleporters</span><span class="sxs-lookup"><span data-stu-id="6ba50-115">Teleporters</span></span>
* <span data-ttu-id="6ba50-116">生成点</span><span class="sxs-lookup"><span data-stu-id="6ba50-116">Spawn Points</span></span>
* <span data-ttu-id="6ba50-117">照片</span><span class="sxs-lookup"><span data-stu-id="6ba50-117">Photos</span></span>
* <span data-ttu-id="6ba50-118">MRE SDK 应用</span><span class="sxs-lookup"><span data-stu-id="6ba50-118">MRE SDK Apps</span></span>
* <span data-ttu-id="6ba50-119">本机应用 (例如，针对现实的全息) </span><span class="sxs-lookup"><span data-stu-id="6ba50-119">Native Apps (for example, Holograms Against Reality)</span></span>

<span data-ttu-id="6ba50-120">不包括以下内容：</span><span class="sxs-lookup"><span data-stu-id="6ba50-120">The following isn’t included:</span></span>

* <span data-ttu-id="6ba50-121">布局重写</span><span class="sxs-lookup"><span data-stu-id="6ba50-121">Layout overrides</span></span>
* <span data-ttu-id="6ba50-122">Skyboxes 和环境声音</span><span class="sxs-lookup"><span data-stu-id="6ba50-122">Skyboxes and ambient sound</span></span>
* <span data-ttu-id="6ba50-123">模板</span><span class="sxs-lookup"><span data-stu-id="6ba50-123">Templates</span></span>
* <span data-ttu-id="6ba50-124">说明</span><span class="sxs-lookup"><span data-stu-id="6ba50-124">Instructions</span></span>
* <span data-ttu-id="6ba50-125">全局角色和上下文角色</span><span class="sxs-lookup"><span data-stu-id="6ba50-125">World roles and contextual roles</span></span>

## <a name="managing-backups"></a><span data-ttu-id="6ba50-126">管理备份</span><span class="sxs-lookup"><span data-stu-id="6ba50-126">Managing Backups</span></span>

<span data-ttu-id="6ba50-127">您可以通过打开您的世界编辑器/Altspace 并单击 "备份" 来创建备份。</span><span class="sxs-lookup"><span data-stu-id="6ba50-127">You can create a Backup by opening your World Editor / Altspace and clicking on “Backups”.</span></span> <span data-ttu-id="6ba50-128">第一个按钮将是 "新备份" 按钮。</span><span class="sxs-lookup"><span data-stu-id="6ba50-128">The first button will be the “New Backup” button.</span></span> <span data-ttu-id="6ba50-129">创建备份时，系统将要求你提供一个短名称。</span><span class="sxs-lookup"><span data-stu-id="6ba50-129">When creating a Backup, you’ll be asked to provide a short name.</span></span> <span data-ttu-id="6ba50-130">这是可选的，但强烈建议这样做，因为这会使速度变得更加容易。</span><span class="sxs-lookup"><span data-stu-id="6ba50-130">This is optional but highly recommended because it will get confusing fast.</span></span> <span data-ttu-id="6ba50-131">现有备份将在 "创建" 按钮的后面列出。</span><span class="sxs-lookup"><span data-stu-id="6ba50-131">Existing backups will be listed after the “Create” button.</span></span> <span data-ttu-id="6ba50-132">单击现有备份将启动还原。</span><span class="sxs-lookup"><span data-stu-id="6ba50-132">Clicking on an existing Backup will start a restore.</span></span> <span data-ttu-id="6ba50-133">还原备份时，你的环境将在几分钟后重置，但你可能看不到反映的更改。</span><span class="sxs-lookup"><span data-stu-id="6ba50-133">When restoring a Backup, your World will reset after a few moments but you may not see the changes reflected.</span></span> <span data-ttu-id="6ba50-134">请等待一两分钟，然后重新启动。</span><span class="sxs-lookup"><span data-stu-id="6ba50-134">Wait a minute or two and reset your World again.</span></span> <span data-ttu-id="6ba50-135">**目前没有任何方法可以在 VR 中编辑或删除备份**。</span><span class="sxs-lookup"><span data-stu-id="6ba50-135">**There's currently no way to edit or delete a Backup in VR**.</span></span> <span data-ttu-id="6ba50-136">你现在需要在我们的网站上管理你的备份。</span><span class="sxs-lookup"><span data-stu-id="6ba50-136">You'll need to manage your Backups on our website for now.</span></span> <span data-ttu-id="6ba50-137"> (在 VR 中进行的备份管理很快就会得到改进。</span><span class="sxs-lookup"><span data-stu-id="6ba50-137">(Backup management in VR will be improved soon.</span></span> <span data-ttu-id="6ba50-138">同时，我们) 。</span><span class="sxs-lookup"><span data-stu-id="6ba50-138">In the meantime, bear with us).</span></span>

<span data-ttu-id="6ba50-139">若要在我们的网站上管理你的备份：</span><span class="sxs-lookup"><span data-stu-id="6ba50-139">To manage your Backups on our website:</span></span>

1. <span data-ttu-id="6ba50-140">导航到 " [世界" > 地雷](https://account.altvr.com/users/sign_in)，找到你的世界，并按 "管理员" 控件中的 "备份"：</span><span class="sxs-lookup"><span data-stu-id="6ba50-140">Navigate to [Worlds > Mine](https://account.altvr.com/users/sign_in), find your World, and press “Backups” in the Administrator Controls:</span></span>

![通过 "备份" 面板打开的世界网站中的管理员控件](images/world-backup-img-01.png)

2. <span data-ttu-id="6ba50-142">你可以创建、编辑和删除备份，检查内部有多少对象，甚至上载预览图像：</span><span class="sxs-lookup"><span data-stu-id="6ba50-142">You can create, edit, and delete your Backups, check how many objects are inside, and even upload a preview image:</span></span> 

![突出显示 "创建"、"编辑" 和 "删除" 命令的 "备份" 窗口](images/world-backup-img-02.png)

<span data-ttu-id="6ba50-144">备份数没有限制，具有更多备份不会影响你的世界性能。</span><span class="sxs-lookup"><span data-stu-id="6ba50-144">There's no limit to the number of Backups and having more Backups won't impact the performance of your World.</span></span>

## <a name="other-ways-to-back-up-your-worlds"></a><span data-ttu-id="6ba50-145">备份世界的其他方法</span><span class="sxs-lookup"><span data-stu-id="6ba50-145">Other ways to back up your Worlds</span></span>

* <span data-ttu-id="6ba50-146">创建另一个世界，显示高级选项，并从世界导入。</span><span class="sxs-lookup"><span data-stu-id="6ba50-146">Create another World, Show Advanced Options, and Import from World.</span></span> <span data-ttu-id="6ba50-147">从下拉菜单中选择要备份的世界。</span><span class="sxs-lookup"><span data-stu-id="6ba50-147">Choose the World you want to back up from the dropdown menu into the new one.</span></span> <span data-ttu-id="6ba50-148">导入没有限制。</span><span class="sxs-lookup"><span data-stu-id="6ba50-148">There no limit for imports.</span></span>
* <span data-ttu-id="6ba50-149">如果你使用的是 Unity 上载者，我们强烈建议你使用版本控制。</span><span class="sxs-lookup"><span data-stu-id="6ba50-149">If you’re using the Unity Uploader, we strongly recommend you use version control.</span></span> <span data-ttu-id="6ba50-150">例如， [适用于 Unity 的 Github](https://unity.github.com)。</span><span class="sxs-lookup"><span data-stu-id="6ba50-150">For example, [Github for Unity](https://unity.github.com).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="6ba50-151">疑难解答</span><span class="sxs-lookup"><span data-stu-id="6ba50-151">Troubleshooting</span></span>

<span data-ttu-id="6ba50-152">**帮助！我意外还原了备份，** 无需担心。</span><span class="sxs-lookup"><span data-stu-id="6ba50-152">**Help! I accidentally restored a Backup and my work is gone** Don’t worry.</span></span> <span data-ttu-id="6ba50-153">我们会在还原旧备份之前自动创建一个新备份。</span><span class="sxs-lookup"><span data-stu-id="6ba50-153">We automatically create a new Backup before restoring old one.</span></span> <span data-ttu-id="6ba50-154">查找名称以 " **自动** " 开头为正确的时间戳的名称，并还原 (例如， **自动 2019-01-14T08：23： 33-08： 00**) 。</span><span class="sxs-lookup"><span data-stu-id="6ba50-154">Look for one with a name starting with **Auto** with the right timestamp and restore that one (for example, **Auto 2019-01-14T08:23:33-08:00**).</span></span>  <span data-ttu-id="6ba50-155">如果这不起作用，请提交 [支持请求](https://help.altvr.com/hc/requests/new)</span><span class="sxs-lookup"><span data-stu-id="6ba50-155">If that doesn’t work submit a [Support request](https://help.altvr.com/hc/requests/new)</span></span>

<span data-ttu-id="6ba50-156">**我还原了备份，但缺少某些对象** 如果有照片，这些照片是否被删除？</span><span class="sxs-lookup"><span data-stu-id="6ba50-156">**I restored a Backup and some objects are missing** If any were photos, were those photos deleted?</span></span> <span data-ttu-id="6ba50-157">由于隐私原因，无法还原已删除的照片。</span><span class="sxs-lookup"><span data-stu-id="6ba50-157">We can’t restore deleted photos for privacy reasons.</span></span> <span data-ttu-id="6ba50-158">提交 [支持请求](https://help.altvr.com/hc/requests/new) 以便调查</span><span class="sxs-lookup"><span data-stu-id="6ba50-158">Submit a [Support request](https://help.altvr.com/hc/requests/new) so we can investigate</span></span>

<span data-ttu-id="6ba50-159">**我看不到任何更改** 备份是异步还原的，这意味着可能需要几分钟的时间来还原，具体取决于对象的数量。</span><span class="sxs-lookup"><span data-stu-id="6ba50-159">**I don’t see any changes** Backups are restored asynchronously meaning they can take a few minutes to restore depending on the number of objects.</span></span> <span data-ttu-id="6ba50-160">请记住重置世界，如果在几分钟后看不到任何内容，请尝试再次重置。</span><span class="sxs-lookup"><span data-stu-id="6ba50-160">Remember to reset your World and if you don’t see anything after a few minutes try resetting again.</span></span> <span data-ttu-id="6ba50-161">将来，我们可以提供有关还原过程状态的更多反馈</span><span class="sxs-lookup"><span data-stu-id="6ba50-161">In the future, we can provide more feedback on the status of the restoration process</span></span>