---
title: 查找 AltspaceVR 应用版本
description: 了解如何使用 AltspaceVR 应用、设置和客户端日志查找当前正在运行的 AltspaceVR 的版本。
ms.date: 02/10/2021
ms.topic: article
keywords: 应用版本
ms.openlocfilehash: 5d503d3b89cd213696dd53616c5c7e3013aeef01
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212002"
---
# <a name="finding-the-altspacevr-app-version"></a><span data-ttu-id="1b38b-104">查找 AltspaceVR 应用版本</span><span class="sxs-lookup"><span data-stu-id="1b38b-104">Finding the AltspaceVR app version</span></span>

<span data-ttu-id="1b38b-105">在对问题进行故障排除的过程中，可能会询问你当前正在运行的 AltspaceVR 应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="1b38b-105">In the course of troubleshooting an issue, you may be asked what version of the AltspaceVR app you're currently running.</span></span>

## <a name="in-altspacevr"></a><span data-ttu-id="1b38b-106">在 AltspaceVR 中</span><span class="sxs-lookup"><span data-stu-id="1b38b-106">In AltspaceVR</span></span>

<span data-ttu-id="1b38b-107">若要在 AltspaceVR 中查找应用版本，请导航到 " **设置" 菜单** ，然后在左侧导航栏中选择 " **关于** "。</span><span class="sxs-lookup"><span data-stu-id="1b38b-107">To find the app version in AltspaceVR, navigate to the **settings menu** and select **About** in the left navigation bar.</span></span> <span data-ttu-id="1b38b-108">此处报告了 "应用版本"，如下面的屏幕截图中所示。</span><span class="sxs-lookup"><span data-stu-id="1b38b-108">The 'App Version' is reported here, as shown in the screenshot below.</span></span>

!["设置" 菜单打开，并打开 "关于面板"](images/app-version-img-01.png)

## <a name="in-windows-system-settings"></a><span data-ttu-id="1b38b-110">在 Windows 系统设置中</span><span class="sxs-lookup"><span data-stu-id="1b38b-110">In Windows System Settings</span></span>

<span data-ttu-id="1b38b-111">如果通过 Microsoft Store 安装了 AltspaceVR，则还可以在 Windows 系统设置中查找应用版本。</span><span class="sxs-lookup"><span data-stu-id="1b38b-111">If you installed AltspaceVR via the Microsoft Store, you can additionally find the app version in the Windows system settings.</span></span>  <span data-ttu-id="1b38b-112">如果无法成功登录到客户端，则此方案适用于报告应用程序版本。</span><span class="sxs-lookup"><span data-stu-id="1b38b-112">This scenario is a good fit when reporting the app version if you're unable to successfully log into the client.</span></span>

<span data-ttu-id="1b38b-113">若要在 Windows 系统设置中查找应用版本，请打开 " **开始" 菜单**，在 " **应用 & 功能**" 中输入，然后选择结果。</span><span class="sxs-lookup"><span data-stu-id="1b38b-113">To find the app version in Windows system settings, open the **Start Menu**, type in **Apps & Features**, and select the result.</span></span> <span data-ttu-id="1b38b-114">在应用列表中导航到 **AltspaceVR** 。</span><span class="sxs-lookup"><span data-stu-id="1b38b-114">Navigate to **AltspaceVR** in the list of apps.</span></span> <span data-ttu-id="1b38b-115">左键单击 "AltspaceVR"，然后从出现的菜单中选择 " **高级选项** "。</span><span class="sxs-lookup"><span data-stu-id="1b38b-115">Left-click AltspaceVR and select **Advanced Options** from the menu that appears.</span></span>

![突出显示了 "高级" 选项的 "应用和功能" 菜单](images/app-version-img-02.png)

<span data-ttu-id="1b38b-117">在 "**规范**" 标头下的 "**高级选项**" 中，**应用版本** 应列在 "**版本**" 标签的右侧。</span><span class="sxs-lookup"><span data-stu-id="1b38b-117">In the **Advanced Options**, under the **Specifications** header, the **App Version** should be listed to the right of the **Version** label.</span></span>

![已突出显示应用版本的高级选项打开](images/app-version-img-03.png)

## <a name="in-client-logs"></a><span data-ttu-id="1b38b-119">在客户端日志中</span><span class="sxs-lookup"><span data-stu-id="1b38b-119">In Client Logs</span></span>

<span data-ttu-id="1b38b-120">在应用程序启动过程中，AltspaceVR 将客户端日志文件中的应用版本报告为 "Altspace 版本"。</span><span class="sxs-lookup"><span data-stu-id="1b38b-120">AltspaceVR reports the app version in the client logs file as "Altspace Version" during application startup.</span></span> <span data-ttu-id="1b38b-121">如果无法成功登录到客户端，则这是获取应用程序版本的一个不错的选择，但它确实会在失败之前尝试启动。</span><span class="sxs-lookup"><span data-stu-id="1b38b-121">This would be a good option to get the app version if you can't successfully log into the client, but it did attempt to start before failing.</span></span>

## <a name="windows"></a><span data-ttu-id="1b38b-122">Windows</span><span class="sxs-lookup"><span data-stu-id="1b38b-122">Windows</span></span>

<span data-ttu-id="1b38b-123">在 Windows 上，可以通过 Windows 资源管理器找到客户端日志文件，网址为：</span><span class="sxs-lookup"><span data-stu-id="1b38b-123">On Windows, the client logs file can be found via Windows Explorer at:</span></span>

```
%userprofile%\appdata\locallow\altspacevr\altspacevr\Player.log
%userprofile%\appdata\locallow\altspacevr\altspacevr\Player-prev.log
```

<span data-ttu-id="1b38b-124">每次启动 AltspaceVR 时，都会覆盖此文件。</span><span class="sxs-lookup"><span data-stu-id="1b38b-124">This file is overwritten each time you launch AltspaceVR.</span></span> <span data-ttu-id="1b38b-125">"唱机" 代表最新的会话，"Player-prev" 表示上一个会话。</span><span class="sxs-lookup"><span data-stu-id="1b38b-125">'Player.log' represents your latest session, and 'Player-prev.log' represents the previous session.</span></span>

## <a name="via-powershell"></a><span data-ttu-id="1b38b-126">通过 PowerShell</span><span class="sxs-lookup"><span data-stu-id="1b38b-126">Via PowerShell</span></span>

<span data-ttu-id="1b38b-127">高级用户可以通过 PowerShell 搜索此字符串的客户端日志，如下所示：</span><span class="sxs-lookup"><span data-stu-id="1b38b-127">Advanced users can search the client logs for this string via PowerShell as follows:</span></span>

<span data-ttu-id="1b38b-128">输入：</span><span class="sxs-lookup"><span data-stu-id="1b38b-128">Input:</span></span>

```
gc $env:userprofile\appdata\locallow\altspacevr\altspacevr\Player.log | ? { $_ -match "Altspace Version" }
```

<span data-ttu-id="1b38b-129">输出：</span><span class="sxs-lookup"><span data-stu-id="1b38b-129">Output:</span></span>

<span data-ttu-id="1b38b-130">[2.047] AltspaceVR 版本： 3.2.23. e66c2</span><span class="sxs-lookup"><span data-stu-id="1b38b-130">[2.047] AltspaceVR Version: 3.2.23.e66c2</span></span>