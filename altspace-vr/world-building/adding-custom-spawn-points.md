---
title: 添加自定义生成点
description: 了解如何创建自定义生成点，并将其添加到 AltspaceVR。
ms.date: 03/11/2021
ms.topic: article
keywords: spawnpoint，故障排除
ms.openlocfilehash: 0f53bdc229eb21e50edef34981c592556236fc55
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2021
ms.locfileid: "107211924"
---
# <a name="adding-custom-spawn-points"></a><span data-ttu-id="4af48-104">添加自定义生成点</span><span class="sxs-lookup"><span data-stu-id="4af48-104">Adding custom spawn points</span></span>

<span data-ttu-id="4af48-105">进入你的世界的人员将 **生成** 或显示在源位置， (0，0，0) ，当他们进入你的世界时。</span><span class="sxs-lookup"><span data-stu-id="4af48-105">People entering your World will **spawn** or appear at the origin, position (0,0,0), when they enter your World.</span></span> <span data-ttu-id="4af48-106">但是，如果想要让用户从城堡的入口开始，则可以添加一个或多个生成点。</span><span class="sxs-lookup"><span data-stu-id="4af48-106">However, you can add one or more Spawn Points if you want to, say, have people start at the entrance to your castle.</span></span> <span data-ttu-id="4af48-107">如果指定多个生成点，则每次输入时都会随机选择一个生成点，并且不会包含源。</span><span class="sxs-lookup"><span data-stu-id="4af48-107">If you specify multiple Spawn Points, one will be randomly chosen whenever someone enters and the origin won't be included.</span></span> <span data-ttu-id="4af48-108">您可以管理在其中启用了世界编辑器的任何世界或事件的生成点。</span><span class="sxs-lookup"><span data-stu-id="4af48-108">You can manage Spawn Points to any World or Event where your World Editor is enabled.</span></span> <span data-ttu-id="4af48-109">可以控制用户产生 (位置的位置) 以及 (旋转) 的方向。</span><span class="sxs-lookup"><span data-stu-id="4af48-109">You control where people spawn (position) and what direction they'll be facing (rotation).</span></span> <span data-ttu-id="4af48-110">生成点将仅在编辑模式下可见。</span><span class="sxs-lookup"><span data-stu-id="4af48-110">Spawn Points will only be visible in Edit Mode.</span></span> 

1. <span data-ttu-id="4af48-111">在希望用户产生的位置附近。</span><span class="sxs-lookup"><span data-stu-id="4af48-111">Go near the spot where you want people to spawn.</span></span> <span data-ttu-id="4af48-112">开放式 **世界编辑器 > 基础知识** ，并确保选中 **锁定旋转** 。</span><span class="sxs-lookup"><span data-stu-id="4af48-112">Open **World Editor > Basics** and make sure **Lock Rotation** is checked.</span></span> <span data-ttu-id="4af48-113">选择 " **衍生点** " 创建一个。</span><span class="sxs-lookup"><span data-stu-id="4af48-113">Select **Spawn Point** to create one.</span></span> <span data-ttu-id="4af48-114">将它移动到所需的确切位置：</span><span class="sxs-lookup"><span data-stu-id="4af48-114">Move it to the exact position you want:</span></span>

!["世界编辑器基础知识" 窗口打开](images/spawn-points-img-01.png)

2. <span data-ttu-id="4af48-116">选择 "生成点" 的 "设置" 图标，并确保 **旋转 > X** 和 **旋转 > Z** 均为 **0**。</span><span class="sxs-lookup"><span data-stu-id="4af48-116">Select on the settings icon for the Spawn Point and make sure **Rotation > X** and **Rotation > Z** are both **0**.</span></span> <span data-ttu-id="4af48-117">如果它们是较小的数字（如 **8.537777745**），则这也很好。</span><span class="sxs-lookup"><span data-stu-id="4af48-117">If they are small numbers like **8.537777745E-07**, that's fine too.</span></span> <span data-ttu-id="4af48-118">奇怪如何处理浮点数：</span><span class="sxs-lookup"><span data-stu-id="4af48-118">That's a quirk of how floating point numbers are handled:</span></span>

![更新世界编辑器设置中的生成点](images/spawn-points-img-02.png)

