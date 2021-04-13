---
title: 导入 glTF 模型
description: 了解如何将 3D glTF 模型正确地导入 AltspaceVR 体验，并解决任何问题。
ms.date: 03/11/2021
ms.topic: article
keywords: 模型，glTF，导入，sketchfab，故障排除
ms.openlocfilehash: 4489f90832bd1cf85ff161caed11684257cce6ab
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212017"
---
# <a name="importing-gltf-models"></a><span data-ttu-id="32787-104">导入 glTF 模型</span><span class="sxs-lookup"><span data-stu-id="32787-104">Importing glTF models</span></span>

> [!NOTE]
> <span data-ttu-id="32787-105">此功能在 "早期访问" 计划中可用于选择用户。</span><span class="sxs-lookup"><span data-stu-id="32787-105">This feature is available for select users in the Early Access program at this time.</span></span>

<span data-ttu-id="32787-106">将三维模型和场景引入 Altspace 的一种方法是使用 [glTF 标准](https://en.wikipedia.org/wiki/GlTF)。</span><span class="sxs-lookup"><span data-stu-id="32787-106">One way to bring 3D models and scenes into Altspace is using the [glTF standard](https://en.wikipedia.org/wiki/GlTF).</span></span> <span data-ttu-id="32787-107">您可以上载 (打包的 glTF) 的 glb 文件，以创建以后在世界编辑器中生成的模型。</span><span class="sxs-lookup"><span data-stu-id="32787-107">You can upload a .glb file (packed glTF) to create a Model that you can later spawn in the World Editor.</span></span> <span data-ttu-id="32787-108">这是 [上传自己的工具包](uploading-custom-kits.md)的替代方法。</span><span class="sxs-lookup"><span data-stu-id="32787-108">It's an alternative to [uploading your own Kits](uploading-custom-kits.md).</span></span> <span data-ttu-id="32787-109">建议为快速演示创建模型，因为当你想要最大程度地提高性能和可重用性时，无需使用 Unity 和工具包。</span><span class="sxs-lookup"><span data-stu-id="32787-109">We recommend creating Models for quick demonstrations because you won't need to use Unity, and Kits when you want to maximize performance and reusability.</span></span> 

1. <span data-ttu-id="32787-110">查找一些 glTF 3D 资产。</span><span class="sxs-lookup"><span data-stu-id="32787-110">Find some glTF 3D assets.</span></span> <span data-ttu-id="32787-111">要搜索的一个位置是 Sketchfab (尝试 [按如下所示筛选](https://sketchfab.com/search?features=downloadable&q=low+poly+wolf&sort_by=-pertinence&type=models)**可下载** 模型) 。</span><span class="sxs-lookup"><span data-stu-id="32787-111">One place to search is Sketchfab (try filtering for **Downloadable** models like [this](https://sketchfab.com/search?features=downloadable&q=low+poly+wolf&sort_by=-pertinence&type=models)).</span></span> <span data-ttu-id="32787-112">找到后，选择 " **下载3D 模型**"：</span><span class="sxs-lookup"><span data-stu-id="32787-112">Once you find it, select **Download 3D Model**:</span></span>

![Sketchfab 中的3D 狗模型](images/importing-models-img-01.png)

2. <span data-ttu-id="32787-114">将链接复制到模型并阅读许可要求。</span><span class="sxs-lookup"><span data-stu-id="32787-114">Copy the link to the model and read the licensing requirements.</span></span> 
3. <span data-ttu-id="32787-115">下载 **Autoconverted 格式 (glTF)** 版本</span><span class="sxs-lookup"><span data-stu-id="32787-115">Download the **Autoconverted Format (glTF)** version</span></span>

![突出显示自动转换格式的 Sketchfab 下载选项](images/importing-models-img-02.png)

4. <span data-ttu-id="32787-117">打开 [GLB Packer](https://glb-packer.glitch.me) 网站并选中 " **将 PNG 转换为 JPEG (beta)**</span><span class="sxs-lookup"><span data-stu-id="32787-117">Open the [GLB Packer](https://glb-packer.glitch.me) site and check the box **Convert PNG to JPEG (beta)**</span></span>
5. <span data-ttu-id="32787-118">解压缩你下载的 glTF 文件，并将其一次性拖到 GLB Packer 浏览器选项卡中</span><span class="sxs-lookup"><span data-stu-id="32787-118">Uncompress the glTF files you downloaded and drag them all at once into the GLB Packer browser tab</span></span>

![显示模型解压缩的窗口](images/importing-models-img-03.png)

6. <span data-ttu-id="32787-120">处理过程可能需要一段时间，具体取决于文件的数量和大小。</span><span class="sxs-lookup"><span data-stu-id="32787-120">Depending on the number and size of the files, it may take a while to process.</span></span> <span data-ttu-id="32787-121">处理完成后，将下载 **glb** 文件。</span><span class="sxs-lookup"><span data-stu-id="32787-121">When processing is done, an **out.glb** file will be downloaded.</span></span> <span data-ttu-id="32787-122">将该文件重命名为信息性信息--这将是世界 (的对象的名称，例如 **Low Poly 狼. glb**) </span><span class="sxs-lookup"><span data-stu-id="32787-122">Rename that file to something informative--this will be the name of the object in the world (e.g **Low Poly Wolf.glb**)</span></span>
7. <span data-ttu-id="32787-123">导航到 [altvr.com > 更多 > 模型](https://account.altvr.com/users/sign_in)并选择 "**创建**"</span><span class="sxs-lookup"><span data-stu-id="32787-123">Navigate to [altvr.com > More > Models](https://account.altvr.com/users/sign_in) and select **Create**</span></span>
8. <span data-ttu-id="32787-124">指定 glb 文件的位置，并确保将 Sketchfab 链接复制到 "归属说明"。</span><span class="sxs-lookup"><span data-stu-id="32787-124">Specify the location of the .glb file and make sure you copy the Sketchfab link into the description for attribution.</span></span> <span data-ttu-id="32787-125">如果需要，可以指定预览图像，然后选择 " **创建模型**"：</span><span class="sxs-lookup"><span data-stu-id="32787-125">You can specify a preview image if you want, then select **Create Model**:</span></span>

![AltspaceVR 中的模型预览](images/importing-models-img-04.png)

9. <span data-ttu-id="32787-127">选择 "**复制到剪贴板**"</span><span class="sxs-lookup"><span data-stu-id="32787-127">Select **Copy to Clipboard**</span></span>
10. <span data-ttu-id="32787-128">打开 **世界编辑器 > Altspace > 基础知识 > GLTF**</span><span class="sxs-lookup"><span data-stu-id="32787-128">Open the **World Editor > Altspace > Basics > GLTF**</span></span>
11. <span data-ttu-id="32787-129">粘贴到 url，然后选择 "**确认**"</span><span class="sxs-lookup"><span data-stu-id="32787-129">Paste in your url and select **Confirm**</span></span>

<span data-ttu-id="32787-130">恭喜！</span><span class="sxs-lookup"><span data-stu-id="32787-130">Congrats!</span></span> <span data-ttu-id="32787-131">你只是生成了第一个模型。</span><span class="sxs-lookup"><span data-stu-id="32787-131">You just spawned your first Model.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="32787-132">疑难解答</span><span class="sxs-lookup"><span data-stu-id="32787-132">Troubleshooting</span></span>

<span data-ttu-id="32787-133">**单击 " **确认** 没有发生"**</span><span class="sxs-lookup"><span data-stu-id="32787-133">**When I clicked **Confirm** nothing happened**</span></span>
    * <span data-ttu-id="32787-134">目前有10万个多边形限制。</span><span class="sxs-lookup"><span data-stu-id="32787-134">We currently have a 100k polygon limit.</span></span> <span data-ttu-id="32787-135">如果此操作失败，请删除对象，以避免在加入你的用户时出现潜在问题</span><span class="sxs-lookup"><span data-stu-id="32787-135">If it fails, delete the Object to avoid potential problems with users joining your World</span></span>
    * <span data-ttu-id="32787-136">资产可能还有其他问题。</span><span class="sxs-lookup"><span data-stu-id="32787-136">There may be other problems with the asset.</span></span> <span data-ttu-id="32787-137">尝试使用尽可能少多边形的资产。</span><span class="sxs-lookup"><span data-stu-id="32787-137">Try to use assets with as few polygons as possible.</span></span>
    * <span data-ttu-id="32787-138">要引入的模型可能很小，也可能很大。</span><span class="sxs-lookup"><span data-stu-id="32787-138">The model you're bringing in may be small or large.</span></span> <span data-ttu-id="32787-139">尝试增加/减少规模，或四处移动您的头像，你可能会在模型中！</span><span class="sxs-lookup"><span data-stu-id="32787-139">Try increasing/decreasing the Scale or move your avatar around, you might be standing inside the model!</span></span>

<span data-ttu-id="32787-140">**加载速度缓慢** 世界上其他用户的负载速度将取决于其连接速度。</span><span class="sxs-lookup"><span data-stu-id="32787-140">**It's slow to load** How quickly other users in the World load it will depend on their connection speeds.</span></span> <span data-ttu-id="32787-141">它也不缓存，如套件资产。</span><span class="sxs-lookup"><span data-stu-id="32787-141">It's also not cached like Kit assets.</span></span> <span data-ttu-id="32787-142">如果你将其放在家里，则每次加入时，最终都将 redownloading 相同的模型，这种情况并不好。</span><span class="sxs-lookup"><span data-stu-id="32787-142">If you place one in your Home, you'll end up redownloading the same Model every time you join, which isn't great.</span></span>

<span data-ttu-id="32787-143">**无冲突** 默认情况下，不会对以这种方式引入的对象发生冲突</span><span class="sxs-lookup"><span data-stu-id="32787-143">**There's no collision** By default there's no collision on the objects that are brought in this way</span></span>

<span data-ttu-id="32787-144">**当我生成控件时，我在六个 DOF 上失去了控制** 是的，我们意识到这些问题，希望尽快解决这些问题。</span><span class="sxs-lookup"><span data-stu-id="32787-144">**When I spawn it, I lose my controls on six DOF or I'm inside so it's hard to manipulate it** Yes, we're aware of these issues and hope to address them soon.</span></span>  