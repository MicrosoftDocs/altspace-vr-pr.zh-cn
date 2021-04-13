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
# <a name="using-the-interactables-spawner"></a><span data-ttu-id="1b907-104">使用 Interactables Spawner</span><span class="sxs-lookup"><span data-stu-id="1b907-104">Using the Interactables Spawner</span></span>

<span data-ttu-id="1b907-105">可以通过 Interactables Spawner 将种不可交互项放置在事件、世界或主空间中。</span><span class="sxs-lookup"><span data-stu-id="1b907-105">The Interactables Spawner allows you to place interactable items in your event, world, or home-space.</span></span> <span data-ttu-id="1b907-106">此功能当前是 [早期访问计划](../world-building/early-access.md) 的一部分，除非你已在主菜单中选择了，否则此功能将不可用。</span><span class="sxs-lookup"><span data-stu-id="1b907-106">This feature is currently part of our [Early Access Program](../world-building/early-access.md) and won't be available unless you've opted in through your Main Menu.</span></span>

> [!NOTE]
> <span data-ttu-id="1b907-107">尽管我们继续试点此功能，但请注意，生成太多 interactables 可能会影响环境或事件的性能。</span><span class="sxs-lookup"><span data-stu-id="1b907-107">While we continue to pilot this feature please be aware that spawning too many interactables may affect the performance of your environment or event.</span></span> 

## <a name="creating-an-interactable"></a><span data-ttu-id="1b907-108">创建种不可交互</span><span class="sxs-lookup"><span data-stu-id="1b907-108">Creating an interactable</span></span>

<span data-ttu-id="1b907-109">若要将对象转换为种不可交互对象，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="1b907-109">To turn your object into an interactable object:</span></span>

1. <span data-ttu-id="1b907-110">将对象放入空间。</span><span class="sxs-lookup"><span data-stu-id="1b907-110">Place the object in your space.</span></span>
2. <span data-ttu-id="1b907-111">然后，在 "对象" 列表中找到条目，然后选择它旁边的 **齿轮图标** 以打开其设置：</span><span class="sxs-lookup"><span data-stu-id="1b907-111">Then, find the entry in the object list, and select the **gear icon** next to it to open its settings:</span></span>

![显示突出显示对象列表的世界编辑器打开](images/interactables-spawner-img-01.png)

<span data-ttu-id="1b907-113">在 "设置" 页上，你将看到一个新的复选框 **"对象 spawner"**，它用于使其成为种不可交互对象。</span><span class="sxs-lookup"><span data-stu-id="1b907-113">On the settings page you’ll find a new checkbox **“Object spawner“**, which is used to make it an interactable object.</span></span>

1. <span data-ttu-id="1b907-114">选中此框，然后选择 " **确认**"。</span><span class="sxs-lookup"><span data-stu-id="1b907-114">Check the box and select **confirm**.</span></span>
2. <span data-ttu-id="1b907-115">在编辑模式下，可以在空间中的对象的生成位置周围移动。</span><span class="sxs-lookup"><span data-stu-id="1b907-115">While in edit mode, you can move around the object’s spawn location in the space.</span></span>
3. <span data-ttu-id="1b907-116">**退出编辑模式** 以启用项交互。</span><span class="sxs-lookup"><span data-stu-id="1b907-116">**Exit edit mode** to enable item interaction.</span></span>

![在 AltspaceVR 应用中打开 "更新项目" 窗口](images/interactables-spawner-img-02.png)

## <a name="other-customizations"></a><span data-ttu-id="1b907-118">其他自定义</span><span class="sxs-lookup"><span data-stu-id="1b907-118">Other customizations</span></span>

<span data-ttu-id="1b907-119">当你返回到该对象的属性后，启用 **"Object spawner"** 后，将有额外的设置可应用于生成的对象的行为方式。</span><span class="sxs-lookup"><span data-stu-id="1b907-119">After enabling **“Object spawner”** when you go back into the properties for that object, there will be an extra setting you can apply to how the spawned object behaves.</span></span>

> [!NOTE]
> <span data-ttu-id="1b907-120">种不可交互对象比例：这会在选取对象时设置对象的小数位数，而 "小数位数" 是指对象在世界上第一次选取之前的显示比例。</span><span class="sxs-lookup"><span data-stu-id="1b907-120">Interactable object scale: This sets the scale of the object when it gets picked up, compared to “Scale” which is the scale of how the object appears in the world prior to picking it up for the first time.</span></span>

<span data-ttu-id="1b907-121">包制造商可能会注意到，在 AltspaceVR 运行时对你的工具包所做的更改不会生效，直到你重新启动 AltspaceVR。</span><span class="sxs-lookup"><span data-stu-id="1b907-121">Kit makers may notice that changes to your Kit while AltspaceVR is running won't take effect until you restart AltspaceVR.</span></span>

<span data-ttu-id="1b907-122">最近，我们已在 " **中等设置** " 选项卡下添加一个名为 " **重新加载**" 的按钮。</span><span class="sxs-lookup"><span data-stu-id="1b907-122">Recently we’ve added a button under the **Moderate Settings** tab called **Reload Worlds Kits**.</span></span> <span data-ttu-id="1b907-123">单击此按钮将导致 (您) 重新输入空间，重新加载所有工具包，这将只下载在 AltspaceVR 时更新的工具包的新版本。</span><span class="sxs-lookup"><span data-stu-id="1b907-123">Clicking this button causes (just you) to reenter the space, reloading all Kits again, which will download only new versions of the Kits that have been updated while you were in AltspaceVR.</span></span>

![在 AltspaceVR 应用中打开适中的设置面板](images/interactables-spawner-img-03.png)