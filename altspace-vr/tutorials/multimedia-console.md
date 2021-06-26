---
title: 使用多媒体控制台
description: 了解如何开始在 AltspaceVR 体验中配置、发布和控制多媒体控制台。
ms.date: 03/11/2021
ms.topic: article
keywords: 控制台，多媒体
ms.openlocfilehash: 4a51ff76e44d3870972bc17288ae77c1fa888922
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/25/2021
ms.locfileid: "112923004"
---
# <a name="using-the-multimedia-console"></a><span data-ttu-id="934c8-104">使用多媒体控制台</span><span class="sxs-lookup"><span data-stu-id="934c8-104">Using the multimedia console</span></span>

<span data-ttu-id="934c8-105">多媒体控制台是一种支持事件和世界媒体共享的工具。</span><span class="sxs-lookup"><span data-stu-id="934c8-105">The Multimedia Console is a tool that enables media sharing in events and worlds.</span></span> <span data-ttu-id="934c8-106">可以使用它来共享图像、演示文稿幻灯片、实时流、视频、播放列表等内容。</span><span class="sxs-lookup"><span data-stu-id="934c8-106">You can use it to share things like images, presentation slides, livestreams, videos, playlists, and more.</span></span> <span data-ttu-id="934c8-107">下面是有关如何使用多媒体控制台 **v0.5.0+ 的分步说明**。</span><span class="sxs-lookup"><span data-stu-id="934c8-107">Below is a step-by-step instruction on how to use the Multimedia Console **v0.5.0+**.</span></span> 

## <a name="getting-started"></a><span data-ttu-id="934c8-108">入门</span><span class="sxs-lookup"><span data-stu-id="934c8-108">Getting started</span></span>

<span data-ttu-id="934c8-109">多媒体控制台入门由两部分完成。</span><span class="sxs-lookup"><span data-stu-id="934c8-109">Getting started with the Multimedia Console is a two part process.</span></span>  <span data-ttu-id="934c8-110">首先，使用 Web 门户为环境中放置的多媒体控制台会话生成和发布配置。</span><span class="sxs-lookup"><span data-stu-id="934c8-110">First there's the web portal that you'll use to generate and publish a configuration for the Multimedia Console session you place in your environment.</span></span>  <span data-ttu-id="934c8-111">其次，将实际多媒体控制台应用放置于环境中，并设置它应该使用的配置代码。</span><span class="sxs-lookup"><span data-stu-id="934c8-111">Second is the placement of the actual Multimedia Console app in your environment and setting the configuration code it should use.</span></span>

### <a name="configuring-the-multimedia-console-with-the-web-portal"></a><span data-ttu-id="934c8-112">使用 Web 门户配置多媒体控制台</span><span class="sxs-lookup"><span data-stu-id="934c8-112">Configuring the Multimedia console with the web portal</span></span>

