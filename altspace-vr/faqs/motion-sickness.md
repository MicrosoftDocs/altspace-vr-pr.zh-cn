---
title: AltspaceVR 会导致运动 sickness 吗？
description: 随时了解最新的最新常见问题，以及在 VR 环境中 sickness 的解决方案。
ms.date: 02/10/2021
ms.topic: article
keywords: 运动 sickness，vr，恶心
ms.openlocfilehash: 54f746bc2b213f011dbf94c2703ed039b4717d72
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212043"
---
# <a name="will-altspacevr-cause-motion-sickness"></a><span data-ttu-id="5fdfd-104">AltspaceVR 会导致运动 sickness 吗？</span><span class="sxs-lookup"><span data-stu-id="5fdfd-104">Will AltspaceVR cause motion sickness?</span></span>

## <a name="why-do-some-people-feel-ill-in-vr"></a><span data-ttu-id="5fdfd-105">为什么有些人在 VR 中感觉不正确？</span><span class="sxs-lookup"><span data-stu-id="5fdfd-105">Why do some people feel ill in VR?</span></span>

<span data-ttu-id="5fdfd-106">所有 VR 都会导致 vertigo 和恶心。</span><span class="sxs-lookup"><span data-stu-id="5fdfd-106">It's a popular belief that all VR causes vertigo and nausea.</span></span> <span data-ttu-id="5fdfd-107">此问题源于眼睛之间的差异，以及你的内部耳将发射到大脑的内容。</span><span class="sxs-lookup"><span data-stu-id="5fdfd-107">The problem stems from a discrepancy between what your eyes are seeing, and what your inner ear is transmitting to your brain.</span></span> <span data-ttu-id="5fdfd-108">当你的眼睛检测到你的引入，而你的耳传达你仍在进行交流时，一些人的大脑可能会通过眩晕和恶心做出反应。</span><span class="sxs-lookup"><span data-stu-id="5fdfd-108">When your eyes detect motion, and your ears communicate that you're standing still, some individuals' brain may react by inducing dizziness and nausea.</span></span> <span data-ttu-id="5fdfd-109">对于这种现象，更易受到运动 sickness 的用户可能更敏感，而其他人可能不会遇到问题。</span><span class="sxs-lookup"><span data-stu-id="5fdfd-109">Some people who are more susceptible to motion sickness may be more sensitive to this phenomenon, while others may not have an issue with it.</span></span> 

<span data-ttu-id="5fdfd-110">在硬件级别上完成了几项任务，一些功能在 AltspaceVR 的软件中，它在 VR 中大大减少或完全消除了恶心-引入运动。</span><span class="sxs-lookup"><span data-stu-id="5fdfd-110">There are several things that are done at the hardware level, and some in AltspaceVR's software that severely reduces or completely eliminate the nausea-inducing motion in VR.</span></span>

## <a name="hardware-based-nausea-reduction"></a><span data-ttu-id="5fdfd-111">Hardware-Based 恶心缩减</span><span class="sxs-lookup"><span data-stu-id="5fdfd-111">Hardware-Based Nausea Reduction</span></span>

<span data-ttu-id="5fdfd-112">现代型 VR 硬件，如 Oculus Rift 和 HTC Naopak，通过以消除可能导致恶心的延迟的速率呈现视频帧来减少运动 sickness。</span><span class="sxs-lookup"><span data-stu-id="5fdfd-112">Contemporary VR hardware like the Oculus Rift and HTC Vive, reduces motion sickness by presenting video frames at a rate that eliminates the latency that can cause nausea.</span></span> <span data-ttu-id="5fdfd-113">如果软件已经过优化，AltspaceVR 为，则在 VR 中打开 head 时，不会出现延迟。</span><span class="sxs-lookup"><span data-stu-id="5fdfd-113">If the software is optimized, as AltspaceVR is, then there's no perceived delay when you turn your head in VR.</span></span> <span data-ttu-id="5fdfd-114">HMD 中的加速感应器是通信移动，传输速度快于人们眼就能检测到任何滞后时间。</span><span class="sxs-lookup"><span data-stu-id="5fdfd-114">The accelerometers in the HMD are communicating movement and transmitting that telemetry faster than the human eye can detect any latency.</span></span> <span data-ttu-id="5fdfd-115">在具有位置照相机的 HMD 模型 outfitted 上，这会进一步进一步，而不仅表示旋转移动，因此，横向 (侧) 运动。</span><span class="sxs-lookup"><span data-stu-id="5fdfd-115">On HMD models outfitted with positional cameras, this goes a step further, not only is rotational movement represented, so is lateral (side to side) motion.</span></span>

## <a name="software-based-nausea-reduction"></a><span data-ttu-id="5fdfd-116">Software-Based 恶心缩减</span><span class="sxs-lookup"><span data-stu-id="5fdfd-116">Software-Based Nausea Reduction</span></span>

<span data-ttu-id="5fdfd-117">除了硬件改进和 framerates，AltspaceVR 还实现了一些功能，可帮助用户减少和消除恶心：</span><span class="sxs-lookup"><span data-stu-id="5fdfd-117">In addition to hardware improvements and framerates, AltspaceVR has implemented several features that help people reduce and eliminate nausea:</span></span>

