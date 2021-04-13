---
title: 使用多媒体控制台
description: 了解如何在 AltspaceVR 体验中开始配置、发布和 controling 多媒体控制台。
ms.date: 03/11/2021
ms.topic: article
keywords: 控制台，多媒体
ms.openlocfilehash: 601328eb6f266dbcfc9d81fc4f1c2d09ac62b318
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2021
ms.locfileid: "107211929"
---
# <a name="using-the-multimedia-console"></a><span data-ttu-id="cb410-104">使用多媒体控制台</span><span class="sxs-lookup"><span data-stu-id="cb410-104">Using the multimedia console</span></span>

<span data-ttu-id="cb410-105">多媒体控制台是一个工具，可用于在事件和世界中共享媒体。</span><span class="sxs-lookup"><span data-stu-id="cb410-105">The Multimedia Console is a tool that enables media sharing in events and worlds.</span></span> <span data-ttu-id="cb410-106">可以使用它来共享图像、演示文稿、livestreams、视频、播放列表等。</span><span class="sxs-lookup"><span data-stu-id="cb410-106">You can use it to share things like images, presentation slides, livestreams, videos, playlists, and more.</span></span> <span data-ttu-id="cb410-107">下面是有关如何使用多媒体控制台 **v 0.5.0 +** 的分步说明。</span><span class="sxs-lookup"><span data-stu-id="cb410-107">Below is a step-by-step instruction on how to use the Multimedia Console **v0.5.0+**.</span></span> 

## <a name="getting-started"></a><span data-ttu-id="cb410-108">入门</span><span class="sxs-lookup"><span data-stu-id="cb410-108">Getting started</span></span>

<span data-ttu-id="cb410-109">多媒体控制台入门是一个由两个部分组成的过程。</span><span class="sxs-lookup"><span data-stu-id="cb410-109">Getting started with the Multimedia Console is a two part process.</span></span>  <span data-ttu-id="cb410-110">首先，你将使用 web 门户为环境中放置的多媒体控制台会话生成和发布配置。</span><span class="sxs-lookup"><span data-stu-id="cb410-110">First there's the web portal that you'll use to generate and publish a configuration for the Multimedia Console session you place in your environment.</span></span>  <span data-ttu-id="cb410-111">其次是在您的环境中放置实际的多媒体控制台应用程序，并设置它应使用的配置代码。</span><span class="sxs-lookup"><span data-stu-id="cb410-111">Second is the placement of the actual Multimedia Console app in your environment and setting the configuration code it should use.</span></span>

### <a name="configuring-the-multimedia-console-with-the-web-portal"></a><span data-ttu-id="cb410-112">通过 web 门户配置多媒体控制台</span><span class="sxs-lookup"><span data-stu-id="cb410-112">Configuring the Multimedia console with the web portal</span></span>

