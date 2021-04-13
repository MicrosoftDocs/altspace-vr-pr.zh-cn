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
# <a name="using-a-mixed-reality-extension"></a><span data-ttu-id="c9858-104">使用混合现实扩展</span><span class="sxs-lookup"><span data-stu-id="c9858-104">Using a Mixed Reality Extension</span></span>

<span data-ttu-id="c9858-105">[混合现实扩展](https://developer.altvr.com/) (MREs) 是可以在世界中将 [Helmets](https://account.altvr.com/mres/1173667287173955931) 用于工作 [Stargate](https://account.altvr.com/mres/1152987031857529562)的应用。</span><span class="sxs-lookup"><span data-stu-id="c9858-105">[Mixed Reality Extensions](https://developer.altvr.com/) (MREs) are apps you can use in your Worlds from [helmets](https://account.altvr.com/mres/1173667287173955931) to a working [Stargate](https://account.altvr.com/mres/1152987031857529562).</span></span> <span data-ttu-id="c9858-106">这就是具有编程经验的社区成员如何扩展 Altspace，而单向世界建筑者可以使其世界更加交互。</span><span class="sxs-lookup"><span data-stu-id="c9858-106">This is how community members with programming experience can extend Altspace and one-way World Builders can make their Worlds more interactive.</span></span> <span data-ttu-id="c9858-107">虽然世界上的任何人都可以使用 MREs，但只有世界大楼计划的人员才能浏览和生成 MREs。</span><span class="sxs-lookup"><span data-stu-id="c9858-107">While MREs can be used by anyone in a World, only people in the World Building Program can browse and spawn MREs in their Worlds.</span></span> 

1. <span data-ttu-id="c9858-108">浏览 [网站](https://account.altvr.com/mres)的 MRE 部分。</span><span class="sxs-lookup"><span data-stu-id="c9858-108">Browse the MRE section of our [website](https://account.altvr.com/mres).</span></span> <span data-ttu-id="c9858-109">默认情况下，你会看到你自己的 MREs，因此请选择 " **Altspace** " 以查看官方 MREs 和 **特色** ，以查看来自社区的 MREs。</span><span class="sxs-lookup"><span data-stu-id="c9858-109">By default you'll see your own MREs so select on **Altspace** to see official MREs and **Featured** to see MREs from the community.</span></span> <span data-ttu-id="c9858-110">在世界范围内使用之前，先熟悉所有 MRE。</span><span class="sxs-lookup"><span data-stu-id="c9858-110">Get familiar with any MRE before you use it in your World.</span></span> 
2. <span data-ttu-id="c9858-111">导航到 [Helmets](https://account.altvr.com/mres/1173667287173955931) MRE，并选择 " **复制到剪贴板**"。</span><span class="sxs-lookup"><span data-stu-id="c9858-111">Navigate to the [Helmets](https://account.altvr.com/mres/1173667287173955931) MRE and select **Copy to Clipboard**.</span></span> 
3. <span data-ttu-id="c9858-112">进入你的世界，并打开世界编辑 **> SDK 应用的基本知识**。</span><span class="sxs-lookup"><span data-stu-id="c9858-112">Enter your World and open the World Editor to **Basics > SDK App**.</span></span> <span data-ttu-id="c9858-113">将 Helmets 的 URL 粘贴到 "目标 URI" 字段中，然后选择 " **确认**"。</span><span class="sxs-lookup"><span data-stu-id="c9858-113">Paste in the URL for Helmets into the Target URI field and select **Confirm**.</span></span> <span data-ttu-id="c9858-114">应显示 MRE 对象，并尝试连接到在云中运行的 MRE。</span><span class="sxs-lookup"><span data-stu-id="c9858-114">The MRE Object should appear and attempt to connect to the MRE that's running in the cloud.</span></span> <span data-ttu-id="c9858-115">现在，你应该会看到一些 helmets，你可以单击它。</span><span class="sxs-lookup"><span data-stu-id="c9858-115">You should now see some helmets you can click on.</span></span>
4. <span data-ttu-id="c9858-116">移动/旋转/缩放 MRE，就像处理任何其他世界对象一样。</span><span class="sxs-lookup"><span data-stu-id="c9858-116">Move/rotate/scale the MRE just as you would any other World Object.</span></span>

<span data-ttu-id="c9858-117">恭喜！</span><span class="sxs-lookup"><span data-stu-id="c9858-117">Congratulations!</span></span> <span data-ttu-id="c9858-118">现在正在使用 MREs--非常酷！</span><span class="sxs-lookup"><span data-stu-id="c9858-118">You're using MREs now--you're so cool!</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="c9858-119">疑难解答</span><span class="sxs-lookup"><span data-stu-id="c9858-119">Troubleshooting</span></span>

<span data-ttu-id="c9858-120">**MRE 显示了一个哭表情符号**</span><span class="sxs-lookup"><span data-stu-id="c9858-120">**MRE is showing a frowning emoji**</span></span> 
    * <span data-ttu-id="c9858-121">请验证 URL 是否正确</span><span class="sxs-lookup"><span data-stu-id="c9858-121">Verify that the URL is correct</span></span>
    * <span data-ttu-id="c9858-122">对象上的 "切换 **正在播放**" 选项，然后选择 "**确认**"</span><span class="sxs-lookup"><span data-stu-id="c9858-122">Toggle **Is Playing** option on the Object and choose **confirm**</span></span>
    * <span data-ttu-id="c9858-123">尝试重新进入</span><span class="sxs-lookup"><span data-stu-id="c9858-123">Try reentering</span></span>

<span data-ttu-id="c9858-124">**MRE 为滞后** 根据 MRE 的托管位置，可能会遇到某些网络延迟</span><span class="sxs-lookup"><span data-stu-id="c9858-124">**MRE is lagging** Depending on where an MRE is hosted you may experience some network latency</span></span>

<span data-ttu-id="c9858-125">**为什么必须粘贴 Url？**</span><span class="sxs-lookup"><span data-stu-id="c9858-125">**Why do we have to paste URLs?**</span></span>
<span data-ttu-id="c9858-126">将来，您可以管理和生成 MREs，就像从工具包中进行项目一样。</span><span class="sxs-lookup"><span data-stu-id="c9858-126">In the future, you can manage and spawn MREs like you do Artifacts from Kits.</span></span> <span data-ttu-id="c9858-127">到现在为止，我们将继续使用 Url</span><span class="sxs-lookup"><span data-stu-id="c9858-127">Until then, we'll continue using URLs</span></span>