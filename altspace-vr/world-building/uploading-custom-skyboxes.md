---
title: 上传自定义 Skyboxes
description: 获取有关在 AltspaceVR 体验中上载和排查自定义 skyboxes 的分步说明。
ms.date: 03/11/2021
ms.topic: article
keywords: skyboxes，故障排除
ms.openlocfilehash: 02d5bc762dc36d4195100e8155d6250789e833f7
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212018"
---
# <a name="uploading-custom-skyboxes"></a><span data-ttu-id="ecbec-104">上传自定义 Skyboxes</span><span class="sxs-lookup"><span data-stu-id="ecbec-104">Uploading custom Skyboxes</span></span>

<span data-ttu-id="ecbec-105">Skybox 是一种为世界创建 **背景** 的方式，使体验更具沉浸。</span><span class="sxs-lookup"><span data-stu-id="ecbec-105">A Skybox is a way to create a **background** for your World that makes the experience more immersive.</span></span> <span data-ttu-id="ecbec-106">Skyboxes 有不同种类，但目前支持 **equirectangular**。</span><span class="sxs-lookup"><span data-stu-id="ecbec-106">There are different kinds of Skyboxes but we currently support **equirectangular**.</span></span> <span data-ttu-id="ecbec-107">下面是使用360照相机创建的示例 (更多示例[) ：](http://moments.mankindforward.com/)</span><span class="sxs-lookup"><span data-stu-id="ecbec-107">Here's an example taken with a 360 camera (more example [here](http://moments.mankindforward.com/)):</span></span> 

![360 equirectangular 的视图](images/custom-skyboxes-img-01.jpeg)

<span data-ttu-id="ecbec-109">你还可以使用 [Unity 上载](world-building-toolkit-getting-started.md) ，但此方法更简单。</span><span class="sxs-lookup"><span data-stu-id="ecbec-109">You can also use the [Unity Uploader](world-building-toolkit-getting-started.md) but this approach is simpler.</span></span>

1. <span data-ttu-id="ecbec-110">导航到 " [世界 > Skyboxes](https://account.altvr.com/skyboxes) "，然后按右侧的 " **创建** " 按钮</span><span class="sxs-lookup"><span data-stu-id="ecbec-110">Navigate to [Worlds > Skyboxes](https://account.altvr.com/skyboxes) and press the **Create** button on the right</span></span>

![世界网站页面打开到 skyboxes 面板](images/custom-skyboxes-img-02.png)

2. <span data-ttu-id="ecbec-112">填写名称并指定360映像。</span><span class="sxs-lookup"><span data-stu-id="ecbec-112">Fill in a name and specify your 360 image.</span></span> <span data-ttu-id="ecbec-113">这不一定是一张照片，有一些程序可以让你自行绘制，或者可以搜索一些在线。</span><span class="sxs-lookup"><span data-stu-id="ecbec-113">It doesn't have to be a photo, there are programs that let you draw your own or you can search for some online.</span></span> <span data-ttu-id="ecbec-114">准备就绪后，选择“创建”。</span><span class="sxs-lookup"><span data-stu-id="ecbec-114">When you're ready, select **Create**.</span></span> 

![Skybox 创建窗体](images/custom-skyboxes-img-03.png)

3. <span data-ttu-id="ecbec-116">您可以选择上传 **预览** 图像，以便您可以轻松识别此 skybox。</span><span class="sxs-lookup"><span data-stu-id="ecbec-116">You can optionally upload a **preview** image so you can easily identify this skybox.</span></span> <span data-ttu-id="ecbec-117">你还可以上载 WAV 格式的环境音频。</span><span class="sxs-lookup"><span data-stu-id="ecbec-117">You can also upload ambient audio in WAV format.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="ecbec-118">建议你在上载360映像后分别上传预览图像和环境音频。</span><span class="sxs-lookup"><span data-stu-id="ecbec-118">We recommend you upload preview images and ambient audio separately, after you upload the 360 image.</span></span> <span data-ttu-id="ecbec-119">如果将这些文件上传到一起，则文件大小可能会足够大以使进程停止。</span><span class="sxs-lookup"><span data-stu-id="ecbec-119">If you upload them together the file sizes can be large enough to stall the process.</span></span> <span data-ttu-id="ecbec-120">[Jetsons World](https://account.altvr.com/worlds/1004174988393054363/spaces/1084431533181240311) 是如何使用带有环境音频的 Skybox 的一个很好的示例。</span><span class="sxs-lookup"><span data-stu-id="ecbec-120">[Jetsons World](https://account.altvr.com/worlds/1004174988393054363/spaces/1084431533181240311) is a great example of how to use a Skybox with ambient audio.</span></span> <span data-ttu-id="ecbec-121">请注意，世界构建器如何保持音频音量低、听听声音非常小，使人们不会收到厌恶。</span><span class="sxs-lookup"><span data-stu-id="ecbec-121">Notice how the World-Builder kept the audio volume low and sounds you hear are sporadic so people don't get annoyed.</span></span> 

4. <span data-ttu-id="ecbec-122">输入您的世界并打开 "世界" 编辑器。</span><span class="sxs-lookup"><span data-stu-id="ecbec-122">Enter your World and open the World Editor.</span></span> <span data-ttu-id="ecbec-123">在 "Skyboxes" 下，选择新的 Skybox。</span><span class="sxs-lookup"><span data-stu-id="ecbec-123">Under Skyboxes, select your new Skybox.</span></span> <span data-ttu-id="ecbec-124">几秒钟后，天空会按原义发生变化。</span><span class="sxs-lookup"><span data-stu-id="ecbec-124">In a few seconds, the sky will literally change.</span></span> <span data-ttu-id="ecbec-125">世界上的其他人也会看到天空发生变化。</span><span class="sxs-lookup"><span data-stu-id="ecbec-125">Others in your World will also see the sky change.</span></span> <span data-ttu-id="ecbec-126">若要切换回来，请选择同一列表中的 **默认** skybox。</span><span class="sxs-lookup"><span data-stu-id="ecbec-126">To switch back, choose the **default** skybox in that same list.</span></span> 

## <a name="troubleshooting"></a><span data-ttu-id="ecbec-127">疑难解答</span><span class="sxs-lookup"><span data-stu-id="ecbec-127">Troubleshooting</span></span>

<span data-ttu-id="ecbec-128">**天空中有接缝或直线：- (。**</span><span class="sxs-lookup"><span data-stu-id="ecbec-128">**There's a seam or line in the sky :-(.**</span></span> <span data-ttu-id="ecbec-129">这是我们即将解决的 bug</span><span class="sxs-lookup"><span data-stu-id="ecbec-129">It's a bug that we'll fix soon</span></span>

<span data-ttu-id="ecbec-130">**上载失败**</span><span class="sxs-lookup"><span data-stu-id="ecbec-130">**Upload failed**</span></span>
    * <span data-ttu-id="ecbec-131">尝试自行仅上载360映像</span><span class="sxs-lookup"><span data-stu-id="ecbec-131">try uploading just the 360 image on its own</span></span>
    * <span data-ttu-id="ecbec-132">尝试使用另一个较小的文件作为测试</span><span class="sxs-lookup"><span data-stu-id="ecbec-132">try with another, smaller file as a test</span></span>

<span data-ttu-id="ecbec-133">**我找不到360照片**</span><span class="sxs-lookup"><span data-stu-id="ecbec-133">**I can't find a 360 photo**</span></span>
    * <span data-ttu-id="ecbec-134">Flickr 是良好的源 (更改筛选器以查找创造性的 commons) </span><span class="sxs-lookup"><span data-stu-id="ecbec-134">Flickr is a good source (change the filters to find creative commons ones)</span></span>
    * <span data-ttu-id="ecbec-135">自行学习！</span><span class="sxs-lookup"><span data-stu-id="ecbec-135">Take your own!</span></span> <span data-ttu-id="ecbec-136">我们已成功完成了 Ricoh 的相机。</span><span class="sxs-lookup"><span data-stu-id="ecbec-136">We've had success with Ricoh's cameras.</span></span> 
<span data-ttu-id="ecbec-137">**天空看起来有纹理或 blocky** 可能需要查找更高分辨率的图像。</span><span class="sxs-lookup"><span data-stu-id="ecbec-137">**The sky looks grainy or blocky** You may need to find a higher-resolution image.</span></span> <span data-ttu-id="ecbec-138">通常约 2-5 MB，~ 5000 px x 2000 px</span><span class="sxs-lookup"><span data-stu-id="ecbec-138">Typically around 2-5 MB and ~5000 px x 2000 px</span></span>

<span data-ttu-id="ecbec-139">**这会影响我世界的帧速率！**</span><span class="sxs-lookup"><span data-stu-id="ecbec-139">**It hurts my World's framerate!**</span></span>
<span data-ttu-id="ecbec-140">映像可能太大。</span><span class="sxs-lookup"><span data-stu-id="ecbec-140">The image is probably too large.</span></span> <span data-ttu-id="ecbec-141">某些生成的 skyboxes 可能是8k。</span><span class="sxs-lookup"><span data-stu-id="ecbec-141">Some generated skyboxes can be 8k.</span></span> <span data-ttu-id="ecbec-142">它们通常附带移动友好的2k 版本--使用该版本。</span><span class="sxs-lookup"><span data-stu-id="ecbec-142">They usually come with mobile-friendly 2k versions--use that.</span></span>

<span data-ttu-id="ecbec-143">**帮助我了解环境音频**</span><span class="sxs-lookup"><span data-stu-id="ecbec-143">**Help me with the ambient audio**</span></span>
    * <span data-ttu-id="ecbec-144">使用 Audacity 等免费软件来降低音量或创建自己的循环。</span><span class="sxs-lookup"><span data-stu-id="ecbec-144">Use free software like Audacity to lower the volume or create your own loops.</span></span> <span data-ttu-id="ecbec-145">请记住，音频会重复并在人们的耳中播放，因此保持较低且不令人讨厌</span><span class="sxs-lookup"><span data-stu-id="ecbec-145">Remember that the audio will be repeated and playing in people's ears so keep it low and not annoying</span></span>
    * <span data-ttu-id="ecbec-146">[免费音响](https://freesound.org/) 是合理的免版税声音来源</span><span class="sxs-lookup"><span data-stu-id="ecbec-146">[Free Sound](https://freesound.org/) is a good source of royalty-free sounds</span></span>