* <span data-ttu-id="5fdfd-118">**Teleporting** -从点到点即时移动不会向大脑传达运动，从而消除运动 sickness。</span><span class="sxs-lookup"><span data-stu-id="5fdfd-118">**Teleporting** - Moving instantaneously from point-to-point doesn't communicate motion to the brain, thereby eliminating motion sickness.</span></span>
* <span data-ttu-id="5fdfd-119">**启用** 所有硬件的管理，AltspaceVR 提供了在 VR 中的视图的 "ratcheted" 或 "逐步" 旋转的方式。</span><span class="sxs-lookup"><span data-stu-id="5fdfd-119">**Snap Turning** - On all hardware, AltspaceVR provides means for "ratcheted" or "stepped" rotation of the view in VR.</span></span> <span data-ttu-id="5fdfd-120">换句话说，在打开时，视图将透视约20度的旋转。</span><span class="sxs-lookup"><span data-stu-id="5fdfd-120">In other words when turning, your view will pivot about 20 degrees of rotation.</span></span> <span data-ttu-id="5fdfd-121">同样，这并不会对大多数人触发恶心。</span><span class="sxs-lookup"><span data-stu-id="5fdfd-121">Again, this doesn't trigger nausea in most people.</span></span>
* <span data-ttu-id="5fdfd-122">**对齐动作** -在某些硬件上，触摸板上的向前轻扫会在不触发运动 sickness 的增量中向前移动透视。</span><span class="sxs-lookup"><span data-stu-id="5fdfd-122">**Snap Motion** - On certain hardware, swiping forward on the touchpad will move the perspective forward in an increment that doesn't trigger motion sickness.</span></span> 
 
## <a name="suggestions-for-eliminating-motion-sickness"></a><span data-ttu-id="5fdfd-123">消除运动 Sickness 的建议</span><span class="sxs-lookup"><span data-stu-id="5fdfd-123">Suggestions for Eliminating Motion Sickness</span></span>

<span data-ttu-id="5fdfd-124">**仍**</span><span class="sxs-lookup"><span data-stu-id="5fdfd-124">**Stand Still**</span></span>

<span data-ttu-id="5fdfd-125">不要使用控制器进行太多移动，只需旋转头/或向上/向下即可在 VR 中查找。</span><span class="sxs-lookup"><span data-stu-id="5fdfd-125">Try not to move around too much using the controllers, just rotate your head/or up/down to look around in VR.</span></span>

<span data-ttu-id="5fdfd-126">**不要使用鼠标/KB 或控制器**</span><span class="sxs-lookup"><span data-stu-id="5fdfd-126">**Don't Use a Mouse/KB or Controller**</span></span>

<span data-ttu-id="5fdfd-127">AltspaceVR 为用户提供了使用标准游戏外围设备（如鼠标/键盘和游戏控制器）的选项，可像在视频游戏中那样移动到 VR。</span><span class="sxs-lookup"><span data-stu-id="5fdfd-127">AltspaceVR offers users the option to use standard gaming peripherals such as Mouse/Keyboard and Game controllers to move in VR as you would in a video game.</span></span> <span data-ttu-id="5fdfd-128">这包括多方向移动、strafing 和 turbo 按钮。</span><span class="sxs-lookup"><span data-stu-id="5fdfd-128">This includes multi-directional movement, strafing, and a turbo button.</span></span> <span data-ttu-id="5fdfd-129">建议仅在习惯于 VR 后使用这些项。</span><span class="sxs-lookup"><span data-stu-id="5fdfd-129">We recommend using these only after becoming accustomed to being in VR.</span></span> <span data-ttu-id="5fdfd-130">即使这样，也要慢一些。</span><span class="sxs-lookup"><span data-stu-id="5fdfd-130">Even then, take it slow.</span></span>

<span data-ttu-id="5fdfd-131">**您始终可以将**</span><span class="sxs-lookup"><span data-stu-id="5fdfd-131">**You Can Always Bail Out**</span></span>

<span data-ttu-id="5fdfd-132">如果遇到恶心，请立即删除 HMD。</span><span class="sxs-lookup"><span data-stu-id="5fdfd-132">If you experience nausea, remove your HMD immediately.</span></span> <span data-ttu-id="5fdfd-133">重新获得你的平衡，冷静你的 stomach，并在准备好返回到 VR 环境时。</span><span class="sxs-lookup"><span data-stu-id="5fdfd-133">Regain your equilibrium, calm your stomach, and when ready return to the VR environment.</span></span> <span data-ttu-id="5fdfd-134">请尝试记住导致成名的移动，并避免重复它。</span><span class="sxs-lookup"><span data-stu-id="5fdfd-134">Try to remember the movement that caused the sensation and refrain from repeating it.</span></span>

<span data-ttu-id="5fdfd-135">**知道何时需要退出 VR**</span><span class="sxs-lookup"><span data-stu-id="5fdfd-135">**Know When it's Time to Exit VR**</span></span>

<span data-ttu-id="5fdfd-136">最重要的是，知道何时需要休息时间。</span><span class="sxs-lookup"><span data-stu-id="5fdfd-136">Most importantly, know when it's time to take a break.</span></span> <span data-ttu-id="5fdfd-137">您知道您的身体，当它为您提供了一些很好的迹象时，请倾听。</span><span class="sxs-lookup"><span data-stu-id="5fdfd-137">You know your body, and when it's giving you strong indication that something is wrong, listen.</span></span> <span data-ttu-id="5fdfd-138">休息一下，看看一些气流。</span><span class="sxs-lookup"><span data-stu-id="5fdfd-138">Take a break and get some air.</span></span> <span data-ttu-id="5fdfd-139">浏览并重新对齐你的平衡。</span><span class="sxs-lookup"><span data-stu-id="5fdfd-139">Walk around and realign your equilibrium.</span></span> <span data-ttu-id="5fdfd-140">再次重申后，我们相信，这一方仍将继续工作！</span><span class="sxs-lookup"><span data-stu-id="5fdfd-140">Once you feel good again, come back, we're confident the party will still be going!</span></span>