3. <span data-ttu-id="4af48-120">通过菜单 > 设置重新输入您的世界 **> 常规 > 重新输入空间 > 重新输入**</span><span class="sxs-lookup"><span data-stu-id="4af48-120">Reenter your World via **Menu > Settings > General > Reenter Space > Re-Enter**</span></span>
4. <span data-ttu-id="4af48-121">应该在新的衍生点上生成！</span><span class="sxs-lookup"><span data-stu-id="4af48-121">You should spawn at your new Spawn Point!</span></span>
5. <span data-ttu-id="4af48-122">如果希望用户面临不同方向，则选择 "生成点" 的设置，并将 "旋转" 设置为 "仅 **> Y** "。</span><span class="sxs-lookup"><span data-stu-id="4af48-122">If you want people to face a different direction, select the settings for the Spawn Point and set **Rotation > Y** only.</span></span> <span data-ttu-id="4af48-123">尝试将 Y 设置为180，X 和 Z 到 0 (警告： X 和 Z 是高级的，可能会让人病假) 。</span><span class="sxs-lookup"><span data-stu-id="4af48-123">Try setting Y to 180 and both X and Z to 0 (Warning: X and Z are advanced may make people sick).</span></span> <span data-ttu-id="4af48-124">然后选择 " **确认** "，然后重新输入世界。</span><span class="sxs-lookup"><span data-stu-id="4af48-124">Then select **Confirm** and reenter the World.</span></span> <span data-ttu-id="4af48-125">这会产生相反方向。</span><span class="sxs-lookup"><span data-stu-id="4af48-125">That should spawn you facing the opposite direction.</span></span> 

## <a name="troubleshooting"></a><span data-ttu-id="4af48-126">疑难解答</span><span class="sxs-lookup"><span data-stu-id="4af48-126">Troubleshooting</span></span>

<span data-ttu-id="4af48-127">**用户仍在源位置进行生成？**</span><span class="sxs-lookup"><span data-stu-id="4af48-127">**People still spawning at the origin?**</span></span>
    * <span data-ttu-id="4af48-128">请确保您的衍生点略高于地面或表面。</span><span class="sxs-lookup"><span data-stu-id="4af48-128">Make sure your Spawn Points are slightly above the ground or surface.</span></span> <span data-ttu-id="4af48-129">如果生成点与其他对象重叠，则用户将在默认位置（源）生成。</span><span class="sxs-lookup"><span data-stu-id="4af48-129">If the Spawn Point is overlapping other objects, people spawn at the default location, the origin.</span></span> <span data-ttu-id="4af48-130">如果对象内部的生成点和人员的高度不同，则会发生这种情况。</span><span class="sxs-lookup"><span data-stu-id="4af48-130">This can happen if the Spawn Point inside an object and the height of person varies.</span></span> 
    * <span data-ttu-id="4af48-131">尝试通过 **菜单 > 设置 > 适中 > 重置空间** 来重置世界</span><span class="sxs-lookup"><span data-stu-id="4af48-131">Try resetting your World via **Menu > Settings > Moderate > Reset Space**</span></span>

<span data-ttu-id="4af48-132">**有多个生成点，但仍在同一位置生成？**</span><span class="sxs-lookup"><span data-stu-id="4af48-132">**Have multiple Spawn Points but still spawning in the same place?**</span></span>
<span data-ttu-id="4af48-133">您可能会不幸--它是随机的。</span><span class="sxs-lookup"><span data-stu-id="4af48-133">You might be unlucky--it's random after all.</span></span> <span data-ttu-id="4af48-134">首先尝试多次重新进入5次，直到出现错误。</span><span class="sxs-lookup"><span data-stu-id="4af48-134">Try a few reentering at least five times before assuming there's an error.</span></span> 

<span data-ttu-id="4af48-135">**人们不舒服或其负责人为倾斜** 您可能忘记了检查 **锁定旋转** ，或设置了 X 和 Z 值进行旋转。</span><span class="sxs-lookup"><span data-stu-id="4af48-135">**People are uncomfortable or their head is tilted** You may have forgotten to check **Lock Rotation** or set the X and Z value for Rotation.</span></span> <span data-ttu-id="4af48-136">通常应将其设置为0，除非你要构建现。</span><span class="sxs-lookup"><span data-stu-id="4af48-136">Those should usually be set to 0 unless you're building an exotic World.</span></span> 

<span data-ttu-id="4af48-137">**用户何时产生呢？**</span><span class="sxs-lookup"><span data-stu-id="4af48-137">**People falling when they spawn?**</span></span>
<span data-ttu-id="4af48-138">不要将对象上的生成点位置设置得过高。</span><span class="sxs-lookup"><span data-stu-id="4af48-138">Don't set the Spawn Point position too high above an object.</span></span> <span data-ttu-id="4af48-139">如果它们太远，它们会在源位置 respawned。</span><span class="sxs-lookup"><span data-stu-id="4af48-139">If they fall too far, they'll be respawned at the origin.</span></span>