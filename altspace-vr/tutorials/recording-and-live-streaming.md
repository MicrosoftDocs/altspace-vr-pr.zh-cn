---
title: 记录和实时流式处理
description: 了解如何记录和实时流式传输您的 PC 中的 AltspaceVR 事件，以便升级和与用户共享。
ms.date: 02/10/2021
ms.topic: article
keywords: 流式处理，记录
ms.openlocfilehash: 80d54407915af1a0d4b7783858446f54205e6a2a
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212076"
---
# <a name="recording-and-live-streaming"></a>记录和实时流式处理

记录和实时流式处理你的 AltspaceVR 体验，以便在全球范围内展示你的活动、AltspaceVR 和 VR，这是一个很好的方法。 请查看以下内容了解如何入门：

本文将指导如何进行以下操作：

* [如何在计算机上的2D 模式下录制 AltspaceVR](#recording-altspacevr-in-2d-mode-on-pc)
* [如何在计算机上的2D 模式下实时流到 AltspaceVR 中的 YouTube](#live-streaming-to-youtube-in-altspacevr-2d-mode-on-pc)

## <a name="recording-altspacevr-in-2d-mode-on-pc"></a>在电脑上的2D 模式下录制 AltspaceVR

### <a name="the-short-version"></a>短版本

已安装 AltspaceVR 和 OBS。 在2D 模式下启动 AltspaceVR，启动 OBS，将 OBS 设置为录制 AltspaceVR 并录制！

### <a name="the-slightly-longer-version"></a>略长版本

1. 访问 [https://obsproject.com/](https://obsproject.com/)
2. 选择要下载的 **WINDOWS** OBS。 此文章使用 **OBS v 22.0.2**
3. 安装 OBS

### <a name="have-altspacevr-running-in-2d-mode-before-you-run-obs"></a>在运行 OBS 之前，让 AltspaceVR 在2D 模式下运行

1. 从网站下载并安装 AltspaceVR： [altvr.com/get](https://altvr.com/getaltspacevr)
2. 请确保在2D 模式下启动 AltspaceVR，方法是从 PC 中拔下 HMD 的 USB 电缆，或者如果具有 Rift： Ctrl + Alt + Del、Services、Oculus VR 运行时服务，请右键单击，然后单击 "停止"。 
    * 这将禁用 Oculus 并启动2D 模式下的 AltspaceVR，重复这些步骤并使用 Start 获取 VR 模式。

现在，Alt-Tab 到 OBS：

1. 在 "源" 下，选择 " **+ > 游戏捕获 >** 新建
2. 编辑文本到 "AltspaceVR 捕获"，勾选标记 **使源可见**，然后选择 "确定"
3. 双击 "源" 下的 " **AltspaceVR 捕获** "
4. 用于 **捕获特定窗口** 的更改 **模式**
5. 窗口： [AltspaceVR.exe]： AltspaceVR
6. 窗口匹配优先级：匹配标题，否则查找相同可执行文件的窗口
7. 向下滚动到 "捕获 Cursor： untick"

这会使 AltspaceVR 显示在 OBS 中。 现在若要在 OBS 中设置以下属性，请参阅 **文件 > 设置**：

| 选项卡 | 设置 |
|---|---|
| 常规 | 保留默认值 |
| Stream | 保留默认值 |
| 输出模式：切换到高级 | 流式处理选项卡 <br> 音频轨道1 <br> 编码器： x264 <br> 强制流式处理服务编码器设置：勾选 <br> 重新缩放输出：未选中 <br> 速率控制： CBR <br> 比特率： 6000 (6000 为 30 fps 或 9000 60 fps)  <br> 关键帧间隔 = 2 <br> CPU 使用预设 = veryfast |
| 录制 | 类型：标准 <br> 录制路径： D：/视频 (浏览到想要保存视频文件的位置)  <br> 录制格式：工作方式 (如果你在录制时出现故障，请在此处尝试) 使用 flv 而不是 " <br> 音频轨道1 <br> 编码器：使用流编码器 |
| 音频 | 音频比特率： 160 (所有磁道)  |
| 重播缓冲区 | 保留默认值 |
| 音频 | 采样速率：48khz <br> 频道：立体声 <br> 桌面音频设备：默认 <br> 桌面音频设备2：禁用 <br> Mic/Aux 音频设备：默认值 |
| 视频 | 基本 (画布) 解决方法：1920x1080 <br>  (扩展) 分辨率的输出：1920x1080 <br> 缩减筛选器：双立方 (Sharpened 缩放，16个样本)  <br> 常见 FPS 值：30 |
| 热键 | 保留默认值 |
| 高级 | 进程优先级：正常 |

好了，现在请确保选择 " **应用**"，然后单击 **"确定"** 保存所有 OBS 设置。 

1. Alt-Tab AltspaceVR，进入正确的空间/世界/事件，并将您的相机 (，这就是您的头像) 我们要录制视频！
2. Alt-Tab OBS，当你准备就绪时，单击 " **开始录制**"。

您将看到 OBS 的右下方，它会开始计算，这意味着您正在录制！

使用此内容进行测试记录： 
1. 在 AltspaceVR 中打开/关闭/滚动菜单以创建 UI 声音
2. 说 "Sibilance，Sibilance"，然后让另一个用户在正常音量与您对话，或观看2D 显示的视频。
3. 查看桌面音频和麦克风/Aux 级别，以查看其是否正常工作。

录制时通常会将麦克风/Aux 设为静音。 继续，为 Mic/Aux 选择扬声器图标，该图标将变为红色，其中包含 X。

* 这很难与音频和其他用户的音频匹配，因此麦克风最好是静音。
* 音频的另一个问题是 OBS 的设置方式。 它从您的计算机中捕获所有音频，因此，如果您正在观看 YouTube，则会记录该音频、可宽延的消息或通知声音。
* 若要仅记录来自 AltspaceVR 的音频，请进入卷混合器 (右键单击 Windows) 右下方的扬声器图标，并静音系统声音、浏览器等，但不要将 OBS 或 AltspaceVR 静音。

> [!IMPORTANT]
> 录制后，请不要忘记打开这些音量合成器设置。

现在，请导航回 OBS，并选择 "从文件中 **停止录制** **>显示录制**"。 这会打开包含 OBS 视频文件的文件夹，然后双击测试视频。

有时录音会很大，因此，请降低桌面音频的滑块，并进行另一次记录测试。

<!-- Missing image -->

## <a name="live-streaming-to-youtube-in-altspacevr-2d-mode-on-pc"></a>计算机上 AltspaceVR 2D 模式下的 YouTube 的实时流式处理

### <a name="the-short-version"></a>短版本

已安装 AltspaceVR 和 OBS。 在2D 模式下启动 AltspaceVR，启动 OBS，在 YouTube 上启动，或在 YouTube 上创建 "新建实时事件"，使用你的 YouTube 流密钥设置 OBS，开始流式传输到 YouTube，开始在 YouTube 上流式传输！

### <a name="the-slightly-longer-version"></a>略长版本

1. 访问 [https://obsproject.com/](https://obsproject.com/)
2. 单击 " **Windows** " 下载 OBS， (此文章使用 OBS v 22.0.2) 
3. 安装 OBS

在运行 OBS 之前，让 AltspaceVR 在2D 模式下运行
1. 从我们的网站下载 AltspaceVR： [https://account.altvr.com/downloads](https://account.altvr.com/downloads)
2. 若要确保在2D 模式下启动 AltspaceVR，请从 PC 中拔下 HMD 的 USB 电缆，或使用 Rift： Ctrl + Alt + Del、Services、Oculus VR 运行时服务，右键单击 "停止"。 这将在2D 模式下禁用 Oculus Home 和 start AltspaceVR，重复这些步骤并再次开始获取 VR 模式。

Alt-Tab OBS

1. 在 "源" 下，选择 **+** ，选择 "游戏捕获"，"新建"，然后编辑文本 "AltspaceVR 捕获"，勾选 "使源可见，正常"
2. 双击 "AltspaceVR 捕获"
3. 模式：捕获特定窗口
4. 窗口： [AltspaceVR.exe]： AltspaceVR
5. 窗口匹配优先级：匹配标题，否则查找相同可执行文件的窗口
6. 向下滚动到 "捕获 Cursor： untick"

这会使 AltspaceVR 显示在 OBS 中。 很好！

现在，OBS 转到 File>设置

| 选项卡 | 设置 |
|---|---|
| 常规 | 当流式处理 (时，自动标记会将视频文件记录到计算机，而不是实时流式处理)  |
| Stream | 流类型：流式处理服务 <br> 服务： YouTube/YouTube 游戏 (还可以流式传输到 Twitch、混音器、Facebook Live 等 ) <br>服务器：主要 YouTube 摄取服务器 <br>流密钥：从 YouTube 粘贴你的流密钥 * * (参阅 "实时设置" <br>) 上的 YouTube 流式处理 |
| 输出 | 输出模式：切换到高级 |
| 流式处理 | 音频轨道1 <br>编码器： x264 <br>勾选强制流式处理服务编码器设置 <br>重新缩放输出：未选中 <br>速率控制： CBR <br>比特率： 6000 (6000 为 30 fps 或 9000 60 fps)  <br>关键帧间隔 = 2 <br>CPU 使用预设 = veryfast |
| 录制 | 类型：标准 <br>录制路径： D：/视频 (浏览到你希望视频文件保存到的位置（如果你选择了 "流式处理时自动录制")  <br>录制格式：工作方式 (如果你在录制时出现故障，请在此处尝试) 使用 flv 而不是 " <br>音频轨道1 <br>编码器：使用流编码器 |
| 音频 | 音频比特率： 160 (适用于所有磁道) 采样率：48khz <br>频道：立体声 <br>桌面音频设备：默认 <br>桌面音频设备2：禁用 <br>Mic/Aux 音频设备：默认值 |
| 重播缓冲区 | 保留默认值 |
| 视频 | 基本 (画布) 解决方法：1920x1080 <br> (扩展) 分辨率的输出：1920x1080 <br>缩减筛选器：双立方 (Sharpened 缩放，16个样本)  <br>常见 FPS 值：30 |
| 热键 | 保留默认值 |
| 高级 | 进程优先级：正常 |

好了，现在请确保单击 "应用"，然后单击 "确定"，然后关闭并重新打开 OBS。 这会保存所有 OBS 设置。 看起来不错： ) 

请参阅上面的 "如何在计算机上的2D 模式下记录 AltspaceVR" 部分，了解如何使用本地记录（而不是实时流）测试录制，并说明如何在录制前首先获取照相机快照设置。

音频的另一个问题是 OBS 的设置方式。 它从计算机中捕获所有音频，因此，如果您正在观看 YouTube，则会记录该音频、团队消息或通知声音。

若要仅记录来自 AltspaceVR 的音频，请进入卷混合器 (右键单击 Windows) 右下方的扬声器图标，并静音系统声音、浏览器等，但不要将 OBS 或 AltspaceVR 静音。

录制后请不要忘记将其重新打开; ) 

### <a name="setting-up-live-streaming-on-youtube"></a>设置 YouTube 上的实时流式处理

你可以真正快速地获取实时流 (实时流式处理) 或设置将来的实时流事件 (新的实时事件) 。 我建议您将它设置为 "新的实时事件"。

1. 打开浏览器并登录 [https://www.youtube.com/](https://www.youtube.com/)
2. 选择你的帐户图标右上方，从下拉
3. 页面左侧的实时流式处理。

"立即流式处理" 方法更改缩略图如果你需要更改基本信息编码器安装程序将服务器 URL 保留为默认值 _ * * 流名称/密钥，请单击 "显示" 并复制此密钥打开 OBS 设置流将此项粘贴到流密钥应用中，然后单击 "确定"。
若要查看实际的 YouTube 实时流视频页面，需要向下滚动并查看共享链接的右下方。
将此项复制并粘贴到新的浏览器选项卡中，然后单击 "视频"，在列表中看到你的视频，它会立即显示，然后单击该页面，你将看到你的 YouTube LIVE stream 页面。
此 URL 是你的实时流链接，可共享到你的所有社交频道： ) 若要停止实时流，请单击 "OBS 上的停止流式处理"，这将结束 YouTube 上的实时流。

"Events" 方法- https://www.youtube.com/my_live_events 单击 "新建实时事件" "添加标题"、"日期"、"开始时间"、"说明" 和 "标记" –不要忘记标记 AltspaceVR ) ：从下拉菜单中选择 "公共"：自定义单击 "创建事件" 如果要添加自定义缩略图，请单击 "浏览" 并上传图像。  (1280x720 最佳) 选择：单一使用流密钥选择编码器：其他编码器复制流名称 (流密钥) 

现在，右键单击 "监视时查看页" 和 "在新选项卡中打开链接"

这是你的 YouTube 实时流事件链接，可在你的实际活动之前以社交方式共享！

现在打开 OBS 文件>设置流将刚才复制的流密钥粘贴到 "流密钥" 字段中，然后单击 "确定"，然后单击 "保存更改" 右键单击 "Live Control 会议室" 和 "在新选项卡中打开链接"。此时将显示 "预览" 按钮。单击 "预览" 按钮对话框，询问你是否要预览实时事件，请稍等片刻，然后你会看到 "开始流式处理" 按钮，单击 "开始流式处理" 对话框将打开，询问你是否要流式传输实时事件，请单击 "确定"

你现在已经开始了！

在 "浏览器" 选项卡上，打开 "查看监视页" 链接，确保视频看起来良好。 请记住，你不会听到音频，因为你已在 Windows 音量合成器中将音频从浏览器中关闭。 请在手机上检查音频，或邀请朋友检查音频。

看起来不错！

Alt-Tab 返回到 AltspaceVR，以便将相机 (，即你的头像) 你的活动。

完成实时流后，请返回到 YouTube 的 "Live Control 会议室" 页面

单击 "停止流式处理"

对话框随即打开，询问你是否要停止流式传输实时事件，确定

请切换到 OBS，并单击 "停止流"。

恭喜是 AltspaceVR 的流


Recording_AltspaceVR_.png


对于奖分，请在社交媒体上与世界分享你的视频，并确保标记为 @AltspaceVR ： ) 