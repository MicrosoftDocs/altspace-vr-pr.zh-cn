---
title: 查找 AltspaceVR 应用版本
description: 了解如何使用 AltspaceVR 应用、设置和客户端日志查找当前正在运行的 AltspaceVR 版本。
ms.date: 02/10/2021
ms.topic: article
keywords: 应用版本
ms.openlocfilehash: 6b710e1724b890fa7ba0eecfcd774ef63128d5b7
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/25/2021
ms.locfileid: "112923174"
---
# <a name="finding-the-altspacevr-app-version"></a><span data-ttu-id="66882-104">查找 AltspaceVR 应用版本</span><span class="sxs-lookup"><span data-stu-id="66882-104">Finding the AltspaceVR app version</span></span>

<span data-ttu-id="66882-105">在排查问题时，可能会询问你当前运行的 AltspaceVR 应用的版本。</span><span class="sxs-lookup"><span data-stu-id="66882-105">In the course of troubleshooting an issue, you may be asked what version of the AltspaceVR app you're currently running.</span></span>

## <a name="in-altspacevr"></a><span data-ttu-id="66882-106">在 AltspaceVR 中</span><span class="sxs-lookup"><span data-stu-id="66882-106">In AltspaceVR</span></span>

<span data-ttu-id="66882-107">若要在 AltspaceVR 中查找应用版本，请导航到设置 **菜单，然后选择\*\*\*\*左侧导航栏中** 的"关于"。</span><span class="sxs-lookup"><span data-stu-id="66882-107">To find the app version in AltspaceVR, navigate to the **settings menu** and select **About** in the left navigation bar.</span></span> <span data-ttu-id="66882-108">此处报告"应用版本"，如以下屏幕截图所示。</span><span class="sxs-lookup"><span data-stu-id="66882-108">The 'App Version' is reported here, as shown in the screenshot below.</span></span>

![打开"设置"菜单，并打开"关于"面板](images/app-version-img-01.png)

## <a name="in-windows-system-settings"></a><span data-ttu-id="66882-110">在 Windows 系统设置中</span><span class="sxs-lookup"><span data-stu-id="66882-110">In Windows System Settings</span></span>

<span data-ttu-id="66882-111">如果通过 windows 系统设置Microsoft Store AltspaceVR，还可以在 Windows 系统设置中查找应用版本。</span><span class="sxs-lookup"><span data-stu-id="66882-111">If you installed AltspaceVR via the Microsoft Store, you can additionally find the app version in the Windows system settings.</span></span>  <span data-ttu-id="66882-112">如果无法成功登录到客户端，则报告应用版本时，此方案非常合适。</span><span class="sxs-lookup"><span data-stu-id="66882-112">This scenario is a good fit when reporting the app version if you're unable to successfully log into the client.</span></span>

<span data-ttu-id="66882-113">若要在 Windows 系统设置中查找应用版本，请打开"开始"菜单，键入"应用 **&功能**"，然后选择结果。</span><span class="sxs-lookup"><span data-stu-id="66882-113">To find the app version in Windows system settings, open the **Start Menu**, type in **Apps & Features**, and select the result.</span></span> <span data-ttu-id="66882-114">导航到 **应用列表中的 AltspaceVR。**</span><span class="sxs-lookup"><span data-stu-id="66882-114">Navigate to **AltspaceVR** in the list of apps.</span></span> <span data-ttu-id="66882-115">左键单击 AltspaceVR，然后 **从出现的** 菜单中选择"高级选项"。</span><span class="sxs-lookup"><span data-stu-id="66882-115">Left-click AltspaceVR and select **Advanced Options** from the menu that appears.</span></span>

!["应用和功能"菜单打开，突出显示了高级选项](images/app-version-img-02.png)

<span data-ttu-id="66882-117">在 **"高级选项"** 的"**规范"** 标头下，"版本"标签右侧应列出"应用 **版本**"。 </span><span class="sxs-lookup"><span data-stu-id="66882-117">In the **Advanced Options**, under the **Specifications** header, the **App Version** should be listed to the right of the **Version** label.</span></span>

![打开高级选项，并突出显示应用版本](images/app-version-img-03.png)

## <a name="in-client-logs"></a><span data-ttu-id="66882-119">在客户端日志中</span><span class="sxs-lookup"><span data-stu-id="66882-119">In Client Logs</span></span>

<span data-ttu-id="66882-120">AltspaceVR 在应用程序启动期间将客户端日志文件中的应用版本报告为"Altspace 版本"。</span><span class="sxs-lookup"><span data-stu-id="66882-120">AltspaceVR reports the app version in the client logs file as "Altspace Version" during application startup.</span></span> <span data-ttu-id="66882-121">如果无法成功登录到客户端，但尝试在失败之前启动，则这是获取应用版本的一个不错的选择。</span><span class="sxs-lookup"><span data-stu-id="66882-121">This would be a good option to get the app version if you can't successfully log into the client, but it did attempt to start before failing.</span></span>

## <a name="windows"></a><span data-ttu-id="66882-122">Windows</span><span class="sxs-lookup"><span data-stu-id="66882-122">Windows</span></span>

<span data-ttu-id="66882-123">在 Windows 上，可以通过以下位置找到客户端Windows 资源管理器文件：</span><span class="sxs-lookup"><span data-stu-id="66882-123">On Windows, the client logs file can be found via Windows Explorer at:</span></span>

```
%userprofile%\AppData\LocalLow\Microsoft\AltspaceVR\Player.log
%userprofile%\AppData\LocalLow\Microsoft\AltspaceVR\Player-prev.log
```

<span data-ttu-id="66882-124">每次启动 AltspaceVR 时，此文件将被覆盖。</span><span class="sxs-lookup"><span data-stu-id="66882-124">This file is overwritten each time you launch AltspaceVR.</span></span> <span data-ttu-id="66882-125">"Player.log"表示最新会话，"Player-prev.log"表示上一个会话。</span><span class="sxs-lookup"><span data-stu-id="66882-125">'Player.log' represents your latest session, and 'Player-prev.log' represents the previous session.</span></span>

## <a name="via-powershell"></a><span data-ttu-id="66882-126">通过 PowerShell</span><span class="sxs-lookup"><span data-stu-id="66882-126">Via PowerShell</span></span>

<span data-ttu-id="66882-127">高级用户可以通过 PowerShell 在客户端日志中搜索此字符串，如下所示：</span><span class="sxs-lookup"><span data-stu-id="66882-127">Advanced users can search the client logs for this string via PowerShell as follows:</span></span>

<span data-ttu-id="66882-128">输入：</span><span class="sxs-lookup"><span data-stu-id="66882-128">Input:</span></span>

```
gc $env:userprofile\appdata\locallow\altspacevr\altspacevr\Player.log | ? { $_ -match "Altspace Version" }
```

<span data-ttu-id="66882-129">输出：</span><span class="sxs-lookup"><span data-stu-id="66882-129">Output:</span></span>

<span data-ttu-id="66882-130">[2.047] AltspaceVR 版本：3.2.23.e66c2</span><span class="sxs-lookup"><span data-stu-id="66882-130">[2.047] AltspaceVR Version: 3.2.23.e66c2</span></span>