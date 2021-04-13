---
title: 上传自定义工具包
description: 了解如何在 AltspaceVR 中设置、生成和上传自己的自定义工具包以及故障排除帮助。
ms.date: 03/11/2021
ms.topic: article
keywords: 工具包，上传，故障排除
ms.openlocfilehash: e5a1b9c2ef5339db0cb821cb6f7d21a930416451
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212077"
---
# <a name="uploading-custom-kits"></a><span data-ttu-id="f8567-104">上传自定义工具包</span><span class="sxs-lookup"><span data-stu-id="f8567-104">Uploading custom kits</span></span>

<span data-ttu-id="f8567-105">世界编辑器包含可在世界中生成的项目。</span><span class="sxs-lookup"><span data-stu-id="f8567-105">The World Editor has Kits containing Artifacts that you can spawn into your World.</span></span> <span data-ttu-id="f8567-106">例如， [Campfire 工具包](https://account.altvr.com/kits/993516233267609824) 有多种类型的树，每种类型的树都是一个项目。</span><span class="sxs-lookup"><span data-stu-id="f8567-106">For example, the [Campfire Kit](https://account.altvr.com/kits/993516233267609824) has many types of trees--each type of tree is an Artifact.</span></span> <span data-ttu-id="f8567-107">若要创建自己的工具包，必须创建 Unity AssetBundles 并上载包含每个项目的 Unity Prefab 的 .zip 文件，并在我们的网站上注册每个项目。</span><span class="sxs-lookup"><span data-stu-id="f8567-107">To create your own Kit, you have to create Unity AssetBundles and upload a .zip file containing a Unity Prefab for each Artifact and register each Artifact on our website.</span></span> <span data-ttu-id="f8567-108">幸运的是，社区驱动的 Unity 上载程序可自动执行大部分工作流。</span><span class="sxs-lookup"><span data-stu-id="f8567-108">Fortunately, the community-driven Unity Uploader automates most of the workflow.</span></span> <span data-ttu-id="f8567-109">上传后，你可以在世界中从自己的工具包生成对象，其他用户可以自动查看它们。</span><span class="sxs-lookup"><span data-stu-id="f8567-109">Once uploaded, you can spawn objects from your own Kits in your Worlds and other users can automatically see them.</span></span> <span data-ttu-id="f8567-110">稍后，你可以与朋友分享你的工具包，甚至可以通过功能来与整个社区共享你的工具包。</span><span class="sxs-lookup"><span data-stu-id="f8567-110">Later, you can share your Kit with your friends or even with the entire Community by being featured.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8567-111">先决条件</span><span class="sxs-lookup"><span data-stu-id="f8567-111">Prerequisites</span></span>

1. [<span data-ttu-id="f8567-112">安装 Unity 中心和 Unity</span><span class="sxs-lookup"><span data-stu-id="f8567-112">Install Unity Hub and Unity</span></span>](world-building-toolkit-getting-started.md)
2. <span data-ttu-id="f8567-113">下载最新版本的[Unity 上载](https://altvr.com/download-latest-unity-uploader/)者</span><span class="sxs-lookup"><span data-stu-id="f8567-113">Download the latest version of the [Unity Uploader](https://altvr.com/download-latest-unity-uploader/)</span></span>

## <a name="setup"></a><span data-ttu-id="f8567-114">设置</span><span class="sxs-lookup"><span data-stu-id="f8567-114">Setup</span></span> 

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-my-own-Kits-Part-1-Setup/player]

1. <span data-ttu-id="f8567-115">在我们的网站上的[世界 >](https://account.altvr.com/kits)套件中创建工具包</span><span class="sxs-lookup"><span data-stu-id="f8567-115">Create a Kit on our website at [Worlds > Kits](https://account.altvr.com/kits)</span></span>
2. <span data-ttu-id="f8567-116">将工具包 ID 从浏览器的地址栏复制到剪贴板 (此步骤在第) 版上载程序中更容易</span><span class="sxs-lookup"><span data-stu-id="f8567-116">Copy the Kit ID from your browser's address bar to your clipboard (this step will be easier in Uploader versions 0.9+)</span></span>
3. <span data-ttu-id="f8567-117">创建新的 Unity 项目</span><span class="sxs-lookup"><span data-stu-id="f8567-117">Create a new Unity Project</span></span>
4. <span data-ttu-id="f8567-118">通过双击包导入 Unity 上载程序</span><span class="sxs-lookup"><span data-stu-id="f8567-118">Import the Unity Uploader by double-clicking the package</span></span>

![导入 unity 上载程序包](images/custom-kits-img-01.png)

5. <span data-ttu-id="f8567-120">用你的 Altspace 电子邮件和密码登录到上载程序</span><span class="sxs-lookup"><span data-stu-id="f8567-120">Sign in to the Uploader with your Altspace email and password</span></span>

![Unity 中的 AltspaceVR 登录接口](images/custom-kits-img-02.png)

## <a name="generate-and-upload-your-kit"></a><span data-ttu-id="f8567-122">生成和上传工具包</span><span class="sxs-lookup"><span data-stu-id="f8567-122">Generate and upload your kit</span></span>

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-my-own-Kits-Part-2/player]

1. <span data-ttu-id="f8567-123">使用你的工具包 ID 作为前缀和主题 (填写 **工具包文件夹名称** ，例如 **1137484494681408069_Pirates**) ，并使用你的工具包 Id 作为前缀填写 **包资产名称** 。</span><span class="sxs-lookup"><span data-stu-id="f8567-123">Fill in **Kit Folder Name** with your Kit ID as the prefix and a theme (for example, **1137484494681408069_pirates**) and fill in **Kit Asset Name** with your Kit ID as the prefix.</span></span> <span data-ttu-id="f8567-124">所有资产都需要具有此前缀。</span><span class="sxs-lookup"><span data-stu-id="f8567-124">All the assets will need to have this prefix.</span></span>

![Unity 中的 AltspaceVR 接口，套件文件夹名称](images/custom-kits-img-03.png)

2. <span data-ttu-id="f8567-126">对于每个项目或一组项目：</span><span class="sxs-lookup"><span data-stu-id="f8567-126">For each Artifact or set of Artifacts:</span></span>
* <span data-ttu-id="f8567-127">将源 Prefab (s) 拖到 "层次结构" 选项卡</span><span class="sxs-lookup"><span data-stu-id="f8567-127">Drag your source Prefab(s) into the Hierarchy tab</span></span>
* <span data-ttu-id="f8567-128">选择要包含在集合中的 barrels，例如五种类型的</span><span class="sxs-lookup"><span data-stu-id="f8567-128">Select the ones you want to include in a set, say five types of barrels</span></span>
* <span data-ttu-id="f8567-129">用 **桶** 更新 **工具包资产名称**</span><span class="sxs-lookup"><span data-stu-id="f8567-129">Update the **Kit Asset Name** with **barrel**</span></span>
* <span data-ttu-id="f8567-130">选择 "**将 GameObject (s) 转换为包 Prefab** "</span><span class="sxs-lookup"><span data-stu-id="f8567-130">Select **Convert GameObject(s) to Kit Prefab**</span></span>
* <span data-ttu-id="f8567-131">验证是否在 "资产/Prototyping" 文件夹中创建了新的 Prototyping 和屏幕截图</span><span class="sxs-lookup"><span data-stu-id="f8567-131">Verify that new Prefabs and Screenshots were created in the Assets/Prefabs folder</span></span>

![Unity 中的 AltspaceVR 接口，并选择了项目](images/custom-kits-img-04.png)

> [!NOTE]
> <span data-ttu-id="f8567-133">如果要对生成的 Prefab 进行任何修改，请将其拖回层次结构，进行更改，然后在 "检查器" 选项卡中单击 " **应用** " 以更新 Prefab。</span><span class="sxs-lookup"><span data-stu-id="f8567-133">If you want to make any modifications to a generated Prefab, drag it back into the Hierarchy, make changes, and then click **Apply** in the Inspector tab to update the Prefab.</span></span> 

3. <span data-ttu-id="f8567-134">准备就绪后，在 "上载程序" 选项卡中向下滚动，并准备使用资产捆绑生成 zip 文件</span><span class="sxs-lookup"><span data-stu-id="f8567-134">When you're ready, scroll down the Uploader tab and let's prepare to generate a zip file with the Asset Bundle</span></span>
4. <span data-ttu-id="f8567-135">若要加快迭代速度，请取消勾选 **适用于 Android 的生成工具包？**。</span><span class="sxs-lookup"><span data-stu-id="f8567-135">For faster iteration, uncheck the **Build Kit for Android?**.</span></span> <span data-ttu-id="f8567-136">请记住，稍后在完成迭代或想要共享/功能包时，将生成并上载适用于 Android 的版本。</span><span class="sxs-lookup"><span data-stu-id="f8567-136">Remember to build and upload a version for Android later when you're done iterating or want to share/feature your Kit.</span></span> 
5. <span data-ttu-id="f8567-137">选择 **负载套件 Prefab 目录**</span><span class="sxs-lookup"><span data-stu-id="f8567-137">Select **Load Kit Prefab Directories**</span></span>
6. <span data-ttu-id="f8567-138">选择与工具包文件夹名称匹配的版本旁边的 " **生成** "。</span><span class="sxs-lookup"><span data-stu-id="f8567-138">Choose **Build** next to the one matching your Kit Folder Name.</span></span> <span data-ttu-id="f8567-139">通常从同一 Unity 项目生成多个包。</span><span class="sxs-lookup"><span data-stu-id="f8567-139">It's common to produce multiple Kits from the same Unity project.</span></span> <span data-ttu-id="f8567-140">此过程可能需要一段时间，具体取决于你的工具包大小。</span><span class="sxs-lookup"><span data-stu-id="f8567-140">This may take a while depending on the size of your Kit.</span></span> <span data-ttu-id="f8567-141">完成后，包含 zip 文件的文件夹将自动打开。</span><span class="sxs-lookup"><span data-stu-id="f8567-141">When it's done, the folder containing your zip file will open automatically.</span></span> 
7. <span data-ttu-id="f8567-142">请参阅网站，编辑之前创建的工具包，并上传生成的 zip 文件。</span><span class="sxs-lookup"><span data-stu-id="f8567-142">Go to the website, edit the Kit you created earlier, and upload the zip file you produced.</span></span> <span data-ttu-id="f8567-143">此上传可能需要一段时间，具体取决于文件大小。</span><span class="sxs-lookup"><span data-stu-id="f8567-143">This upload may take a while depending on the file size.</span></span>
    * <span data-ttu-id="f8567-144">如果成功，你会在 "上传" 文件的大小、电脑和 Android 上以及上次更新的时间显示在左侧</span><span class="sxs-lookup"><span data-stu-id="f8567-144">If successful, you’ll see on the left side under “Uploads” the file sizes and for PC and Android and when they were last updated</span></span>
    * <span data-ttu-id="f8567-145">如果不成功，请确保没有任何脚本，我们不支持脚本，我们将检查它们的安全性，然后重试。</span><span class="sxs-lookup"><span data-stu-id="f8567-145">If unsuccessful, make sure you don't have any scripts, we don't support scripts, we check for those for security and try again.</span></span>

<span data-ttu-id="f8567-146">恭喜！</span><span class="sxs-lookup"><span data-stu-id="f8567-146">Congratulations!</span></span> <span data-ttu-id="f8567-147">你已准备好通过自己的工具包构建世界！</span><span class="sxs-lookup"><span data-stu-id="f8567-147">You're ready to build Worlds with your own Kit!</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="f8567-148">疑难解答</span><span class="sxs-lookup"><span data-stu-id="f8567-148">Troubleshooting</span></span> 

<span data-ttu-id="f8567-149">**是否有限制？**</span><span class="sxs-lookup"><span data-stu-id="f8567-149">**Are there limits?**</span></span>
<span data-ttu-id="f8567-150">尚无硬性限制，但请记住，即使只使用了一个项目，用户也需要为整个工具包下载其平台的 AssetBundle。</span><span class="sxs-lookup"><span data-stu-id="f8567-150">There are no hard limits yet but remember that users need to download the AssetBundle for their platform for the entire Kit even if only one Artifact is used.</span></span> <span data-ttu-id="f8567-151">尝试将每个平台的下载保持在 5 MB 或更少。</span><span class="sxs-lookup"><span data-stu-id="f8567-151">Try to keep the download per-platform to 5 MB or less.</span></span> <span data-ttu-id="f8567-152">实现此目的的一种方法是将其拆分为较小的工具包。</span><span class="sxs-lookup"><span data-stu-id="f8567-152">One way to do that is to split up things into smaller Kits.</span></span> <span data-ttu-id="f8567-153">例如，200属性应分成一半。</span><span class="sxs-lookup"><span data-stu-id="f8567-153">For example, 200 props should split in half.</span></span> 

<span data-ttu-id="f8567-154">**看到 "分割眼睛"？**</span><span class="sxs-lookup"><span data-stu-id="f8567-154">**Seeing “split eye”?**</span></span>
<span data-ttu-id="f8567-155">重新导入最新的上载者以获取正确的呈现设置</span><span class="sxs-lookup"><span data-stu-id="f8567-155">Reimport the latest Uploader to get the right rendering settings</span></span>

<span data-ttu-id="f8567-156">**更新/更改未反映？**</span><span class="sxs-lookup"><span data-stu-id="f8567-156">**Updates/changes not reflected?**</span></span>
    * <span data-ttu-id="f8567-157">检查工具包页上的更新时间</span><span class="sxs-lookup"><span data-stu-id="f8567-157">Check the updated time on the Kit page</span></span>
    * <span data-ttu-id="f8567-158">重新进入世界将无法正常工作-重新启动客户端。</span><span class="sxs-lookup"><span data-stu-id="f8567-158">Reentering the World will not work-- restart client.</span></span> <span data-ttu-id="f8567-159">甚至可能需要几分钟的时间来更新</span><span class="sxs-lookup"><span data-stu-id="f8567-159">Even then it may take a few minutes to update</span></span>
    * <span data-ttu-id="f8567-160">请确保文件夹名称或 prefab 名称中没有空格 **，例如 "party_favors" 与 "参与方优先"**</span><span class="sxs-lookup"><span data-stu-id="f8567-160">Make sure there are no spaces in your folder names or prefab names **for example, 'party_favors' vs 'party favors'**</span></span>

<span data-ttu-id="f8567-161">虽然 **我有一个脚本，但** AssetBundle 浏览器有时会自动包含文件。</span><span class="sxs-lookup"><span data-stu-id="f8567-161">**It keeps saying I have a script but I don't** The AssetBundle Browser automatically includes files sometimes.</span></span> <span data-ttu-id="f8567-162">尝试隔离正在引入的模型。</span><span class="sxs-lookup"><span data-stu-id="f8567-162">Try to isolate the model you're bringing in.</span></span> <span data-ttu-id="f8567-163">例如，请勿将其拖放到其他 Prefab 的一部分</span><span class="sxs-lookup"><span data-stu-id="f8567-163">For example, don't drag it in when it's part of another Prefab already</span></span>

<span data-ttu-id="f8567-164">**如何处理粒子系统和动画？**</span><span class="sxs-lookup"><span data-stu-id="f8567-164">**What about Particle Systems and Animations?**</span></span>
<span data-ttu-id="f8567-165">对于这些情况，接下来，将在1x1x1 多维数据集下定位到网格呈现并禁用冲突。</span><span class="sxs-lookup"><span data-stu-id="f8567-165">For these, next them under a 1x1x1 Cube positioned at the origin with Mesh Rendering and Collision disabled.</span></span> <span data-ttu-id="f8567-166">粒子系统应启用循环并且应将其 **缩放** 设置为 **层次结构** ，以便能够正确地在 Altspace 中进行缩放。</span><span class="sxs-lookup"><span data-stu-id="f8567-166">Particle Systems should have looping enabled and **Scaling** should be set to **Hierarchy** so that we can scale them in Altspace properly.</span></span> <span data-ttu-id="f8567-167">为所有动画生成 prototyping 后，对每个动画的 **冲突** 对象禁用冲突。</span><span class="sxs-lookup"><span data-stu-id="f8567-167">After you generate the prefabs for all the animations, disable the collisions on the **collision** objects for each.</span></span>

<span data-ttu-id="f8567-168">**项目很暗** 您是否已将模型的材料着色器设置为 **仅限点即点即点光**？</span><span class="sxs-lookup"><span data-stu-id="f8567-168">**The Artifacts are dark** Did you set the model's material shader to **Mobile/Vertex lit-only directional lights**?</span></span>

<span data-ttu-id="f8567-169">**项目不是正确的方法** 旋转 **模型** 和 **碰撞** 器并更新 Prefab。</span><span class="sxs-lookup"><span data-stu-id="f8567-169">**The Artifact isn't facing the right way** Rotate the **model** and **collider** and update the Prefab.</span></span> <span data-ttu-id="f8567-170">旋转父级不会执行任何操作，这会被忽略。</span><span class="sxs-lookup"><span data-stu-id="f8567-170">Rotating the parent won't do anything--that's ignored.</span></span> <span data-ttu-id="f8567-171">您可以使用 " **旋转覆盖** " 字段轻松完成此操作。</span><span class="sxs-lookup"><span data-stu-id="f8567-171">You can use the **Rotation Override** field to do this easily.</span></span>

<span data-ttu-id="f8567-172">**这些项目是否可以与 SDK 的 **CreateFromLibrary** 函数一起使用？**</span><span class="sxs-lookup"><span data-stu-id="f8567-172">**Can these Artifacts be used with the SDK's **CreateFromLibrary** function?**</span></span>
<span data-ttu-id="f8567-173">是</span><span class="sxs-lookup"><span data-stu-id="f8567-173">Yes</span></span>