1. <span data-ttu-id="cb410-113">首先，您需要确保您的内容已联机托管，因为您需要 URL。</span><span class="sxs-lookup"><span data-stu-id="cb410-113">First, you'll need to make sure your content is hosted online because you'll need a URL.</span></span> <span data-ttu-id="cb410-114"> (可以将照片上传到 altvr.com，或将视频文件联机或使用 Twitch 实时流链接： https://www.twitch.tv/ninja)</span><span class="sxs-lookup"><span data-stu-id="cb410-114">(You can upload photos to altvr.com, host a video .mp4 file online or use Twitch live stream link: https://www.twitch.tv/ninja)</span></span> 
2. <span data-ttu-id="cb410-115">导航到多媒体控制台的 web 门户，网址为： [https://multimedia-console.altvr.com/](https://multimedia-console.altvr.com/)</span><span class="sxs-lookup"><span data-stu-id="cb410-115">Navigate to the web portal for the Multimedia Console at [https://multimedia-console.altvr.com/](https://multimedia-console.altvr.com/)</span></span>
3. <span data-ttu-id="cb410-116">从 web 门户中，可以为多媒体控制台生成和发布配置。</span><span class="sxs-lookup"><span data-stu-id="cb410-116">From the web portal, you can generate and publish a configuration for the Multimedia Console.</span></span>  <span data-ttu-id="cb410-117">有关) 的各种属性的详细信息，请参阅下面的 (。</span><span class="sxs-lookup"><span data-stu-id="cb410-117">(See below for details about the various properties).</span></span>
4. <span data-ttu-id="cb410-118">将媒体输入媒体列表并配置了 "常规设置" 后，在应用程序的右上部分选择 "发布" 按钮。</span><span class="sxs-lookup"><span data-stu-id="cb410-118">Once you've entered the media into the media list and have configured the general settings, select the publish button in the top-right part of the app.</span></span>
5. <span data-ttu-id="cb410-119">发布完成后，将弹出一个对话框，其中包含两个 word 代码，你可以在其中进入你所放置的多媒体控制台。</span><span class="sxs-lookup"><span data-stu-id="cb410-119">Once the publish has completed, a dialog will pop up with a two word code for you to enter in to the Multimedia Console you placed.</span></span>
  
### <a name="placing-the-multimedia-console-in-your-environment"></a><span data-ttu-id="cb410-120">将多媒体控制台放置在您的环境中</span><span class="sxs-lookup"><span data-stu-id="cb410-120">Placing the Multimedia console in your environment</span></span>

1. <span data-ttu-id="cb410-121">选择 "在 **世界编辑器 > 编辑器" 面板 > SDK 应用 > 多媒体控制台**。</span><span class="sxs-lookup"><span data-stu-id="cb410-121">Select on **World Editor > Editor Panel > SDK Apps > Multimedia Console**.</span></span> <span data-ttu-id="cb410-122"> (不会转向 **> 基本 > SDK 应用程序的全球编辑器**-这适用于未注册的应用程序。 ) </span><span class="sxs-lookup"><span data-stu-id="cb410-122">(Don't go to **World Editor > Basics > SDK App**--that's for unregistered apps.)</span></span>  
2. <span data-ttu-id="cb410-123">将多媒体控制台定位到最适合你的空间和受众。</span><span class="sxs-lookup"><span data-stu-id="cb410-123">Position the Multimedia Console to best suite your space and audience.</span></span>
3. <span data-ttu-id="cb410-124">单击 "橙色编辑模式" 按钮即可退出编辑模式。</span><span class="sxs-lookup"><span data-stu-id="cb410-124">Get out of Edit Mode by clicking the orange Edit Mode button.</span></span>
4. <span data-ttu-id="cb410-125">系统将提示你 **是否是 media player 所有者？**</span><span class="sxs-lookup"><span data-stu-id="cb410-125">You'll be prompted **Are you the media player owner?**</span></span> <span data-ttu-id="cb410-126">如果你是此多媒体控制台会话的官方所有者，请确认并继续。</span><span class="sxs-lookup"><span data-stu-id="cb410-126">If you're the person who should be the official owner of this Multimedia Console session, confirm and continue.</span></span> <span data-ttu-id="cb410-127"> (其他授权角色也可用。</span><span class="sxs-lookup"><span data-stu-id="cb410-127">(Other permissioned roles are available as well.</span></span> <span data-ttu-id="cb410-128">请参阅下面的详细列表。 ) </span><span class="sxs-lookup"><span data-stu-id="cb410-128">See below for a detailed list.)</span></span>
5. <span data-ttu-id="cb410-129">选择 "是" 以确认你是主主机。</span><span class="sxs-lookup"><span data-stu-id="cb410-129">Select Yes to confirm that you are the primary host.</span></span>  
6. <span data-ttu-id="cb410-130">将弹出一个对话框，要求您从 web 门户或有效的 JSON 输入一个代码。</span><span class="sxs-lookup"><span data-stu-id="cb410-130">A dialog should pop up that asks you to enter a code from the web portal or valid JSON.</span></span>  <span data-ttu-id="cb410-131">输入来自 web 门户的两个单词代码，包括短划线并单击 "确定"。</span><span class="sxs-lookup"><span data-stu-id="cb410-131">Enter the two word code from the web portal including the dash and hit OK.</span></span> <span data-ttu-id="cb410-132"> (JSON 是如下所述的高级配置) </span><span class="sxs-lookup"><span data-stu-id="cb410-132">(JSON is an advanced configuration described below)</span></span>
7. <span data-ttu-id="cb410-133">多媒体控制台应在几秒钟后使用在 web 门户中生成的配置加载。</span><span class="sxs-lookup"><span data-stu-id="cb410-133">The Multimedia Console should load after a few seconds with the configuration you built in the web portal.</span></span>

### <a name="controlling-the-multimedia-console"></a><span data-ttu-id="cb410-134">控制多媒体控制台</span><span class="sxs-lookup"><span data-stu-id="cb410-134">Controlling the Multimedia console</span></span>

1. <span data-ttu-id="cb410-135">输入代码并完成配置过程后，会看到控件按钮显示在媒体显示下方。</span><span class="sxs-lookup"><span data-stu-id="cb410-135">After you input your code and complete the configuration process, you'll see control buttons appear below a media display.</span></span> 
    * <span data-ttu-id="cb410-136">**播放** 会启动媒体查看器 (或在当前项重新启动（如果以前已停止）) </span><span class="sxs-lookup"><span data-stu-id="cb410-136">**Play** starts the media viewer (or restarts at current entry, if previously stopped)</span></span> 
    * <span data-ttu-id="cb410-137">**停止** 停止 media viewer，并隐藏当前媒体。</span><span class="sxs-lookup"><span data-stu-id="cb410-137">**Stop** stops the media viewer, and hides current media.</span></span>  
    * <span data-ttu-id="cb410-138">**下一个/** 上一个跳转到下一个或上一个媒体</span><span class="sxs-lookup"><span data-stu-id="cb410-138">**Next/Prev** skips to next or previous media</span></span> 
    * <span data-ttu-id="cb410-139">**x/x**  在媒体列表中显示当前索引，并允许跳转到列表中的任何点</span><span class="sxs-lookup"><span data-stu-id="cb410-139">**x/x** shows the current index into the media list, and allows you to jump to any point in the list</span></span>
    * <span data-ttu-id="cb410-140">**Config** 允许重新从 web 门户重新设置新的代码，以便在控制台中设置新的配置。</span><span class="sxs-lookup"><span data-stu-id="cb410-140">**Config** allows reentering a new code from the web portal to set a new configuration in the console.</span></span> 

<span data-ttu-id="cb410-141">现在，你已设置为通过多媒体控制台开始共享！</span><span class="sxs-lookup"><span data-stu-id="cb410-141">Now you're set to begin sharing via the Multimedia Console!</span></span>  
 
## <a name="working-with-the-web-portal"></a><span data-ttu-id="cb410-142">使用 web 门户</span><span class="sxs-lookup"><span data-stu-id="cb410-142">Working with the web portal</span></span>

<span data-ttu-id="cb410-143">Web 门户是一个 web 应用，可用于配置多媒体控制台的各种功能。</span><span class="sxs-lookup"><span data-stu-id="cb410-143">The web portal is a web app that enables configuring the various features of the Multimedia Console.</span></span>  <span data-ttu-id="cb410-144">这些功能分为两类：常规媒体控制台设置和 media play 列表。</span><span class="sxs-lookup"><span data-stu-id="cb410-144">These features fall in to two categories; general media console settings, and the media play list.</span></span>

### <a name="multimedia-console-general-settings"></a><span data-ttu-id="cb410-145">多媒体控制台常规设置</span><span class="sxs-lookup"><span data-stu-id="cb410-145">Multimedia console general settings</span></span>

<span data-ttu-id="cb410-146">**Playback 设置**</span><span class="sxs-lookup"><span data-stu-id="cb410-146">**Playback Settings**</span></span>

<span data-ttu-id="cb410-147">媒体列表的常规播放设置</span><span class="sxs-lookup"><span data-stu-id="cb410-147">General playback settings for the media list</span></span>

* <span data-ttu-id="cb410-148">**循环媒体列表**-确定一旦到达列表的末尾，介质列表是否应该循环进入。</span><span class="sxs-lookup"><span data-stu-id="cb410-148">**Loop Media List**- Determines whether the media list should loop around once you reach the end of the list.</span></span>
* <span data-ttu-id="cb410-149">**启动方法** -选择多媒体控制台应启动的方法。</span><span class="sxs-lookup"><span data-stu-id="cb410-149">**Start Method** - Selects the method by which the multimedia console should start.</span></span>
    * <span data-ttu-id="cb410-150">手动-在启动媒体之前等待按下 "播放" 按钮</span><span class="sxs-lookup"><span data-stu-id="cb410-150">Manual - Waits for the play button to be pressed before starting the media</span></span>
    * <span data-ttu-id="cb410-151">自动开始开始-从列表的开头自动启动媒体列表</span><span class="sxs-lookup"><span data-stu-id="cb410-151">Auto Start from Beginning - Auto start the media list from the beginning of the list</span></span>
    * <span data-ttu-id="cb410-152">自动启动随机-自动从列表中的随机起始点启动媒体</span><span class="sxs-lookup"><span data-stu-id="cb410-152">Auto Start Random - Auto starts the media from a random starting point in the list</span></span>

<span data-ttu-id="cb410-153">**角色**</span><span class="sxs-lookup"><span data-stu-id="cb410-153">**Roles**</span></span>

<span data-ttu-id="cb410-154">用于控制和配置多媒体控制台的角色分配。</span><span class="sxs-lookup"><span data-stu-id="cb410-154">Role assignments for controlling and configuring the Multimedia Console.</span></span>    <span data-ttu-id="cb410-155">这些角色分为以下几组：</span><span class="sxs-lookup"><span data-stu-id="cb410-155">These roles are broken down in to the following set:</span></span>

* <span data-ttu-id="cb410-156">**仅所有者** -用户是多媒体控制台会话的所有者</span><span class="sxs-lookup"><span data-stu-id="cb410-156">**Owner Only** - The user that is the owner of the Multimedia Console Session</span></span>
* <span data-ttu-id="cb410-157">**提升的用户** -在最初配置多媒体控制台的空间中具有仲裁者、主机或表示者角色的用户</span><span class="sxs-lookup"><span data-stu-id="cb410-157">**Elevated Users** - Users that have moderator, host, or presenter roles in the space that the Multimedia Console is configured in originally</span></span>
* <span data-ttu-id="cb410-158">**所有用户** -所有用户</span><span class="sxs-lookup"><span data-stu-id="cb410-158">**All Users** - All users</span></span>

<span data-ttu-id="cb410-159">这些角色堆栈的意义在于，此列表中所选的所有角色都将被授予使用该功能的权限。</span><span class="sxs-lookup"><span data-stu-id="cb410-159">These roles stack in the sense that all roles above the one chosen in this list will also be granted permission to use that feature.</span></span>  <span data-ttu-id="cb410-160">示例： **提升的用户** 包括 **所有者** ，即使他们不是 AltspaceVR 中的仲裁者、主机或表示器 \* \*。</span><span class="sxs-lookup"><span data-stu-id="cb410-160">Example: **Elevated Users** includes the **Owner** even if they aren't a moderator, host, or presenter\*\* in AltspaceVR.</span></span> <span data-ttu-id="cb410-161">由角色分配控制的功能如下所示</span><span class="sxs-lookup"><span data-stu-id="cb410-161">Features that are controlled by role assignments are as follows</span></span>

* <span data-ttu-id="cb410-162">**可以控制 media player** -确定哪些角色可以控制多媒体控制台的媒体播放按钮</span><span class="sxs-lookup"><span data-stu-id="cb410-162">**Can control media player** - Determines what roles can control the media playback buttons for the Multimedia Console</span></span>
* <span data-ttu-id="cb410-163">**可以配置 media player** -确定哪些角色可以通过向 " **配置** " 按钮授予访问权限来配置多媒体控制台</span><span class="sxs-lookup"><span data-stu-id="cb410-163">**Can configure the media player** - Determines what roles can configure the Multimedia Console by being granted access to the **Config** button</span></span>

### <a name="adding-photos-and-videos-to-the-media-list"></a><span data-ttu-id="cb410-164">将照片和视频添加到媒体列表</span><span class="sxs-lookup"><span data-stu-id="cb410-164">Adding photos and videos to the media list</span></span>

<span data-ttu-id="cb410-165">媒体是多媒体控制台的核心。</span><span class="sxs-lookup"><span data-stu-id="cb410-165">Media is the heart of the Multimedia Console.</span></span>  <span data-ttu-id="cb410-166">支持在多媒体控制台中将图像和视频链接作为媒体类型。</span><span class="sxs-lookup"><span data-stu-id="cb410-166">Images and video links are supported as media types within the Multimedia Console.</span></span>  <span data-ttu-id="cb410-167">若要添加新媒体，请选择 " **添加映像** " 或 " **添加视频** " 图标以显示一个对话框，以输入媒体信息和设置。</span><span class="sxs-lookup"><span data-stu-id="cb410-167">To add new media, select either the **Add Image** or **Add Video** icons to have a dialog pop up to enter the media information and settings.</span></span>  <span data-ttu-id="cb410-168">下面是媒体类型和相关设置的细目分类</span><span class="sxs-lookup"><span data-stu-id="cb410-168">Below is the breakdown of the media types and associated settings</span></span>

<span data-ttu-id="cb410-169">**图像**</span><span class="sxs-lookup"><span data-stu-id="cb410-169">**Image**</span></span>

<span data-ttu-id="cb410-170">图像应为标准图像类型，如 jpeg、png 和儿子。</span><span class="sxs-lookup"><span data-stu-id="cb410-170">Images should be a standard image type such as jpeg, png, and son on.</span></span> <span data-ttu-id="cb410-171">它们需要托管在某个位置，并使用公用链接。</span><span class="sxs-lookup"><span data-stu-id="cb410-171">They need to be hosted somewhere with a public link.</span></span>

* <span data-ttu-id="cb410-172">**名称** - (需要用来标识映像的) 名称。</span><span class="sxs-lookup"><span data-stu-id="cb410-172">**Name** - (Required) Name that you wish to identify the image with.</span></span>
* <span data-ttu-id="cb410-173">**图像 URL** - (所需) 图像的公共 URL</span><span class="sxs-lookup"><span data-stu-id="cb410-173">**Image URL** - (Required) The public url of the image</span></span>
* <span data-ttu-id="cb410-174">"**跳过**"-之后应跳过图像的秒数</span><span class="sxs-lookup"><span data-stu-id="cb410-174">**Skip After** - The number of seconds that the image should be skipped after</span></span>

<span data-ttu-id="cb410-175">**视频**</span><span class="sxs-lookup"><span data-stu-id="cb410-175">**Video**</span></span>

<span data-ttu-id="cb410-176">视频可以通过 Twitch 和 DLive 托管视频或实时流。</span><span class="sxs-lookup"><span data-stu-id="cb410-176">Videos can be hosted videos or live streams through Twitch and DLive.</span></span>  <span data-ttu-id="cb410-177"> (其他支持可能会使用额外的工作来获取正确的流 url，但在多媒体控制台内不完全受支持) </span><span class="sxs-lookup"><span data-stu-id="cb410-177">(Other support may function with extra work to get the proper stream url, but aren't fully supported within the Multimedia Console)</span></span>

* <span data-ttu-id="cb410-178">**名称** - (需要用来标识视频的) 名称。</span><span class="sxs-lookup"><span data-stu-id="cb410-178">**Name** - (Required) Name that you wish to identify the video with.</span></span>
* <span data-ttu-id="cb410-179">**视频 URL** - (所需的) 视频所托管的公共 URL，或提供实时流。</span><span class="sxs-lookup"><span data-stu-id="cb410-179">**Video URL** - (Required) The public url that the video is hosted at or the live stream is served from.</span></span>
* <span data-ttu-id="cb410-180">"**跳过**"-之后应跳过视频的秒数</span><span class="sxs-lookup"><span data-stu-id="cb410-180">**Skip After** - The number of seconds that the video should be skipped after</span></span>
* <span data-ttu-id="cb410-181">**卷** -从 0 (最小) -1 (最大) 值的视频量。</span><span class="sxs-lookup"><span data-stu-id="cb410-181">**Volume** - The volume of the video from 0 (min) - 1 (max) values.</span></span>
* <span data-ttu-id="cb410-182">**开始时间** -从视频开始开始的秒数（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="cb410-182">**Start Time** - The number of seconds from the beginning of the video start from.</span></span>
* <span data-ttu-id="cb410-183">**开始距离** -在离开多媒体控制台时，在世界上以米为单位开始衰减的距离</span><span class="sxs-lookup"><span data-stu-id="cb410-183">**Roll Off Start Distance** - The distance in meters in world that the volume begins to fall off at as you move away from the Multimedia Console</span></span>
* <span data-ttu-id="cb410-184">**视频结束操作** -到达视频末尾后要执行的操作。</span><span class="sxs-lookup"><span data-stu-id="cb410-184">**End of Video Action** - The action to take once the end of the video is reached.</span></span>
    * <span data-ttu-id="cb410-185">停止-媒体列表在视频结束后停止</span><span class="sxs-lookup"><span data-stu-id="cb410-185">Stop - The media list stops after the video has ended</span></span>
    * <span data-ttu-id="cb410-186">循环-视频将循环，直到手动跳过</span><span class="sxs-lookup"><span data-stu-id="cb410-186">Loop - The video will loop until manually skipped</span></span>
    * <span data-ttu-id="cb410-187">下一步-在当前视频结束后，介质列表中的下一个介质将启动。</span><span class="sxs-lookup"><span data-stu-id="cb410-187">Play Next - The next media in the media list will be started after the current video ends.</span></span>

## <a name="working-with-json-directly-advancedoptional"></a><span data-ttu-id="cb410-188">直接使用 JSON (高级/可选) </span><span class="sxs-lookup"><span data-stu-id="cb410-188">Working with JSON directly (advanced/optional)</span></span>

<span data-ttu-id="cb410-189">多媒体控制台支持直接在 AltspaceVR 中的控制台提示符下输入 JSON。</span><span class="sxs-lookup"><span data-stu-id="cb410-189">The Multimedia Console supports entering JSON directly in to the prompt of the console in AltspaceVR.</span></span>  <span data-ttu-id="cb410-190">JSON 是一种内部机制，使用它可以实现媒体播放器配置。</span><span class="sxs-lookup"><span data-stu-id="cb410-190">JSON is the internal mechanism with which we enable media player configurations.</span></span> <span data-ttu-id="cb410-191">通过公开设置 JSON 的功能，可使更高级的用户能够构建自己的工作流，这些工作流可满足其需求并熟悉 JSON。</span><span class="sxs-lookup"><span data-stu-id="cb410-191">Exposing the ability to set JSON directly is something that allows for more advanced users to build their own workflows that suites their needs and familiarity with JSON.</span></span>  <span data-ttu-id="cb410-192">下面是 JSON 结构的简短说明，以及 JSON 的验证架构。</span><span class="sxs-lookup"><span data-stu-id="cb410-192">The following is a brief description of the JSON structure and the schema by which the JSON is validated.</span></span> <span data-ttu-id="cb410-193">有关以下属性的更多详细说明，请参阅上一节介绍了如何配置多媒体控制台。</span><span class="sxs-lookup"><span data-stu-id="cb410-193">For more detailed descriptions of the properties below, see the above sections that talk about configuring the Multimedia Console.</span></span>  <span data-ttu-id="cb410-194">本部分重点介绍用于 JSON 数据的架构示例和结构。</span><span class="sxs-lookup"><span data-stu-id="cb410-194">This section is focused primarily on the schema examples and structuring for the JSON data.</span></span>

### <a name="global-media-settings"></a><span data-ttu-id="cb410-195">全局媒体设置</span><span class="sxs-lookup"><span data-stu-id="cb410-195">Global media settings</span></span>

```json
{
  "loopMediaList": true | false
  "startMethod": "manual" | "autostart-beginning" | "autostart-random"
  "controlMediaPlayer": "everyone" | "elevated" | "owner"
  "configureMediaPlayer": "elevated" | "owner"
  ...
}
```

### <a name="media-list"></a><span data-ttu-id="cb410-196">媒体列表</span><span class="sxs-lookup"><span data-stu-id="cb410-196">Media list</span></span>

<span data-ttu-id="cb410-197">媒体列表是 JSON 结构的根目录中的属性集，如角色和播放设置。</span><span class="sxs-lookup"><span data-stu-id="cb410-197">The media list is a property set at the root of the JSON structure like the Roles and Playback Settings.</span></span>  <span data-ttu-id="cb410-198">它是一个简单的数组，它可以包含以下媒体配置结构之一。</span><span class="sxs-lookup"><span data-stu-id="cb410-198">It's a simple array that can contain one of the following media configuration structures.</span></span> <span data-ttu-id="cb410-199"> (参见上面的属性说明了解每个操作的详细信息。 ) </span><span class="sxs-lookup"><span data-stu-id="cb410-199">(See property descriptions above for details on what each does.)</span></span>

<span data-ttu-id="cb410-200">**图像示例**</span><span class="sxs-lookup"><span data-stu-id="cb410-200">**Image example**</span></span>

<span data-ttu-id="cb410-201">*必填字段： "name" 和 "imageUrl"*</span><span class="sxs-lookup"><span data-stu-id="cb410-201">*Required fields: "name" and "imageUrl"*</span></span>

```json
{
    "name": "Altspace Screenshot",
    "imageUrl": "https://pbs.twimg.com/media/CxJ-fJqUsAAFtd9.jpg",
    "skipAfter": 10
}
```

<span data-ttu-id="cb410-202">**视频示例**</span><span class="sxs-lookup"><span data-stu-id="cb410-202">**Video example**</span></span>

<span data-ttu-id="cb410-203">*必填字段： "name" 和 "videoUrl"*</span><span class="sxs-lookup"><span data-stu-id="cb410-203">*Required fields: "name" and "videoUrl"*</span></span>

```json
{
    "name": "Ninja Twitch Live Stream",
    "videoUrl":"https://www.twitch.tv/ninja",
    "volume":0.2,
    "startTime":0,
    "endOfVideoAction":"play-next"
}
```

### <a name="example-json"></a><span data-ttu-id="cb410-204">示例 JSON</span><span class="sxs-lookup"><span data-stu-id="cb410-204">Example JSON</span></span>

```json
{
  "loopMediaList": false,
  "startMethod": "autostart-beginning",
  "controlMediaPlayer": "everyone",
  "configureMediaPlayer": "elevated",
  "mediaList": [
    {
      "videoUrl": "https://www.twitch.tv/ninja",
      "volume": 0.2,
      "startTime": 0,
      "endOfVideoAction": "play-next"
    },
    {
      "imageUrl": "http://www.hypergridbusiness.com/wp-content/uploads/2016/09/AltspaceVR-highrise.jpg",
      "skipAfter": 10
    },
    {
      "imageUrl": "https://d1qb2nb5cznatu.cloudfront.net/startups/i/333629-6ffd7199b9bcf34d8957e8e09d974a38-medium_jpg.jpg?buster=1423092095",
      "skipAfter": 5
    },
    {
      "imageUrl": "https://pbs.twimg.com/media/CxJ-fJqUsAAFtd9.jpg",
      "skipAfter": 10
    },
    {
      "imageUrl": "https://altvr-wpengine.netdna-ssl.com/wp-content/uploads/2019/05/Educators-in-VR-Social-VR-AltspaceVR.png",
      "skipAfter": 10
    },
    {
      "videoUrl": "https://www.twitch.tv/shroud",
      "volume": 1,
      "startTime": 0,
      "endOfVideoAction": "stop"
    }
  ]
}
```

### <a name="schema"></a><span data-ttu-id="cb410-205">架构</span><span class="sxs-lookup"><span data-stu-id="cb410-205">Schema</span></span>

```json
{
  "$schema": "https://json-schema.org/draft-04/schema#",
  "type": "object",
  "required": [
    "mediaList"
  ],
  "properties": {
    "loopMediaList": {
      "type": "boolean",
      "description": "Whether to loop through the media list when reaching the beginning or end of the list."
    },
    "controlMediaPlayer": {
      "type": "string",
      "enum": [
        "everyone",
        "elevated",
        "owner"
      ],
      "default": "owner",
      "description": "What roles are able to control the media player. (Owner can always control player)"
    },
    "configureMediaPlayer": {
      "type": "string",
      "enum": [
        "elevated",
        "owner"
      ],
      "default": "owner",
      "description": "What roles are allowed to configure the media play list.  Note: This role needs to be able to control the media player in order to configure it. (Owner can always configure media)"
    },
    "startMethod": {
      "type": "string",
      "enum": [
        "manual",
        "autostart-beginning",
        "autostart-random"
      ],
      "default": "manual",
      "description": "The method by which the media player should start"
    },
    "mediaList": {
      "description": "A list of images or videos to configure the media player to operate on.",
      "type": "array",
      "items": {
        "oneOf": [
          {
            "title": "Image",
            "type": "object",
            "description": "Configuration for an image media.",
            "properties": {
              "imageUrl": {
                "type": "string",
                "description": "The url for the image to load."
              },
              "skipAfter": {
                "type": "number",
                "minimum": 5,
                "default": null,
                "description": "The number of seconds that should pass before skipping to the next media. (Minimum 5)."
              }
            },
            "required": [
              "imageUrl"
            ]
          },
          {
            "title": "Video",
            "type": "object",
            "description": "Configuration for a video media.",
            "properties": {
              "videoUrl": {
                "type": "string",
                "description": "The url of the video to load."
              },
              "skipAfter": {
                "type": "number",
                "minimum": 5,
                "default": null,
                "description": "The number of seconds that should pass before skipping to the next media. (Minimum 5)."
              },
              "volume": {
                "type": "number",
                "minimum": 0,
                "maximum": 1,
                "default": null,
                "description": "The volume to play the video at. (Minimum 0, maximum 1)"
              },
              "startTime": {
                "type": "number",
                "minimum": 0,
                "default": null,
                "description": "The time in seconds from the start of the video to begin playing the video at. (Minimum of 0)"
              },
              "rolloffStartDistance": {
                "type": "number",
                "minimum": 0,
                "default": null,
                "description": "The distance in meters away from the media player that the volume will begin to fall off. (Minimum 0)"
              },
              "endOfVideoAction": {
                "type": "string",
                "enum": [
                  "stop",
                  "loop",
                  "play-next"
                ],
                "default": null,
                "description": "The type of action to take at the end of the video."
              }
            },
            "required": [
              "videoUrl"
            ]
          }
        ]
      }
    }
  }
}
```

> [!NOTE]
> <span data-ttu-id="cb410-206">多媒体控制台 v 0.5.0 的最新版本</span><span class="sxs-lookup"><span data-stu-id="cb410-206">Up to date with Multimedia Console v0.5.0</span></span>