1. <span data-ttu-id="934c8-113">首先，需要确保内容联机托管，因为需要 URL。</span><span class="sxs-lookup"><span data-stu-id="934c8-113">First, you'll need to make sure your content is hosted online because you'll need a URL.</span></span> <span data-ttu-id="934c8-114"> (可以将照片上传到 altvr.com、在线托管视频.mp4或使用 Dlive 实时流链接： https://dlive.tv/yourlivestream)</span><span class="sxs-lookup"><span data-stu-id="934c8-114">(You can upload photos to altvr.com, host a video .mp4 file online or use a Dlive live stream link: https://dlive.tv/yourlivestream)</span></span> 
2. <span data-ttu-id="934c8-115">导航到多媒体控制台的 Web 门户，网址为 [https://multimedia-console.altvr.com/](https://multimedia-console.altvr.com/)</span><span class="sxs-lookup"><span data-stu-id="934c8-115">Navigate to the web portal for the Multimedia Console at [https://multimedia-console.altvr.com/](https://multimedia-console.altvr.com/)</span></span>
3. <span data-ttu-id="934c8-116">在 Web 门户中，可以生成并发布多媒体控制台的配置。</span><span class="sxs-lookup"><span data-stu-id="934c8-116">From the web portal, you can generate and publish a configuration for the Multimedia Console.</span></span>  <span data-ttu-id="934c8-117"> (请参阅下文，了解有关各种属性) 。</span><span class="sxs-lookup"><span data-stu-id="934c8-117">(See below for details about the various properties).</span></span>
4. <span data-ttu-id="934c8-118">将媒体输入媒体列表并配置常规设置后，选择应用右上方的"发布"按钮。</span><span class="sxs-lookup"><span data-stu-id="934c8-118">Once you've entered the media into the media list and have configured the general settings, select the publish button in the top-right part of the app.</span></span>
5. <span data-ttu-id="934c8-119">发布完成后，将弹出一个对话框，其中包含两个单词代码，供你进入放置的多媒体控制台。</span><span class="sxs-lookup"><span data-stu-id="934c8-119">Once the publish has completed, a dialog will pop up with a two word code for you to enter in to the Multimedia Console you placed.</span></span>
  
### <a name="placing-the-multimedia-console-in-your-environment"></a><span data-ttu-id="934c8-120">将多媒体控制台置于环境中</span><span class="sxs-lookup"><span data-stu-id="934c8-120">Placing the Multimedia console in your environment</span></span>

1. <span data-ttu-id="934c8-121">在"世界 **编辑器">"编辑器面板> SDK 应用>"多媒体控制台"。**</span><span class="sxs-lookup"><span data-stu-id="934c8-121">Select on **World Editor > Editor Panel > SDK Apps > Multimedia Console**.</span></span> <span data-ttu-id="934c8-122"> (SDK 应用中转到"世界编辑器">">" **基本信息**"-这是针对未注册的应用) </span><span class="sxs-lookup"><span data-stu-id="934c8-122">(Don't go to **World Editor > Basics > SDK App**--that's for unregistered apps.)</span></span>  
2. <span data-ttu-id="934c8-123">定位多媒体控制台，以最佳方式设置空间和受众。</span><span class="sxs-lookup"><span data-stu-id="934c8-123">Position the Multimedia Console to best suite your space and audience.</span></span>
3. <span data-ttu-id="934c8-124">单击橙色的"编辑模式"按钮，退出编辑模式。</span><span class="sxs-lookup"><span data-stu-id="934c8-124">Get out of Edit Mode by clicking the orange Edit Mode button.</span></span>
4. <span data-ttu-id="934c8-125">系统会提示你是 **媒体播放器所有者吗？**</span><span class="sxs-lookup"><span data-stu-id="934c8-125">You'll be prompted **Are you the media player owner?**</span></span> <span data-ttu-id="934c8-126">如果你是此多媒体控制台会话的官方所有者，请确认并继续。</span><span class="sxs-lookup"><span data-stu-id="934c8-126">If you're the person who should be the official owner of this Multimedia Console session, confirm and continue.</span></span> <span data-ttu-id="934c8-127"> (其他权限角色也可用。</span><span class="sxs-lookup"><span data-stu-id="934c8-127">(Other permissioned roles are available as well.</span></span> <span data-ttu-id="934c8-128">有关详细列表，请参阅) </span><span class="sxs-lookup"><span data-stu-id="934c8-128">See below for a detailed list.)</span></span>
5. <span data-ttu-id="934c8-129">选择"是"以确认你是主主机。</span><span class="sxs-lookup"><span data-stu-id="934c8-129">Select Yes to confirm that you are the primary host.</span></span>  
6. <span data-ttu-id="934c8-130">应弹出一个对话框，要求你输入 Web 门户中的代码或有效的 JSON。</span><span class="sxs-lookup"><span data-stu-id="934c8-130">A dialog should pop up that asks you to enter a code from the web portal or valid JSON.</span></span>  <span data-ttu-id="934c8-131">输入 Web 门户中的两个单词代码（包括短划线）并点击"确定"。</span><span class="sxs-lookup"><span data-stu-id="934c8-131">Enter the two word code from the web portal including the dash and hit OK.</span></span> <span data-ttu-id="934c8-132"> (JSON 是下面所述的高级) </span><span class="sxs-lookup"><span data-stu-id="934c8-132">(JSON is an advanced configuration described below)</span></span>
7. <span data-ttu-id="934c8-133">多媒体控制台应在几秒钟后使用你在 Web 门户中构建的配置进行加载。</span><span class="sxs-lookup"><span data-stu-id="934c8-133">The Multimedia Console should load after a few seconds with the configuration you built in the web portal.</span></span>

### <a name="controlling-the-multimedia-console"></a><span data-ttu-id="934c8-134">控制多媒体控制台</span><span class="sxs-lookup"><span data-stu-id="934c8-134">Controlling the Multimedia console</span></span>

1. <span data-ttu-id="934c8-135">输入代码并完成配置过程后，你将看到控件按钮显示在媒体显示下方。</span><span class="sxs-lookup"><span data-stu-id="934c8-135">After you input your code and complete the configuration process, you'll see control buttons appear below a media display.</span></span> 
    * <span data-ttu-id="934c8-136">**如果** 之前已停止 (，Play 将启动媒体查看器，或在当前条目) </span><span class="sxs-lookup"><span data-stu-id="934c8-136">**Play** starts the media viewer (or restarts at current entry, if previously stopped)</span></span> 
    * <span data-ttu-id="934c8-137">**"** 停止"可停止媒体查看器，并隐藏当前媒体。</span><span class="sxs-lookup"><span data-stu-id="934c8-137">**Stop** stops the media viewer, and hides current media.</span></span>  
    * <span data-ttu-id="934c8-138">**Next/Prev** 跳到下一个或上一个媒体</span><span class="sxs-lookup"><span data-stu-id="934c8-138">**Next/Prev** skips to next or previous media</span></span> 
    * <span data-ttu-id="934c8-139">**x/x**  显示媒体列表中的当前索引，并允许跳转到列表中的任意点</span><span class="sxs-lookup"><span data-stu-id="934c8-139">**x/x** shows the current index into the media list, and allows you to jump to any point in the list</span></span>
    * <span data-ttu-id="934c8-140">**配置** 允许从 Web 门户重新输入新代码，以在控制台中设置新配置。</span><span class="sxs-lookup"><span data-stu-id="934c8-140">**Config** allows reentering a new code from the web portal to set a new configuration in the console.</span></span> 

<span data-ttu-id="934c8-141">现在，你已设置为通过多媒体控制台开始共享！</span><span class="sxs-lookup"><span data-stu-id="934c8-141">Now you're set to begin sharing via the Multimedia Console!</span></span>  
 
## <a name="working-with-the-web-portal"></a><span data-ttu-id="934c8-142">使用 Web 门户</span><span class="sxs-lookup"><span data-stu-id="934c8-142">Working with the web portal</span></span>

<span data-ttu-id="934c8-143">Web 门户是一个 Web 应用，可用于配置多媒体控制台的各种功能。</span><span class="sxs-lookup"><span data-stu-id="934c8-143">The web portal is a web app that enables configuring the various features of the Multimedia Console.</span></span>  <span data-ttu-id="934c8-144">这些功能分为两类：常规媒体控制台设置和媒体播放列表。</span><span class="sxs-lookup"><span data-stu-id="934c8-144">These features fall in to two categories; general media console settings, and the media play list.</span></span>

### <a name="multimedia-console-general-settings"></a><span data-ttu-id="934c8-145">多媒体控制台常规设置</span><span class="sxs-lookup"><span data-stu-id="934c8-145">Multimedia console general settings</span></span>

<span data-ttu-id="934c8-146">**Playback 设置**</span><span class="sxs-lookup"><span data-stu-id="934c8-146">**Playback Settings**</span></span>

<span data-ttu-id="934c8-147">媒体列表的常规播放设置</span><span class="sxs-lookup"><span data-stu-id="934c8-147">General playback settings for the media list</span></span>

* <span data-ttu-id="934c8-148">**循环媒体列表**- 确定到达列表末尾后，媒体列表是否应该循环。</span><span class="sxs-lookup"><span data-stu-id="934c8-148">**Loop Media List**- Determines whether the media list should loop around once you reach the end of the list.</span></span>
* <span data-ttu-id="934c8-149">**Start 方法** - 选择多媒体控制台启动的方法。</span><span class="sxs-lookup"><span data-stu-id="934c8-149">**Start Method** - Selects the method by which the multimedia console should start.</span></span>
    * <span data-ttu-id="934c8-150">手动 - 在启动媒体之前等待播放按钮按下</span><span class="sxs-lookup"><span data-stu-id="934c8-150">Manual - Waits for the play button to be pressed before starting the media</span></span>
    * <span data-ttu-id="934c8-151">自动从开始开始 - 从列表开头自动启动媒体列表</span><span class="sxs-lookup"><span data-stu-id="934c8-151">Auto Start from Beginning - Auto start the media list from the beginning of the list</span></span>
    * <span data-ttu-id="934c8-152">自动启动随机 - 自动从列表中的随机起点启动媒体</span><span class="sxs-lookup"><span data-stu-id="934c8-152">Auto Start Random - Auto starts the media from a random starting point in the list</span></span>

<span data-ttu-id="934c8-153">**角色**</span><span class="sxs-lookup"><span data-stu-id="934c8-153">**Roles**</span></span>

<span data-ttu-id="934c8-154">用于控制和配置多媒体控制台的角色分配。</span><span class="sxs-lookup"><span data-stu-id="934c8-154">Role assignments for controlling and configuring the Multimedia Console.</span></span>    <span data-ttu-id="934c8-155">这些角色分为以下集：</span><span class="sxs-lookup"><span data-stu-id="934c8-155">These roles are broken down in to the following set:</span></span>

* <span data-ttu-id="934c8-156">**仅所有者** - 作为多媒体控制台会话所有者的用户</span><span class="sxs-lookup"><span data-stu-id="934c8-156">**Owner Only** - The user that is the owner of the Multimedia Console Session</span></span>
* <span data-ttu-id="934c8-157">**提升的用户** - 在最初配置多媒体控制台的空间内具有审查器或主机角色的用户</span><span class="sxs-lookup"><span data-stu-id="934c8-157">**Elevated Users** - Users that have moderator or host roles in the space that the Multimedia Console is configured in originally</span></span>
* <span data-ttu-id="934c8-158">**所有用户** - 所有用户</span><span class="sxs-lookup"><span data-stu-id="934c8-158">**All Users** - All users</span></span>

<span data-ttu-id="934c8-159">这些角色堆栈在这样一种意义上说，在此列表中选择的角色之上的所有角色也将被授予使用该功能的权限。</span><span class="sxs-lookup"><span data-stu-id="934c8-159">These roles stack in the sense that all roles above the one chosen in this list will also be granted permission to use that feature.</span></span>  <span data-ttu-id="934c8-160">示例： **提升的用户** 包括 **所有者** ，即使他们不是 AltspaceVR 中的审查器或主机。</span><span class="sxs-lookup"><span data-stu-id="934c8-160">Example: **Elevated Users** includes the **Owner** even if they aren't a moderator or host\*\* in AltspaceVR.</span></span> <span data-ttu-id="934c8-161">由角色分配控制的功能如下所示</span><span class="sxs-lookup"><span data-stu-id="934c8-161">Features that are controlled by role assignments are as follows</span></span>

* <span data-ttu-id="934c8-162">**可以控制媒体播放器** - 确定哪些角色可以控制多媒体控制台的媒体播放按钮</span><span class="sxs-lookup"><span data-stu-id="934c8-162">**Can control media player** - Determines what roles can control the media playback buttons for the Multimedia Console</span></span>
* <span data-ttu-id="934c8-163">**可以配置媒体播放器**- 通过授予对"配置"按钮的访问权限，确定哪些角色可以配置多媒体 **控制台**</span><span class="sxs-lookup"><span data-stu-id="934c8-163">**Can configure the media player** - Determines what roles can configure the Multimedia Console by being granted access to the **Config** button</span></span>

### <a name="adding-photos-and-videos-to-the-media-list"></a><span data-ttu-id="934c8-164">将照片和视频添加到媒体列表</span><span class="sxs-lookup"><span data-stu-id="934c8-164">Adding photos and videos to the media list</span></span>

<span data-ttu-id="934c8-165">媒体是多媒体控制台的核心。</span><span class="sxs-lookup"><span data-stu-id="934c8-165">Media is the heart of the Multimedia Console.</span></span>  <span data-ttu-id="934c8-166">多媒体控制台中支持将图像和视频链接作为媒体类型。</span><span class="sxs-lookup"><span data-stu-id="934c8-166">Images and video links are supported as media types within the Multimedia Console.</span></span>  <span data-ttu-id="934c8-167">若要添加新媒体，请选择"添加图像"或"添加 **视频**"图标，弹出一个对话框以输入媒体信息和设置。</span><span class="sxs-lookup"><span data-stu-id="934c8-167">To add new media, select either the **Add Image** or **Add Video** icons to have a dialog pop up to enter the media information and settings.</span></span>  <span data-ttu-id="934c8-168">下面是媒体类型和关联设置的细分</span><span class="sxs-lookup"><span data-stu-id="934c8-168">Below is the breakdown of the media types and associated settings</span></span>

<span data-ttu-id="934c8-169">**Image**</span><span class="sxs-lookup"><span data-stu-id="934c8-169">**Image**</span></span>

<span data-ttu-id="934c8-170">图像应为标准图像类型，例如 jpeg、png 和子图像。</span><span class="sxs-lookup"><span data-stu-id="934c8-170">Images should be a standard image type such as jpeg, png, and son on.</span></span> <span data-ttu-id="934c8-171">它们需要托管在具有公共链接的某处。</span><span class="sxs-lookup"><span data-stu-id="934c8-171">They need to be hosted somewhere with a public link.</span></span>

* <span data-ttu-id="934c8-172">**名称** - (标识) 的必需名称。</span><span class="sxs-lookup"><span data-stu-id="934c8-172">**Name** - (Required) Name that you wish to identify the image with.</span></span>
* <span data-ttu-id="934c8-173">**图像 URL** - (必需) 图像的公共 URL</span><span class="sxs-lookup"><span data-stu-id="934c8-173">**Image URL** - (Required) The public url of the image</span></span>
* <span data-ttu-id="934c8-174">**在** 之后跳过 - 应在之后跳过映像的秒数</span><span class="sxs-lookup"><span data-stu-id="934c8-174">**Skip After** - The number of seconds that the image should be skipped after</span></span>

<span data-ttu-id="934c8-175">**视频**</span><span class="sxs-lookup"><span data-stu-id="934c8-175">**Video**</span></span>

<span data-ttu-id="934c8-176">视频可以通过 Twitch 和 DLive 托管视频或实时流。</span><span class="sxs-lookup"><span data-stu-id="934c8-176">Videos can be hosted videos or live streams through Twitch and DLive.</span></span>  <span data-ttu-id="934c8-177"> (其他支持可能执行额外的工作来获取正确的流 URL，但在多媒体控制台中并不完全支持) </span><span class="sxs-lookup"><span data-stu-id="934c8-177">(Other support may function with extra work to get the proper stream url, but aren't fully supported within the Multimedia Console)</span></span>

* <span data-ttu-id="934c8-178">**名称** - (标识) 的必需名称。</span><span class="sxs-lookup"><span data-stu-id="934c8-178">**Name** - (Required) Name that you wish to identify the video with.</span></span>
* <span data-ttu-id="934c8-179">**视频 URL** - (必需) 用于托管视频的公共 URL，或者提供实时流。</span><span class="sxs-lookup"><span data-stu-id="934c8-179">**Video URL** - (Required) The public url that the video is hosted at or the live stream is served from.</span></span>
* <span data-ttu-id="934c8-180">**在** 之后跳过 - 在之后应跳过视频的秒数</span><span class="sxs-lookup"><span data-stu-id="934c8-180">**Skip After** - The number of seconds that the video should be skipped after</span></span>

> [!NOTE]
> <span data-ttu-id="934c8-181">必需：将时间置于与视频长度匹配的时间，使视频能够正确转发。</span><span class="sxs-lookup"><span data-stu-id="934c8-181">REQUIRED: Put in the time that matches the length of the video to enable videos to properly forward.</span></span> <span data-ttu-id="934c8-182">例如，如果视频长 5 分钟，则 300 秒，否则视频不会跳到下一部分内容。</span><span class="sxs-lookup"><span data-stu-id="934c8-182">For example, if your video is 5 minutes long put 300 seconds, otherwise your video won't skip to the next piece of content.</span></span>

* <span data-ttu-id="934c8-183">**音量** - 视频的音量（从 0 开始 (分钟) - 1 (最大) 值。</span><span class="sxs-lookup"><span data-stu-id="934c8-183">**Volume** - The volume of the video from 0 (min) - 1 (max) values.</span></span>
* <span data-ttu-id="934c8-184">**开始时间** - 从视频开始开始的秒数。</span><span class="sxs-lookup"><span data-stu-id="934c8-184">**Start Time** - The number of seconds from the beginning of the video start from.</span></span>
* <span data-ttu-id="934c8-185">**关闭起始距离** - 离开多媒体控制台时，音量开始下降的距离（以米为单位）</span><span class="sxs-lookup"><span data-stu-id="934c8-185">**Roll Off Start Distance** - The distance in meters in world that the volume begins to fall off at as you move away from the Multimedia Console</span></span>
* <span data-ttu-id="934c8-186">**视频结束操作** - 到达视频末尾后要执行的操作。</span><span class="sxs-lookup"><span data-stu-id="934c8-186">**End of Video Action** - The action to take once the end of the video is reached.</span></span>
    * <span data-ttu-id="934c8-187">停止 - 视频结束后，媒体列表停止</span><span class="sxs-lookup"><span data-stu-id="934c8-187">Stop - The media list stops after the video has ended</span></span>
    * <span data-ttu-id="934c8-188">循环 - 视频将循环，直到手动跳过</span><span class="sxs-lookup"><span data-stu-id="934c8-188">Loop - The video will loop until manually skipped</span></span>
    * <span data-ttu-id="934c8-189">下一步播放 - 媒体列表中的下一个媒体将在当前视频结束后启动。</span><span class="sxs-lookup"><span data-stu-id="934c8-189">Play Next - The next media in the media list will be started after the current video ends.</span></span>

## <a name="working-with-json-directly-advancedoptional"></a><span data-ttu-id="934c8-190">直接使用 JSON (高级/可选) </span><span class="sxs-lookup"><span data-stu-id="934c8-190">Working with JSON directly (advanced/optional)</span></span>

<span data-ttu-id="934c8-191">多媒体控制台支持在 AltspaceVR 中的控制台提示符下直接输入 JSON。</span><span class="sxs-lookup"><span data-stu-id="934c8-191">The Multimedia Console supports entering JSON directly in to the prompt of the console in AltspaceVR.</span></span>  <span data-ttu-id="934c8-192">JSON 是启用媒体播放器配置的内部机制。</span><span class="sxs-lookup"><span data-stu-id="934c8-192">JSON is the internal mechanism with which we enable media player configurations.</span></span> <span data-ttu-id="934c8-193">公开直接设置 JSON 的能力可让更高级的用户构建自己的工作流，以满足其需求和熟悉 JSON。</span><span class="sxs-lookup"><span data-stu-id="934c8-193">Exposing the ability to set JSON directly is something that allows for more advanced users to build their own workflows that suites their needs and familiarity with JSON.</span></span>  <span data-ttu-id="934c8-194">下面简要描述了 JSON 结构和 JSON 的验证架构。</span><span class="sxs-lookup"><span data-stu-id="934c8-194">The following is a brief description of the JSON structure and the schema by which the JSON is validated.</span></span> <span data-ttu-id="934c8-195">有关以下属性的更详细说明，请参阅上述部分，其中介绍了如何配置多媒体控制台。</span><span class="sxs-lookup"><span data-stu-id="934c8-195">For more detailed descriptions of the properties below, see the above sections that talk about configuring the Multimedia Console.</span></span>  <span data-ttu-id="934c8-196">本部分主要介绍 JSON 数据的架构示例和结构。</span><span class="sxs-lookup"><span data-stu-id="934c8-196">This section is focused primarily on the schema examples and structuring for the JSON data.</span></span>

### <a name="global-media-settings"></a><span data-ttu-id="934c8-197">全局媒体设置</span><span class="sxs-lookup"><span data-stu-id="934c8-197">Global media settings</span></span>

```json
{
  "loopMediaList": true | false
  "startMethod": "manual" | "autostart-beginning" | "autostart-random"
  "controlMediaPlayer": "everyone" | "elevated" | "owner"
  "configureMediaPlayer": "elevated" | "owner"
  ...
}
```

### <a name="media-list"></a><span data-ttu-id="934c8-198">媒体列表</span><span class="sxs-lookup"><span data-stu-id="934c8-198">Media list</span></span>

<span data-ttu-id="934c8-199">媒体列表是在 JSON 结构的根目录下设置的属性，如角色和播放设置。</span><span class="sxs-lookup"><span data-stu-id="934c8-199">The media list is a property set at the root of the JSON structure like the Roles and Playback Settings.</span></span>  <span data-ttu-id="934c8-200">它是一个简单的数组，可以包含以下媒体配置结构之一。</span><span class="sxs-lookup"><span data-stu-id="934c8-200">It's a simple array that can contain one of the following media configuration structures.</span></span> <span data-ttu-id="934c8-201"> (请参阅上述属性说明，详细了解每个功能) </span><span class="sxs-lookup"><span data-stu-id="934c8-201">(See property descriptions above for details on what each does.)</span></span>

<span data-ttu-id="934c8-202">**图像示例**</span><span class="sxs-lookup"><span data-stu-id="934c8-202">**Image example**</span></span>

<span data-ttu-id="934c8-203">*必填字段："name"和"imageUrl"*</span><span class="sxs-lookup"><span data-stu-id="934c8-203">*Required fields: "name" and "imageUrl"*</span></span>

```json
{
    "name": "Altspace Screenshot",
    "imageUrl": "https://pbs.twimg.com/media/CxJ-fJqUsAAFtd9.jpg",
    "skipAfter": 10
}
```

<span data-ttu-id="934c8-204">**视频示例**</span><span class="sxs-lookup"><span data-stu-id="934c8-204">**Video example**</span></span>

<span data-ttu-id="934c8-205">*必填字段："name"和"videoUrl"*</span><span class="sxs-lookup"><span data-stu-id="934c8-205">*Required fields: "name" and "videoUrl"*</span></span>

```json
{
    "name": "Ninja Twitch Live Stream",
    "videoUrl":"https://www.twitch.tv/ninja",
    "volume":0.2,
    "startTime":0,
    "endOfVideoAction":"play-next"
}
```

### <a name="example-json"></a><span data-ttu-id="934c8-206">示例 JSON</span><span class="sxs-lookup"><span data-stu-id="934c8-206">Example JSON</span></span>

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

### <a name="schema"></a><span data-ttu-id="934c8-207">架构</span><span class="sxs-lookup"><span data-stu-id="934c8-207">Schema</span></span>

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
> <span data-ttu-id="934c8-208">多媒体控制台 v0.5.0 是最新的</span><span class="sxs-lookup"><span data-stu-id="934c8-208">Up to date with Multimedia Console v0.5.0</span></span>