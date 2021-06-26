---
title: 录制和实时流式处理
description: 了解如何从电脑录制 AltspaceVR 活动并实时流式传输，以便推广和与用户共享。
ms.date: 04/26/2021
ms.topic: article
keywords: 流式处理， 录制， 视频， 音频， youtube， obs
ms.openlocfilehash: 0bf32d8ac7e2d409eb5e2c31a9da8a878e0e5eef
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/25/2021
ms.locfileid: "112923014"
---
# <a name="recording-and-live-streaming"></a>录制和实时流式处理

录制和实时流式传输 AltspaceVR 体验以向全球其他人展示是推广活动、AltspaceVR 和 VR 的一种很好的方法！ 查看以下内容，了解如何开始操作：

本文将指导如何进行以下操作：

* [在电脑上录制 2D 模式下的 AltspaceVR](#recording-altspacevr-in-2d-mode-on-pc)
* [在电脑上以 2D 模式实时流式传输至 AltspaceVR 中的 YouTube](#live-streaming-to-youtube-in-altspacevr-2d-mode-on-pc)

## <a name="recording-altspacevr-in-2d-mode-on-pc"></a>在电脑上以 2D 模式录制 AltspaceVR

### <a name="the-short-version"></a>短版本

1. 已安装 AltspaceVR 和 OBS。 在 2D 模式下启动 AltspaceVR，启动 OBS，将 OBS 设置为录制 AltspaceVR 并记录离开！

### <a name="the-slightly-longer-version"></a>稍微长一点的版本

1. 访问 [https://obsproject.com/](https://obsproject.com/)
2. 选择 **"Windows"** 以下载 OBS。 本文使用 **OBS v22.0.2**
3. 安装 OBS

### <a name="have-altspacevr-running-in-2d-mode-before-you-run-obs"></a>在运行 OBS 之前，在 2D 模式下运行 AltspaceVR

1. 从网站下载并安装 AltspaceVR：altvr.com/get [](https://altvr.com/getaltspacevr)
2. 请确保在 2D 模式下启动 AltspaceVR，方法是从电脑拔下 HMD 的 USB 电缆，或者如果你有一个 Rift：Ctrl+Alt+Del、服务、Oculus VR 运行时服务，请右键单击，停止。 
    * 这将禁用 Oculus，在 2D 模式下启动 AltspaceVR，重复这些步骤并使用"启动"重新获取 VR 模式。

现在，Alt-Tab OBS：

1. 在"源"下，选择 **"+ > Game Capture">"新建"**
2. 将文本编辑为"AltspaceVR Capture"，勾选 **"使源可见**"，然后选择"确定"
3. 双击"源 **"下的 AltspaceVR** 捕获
4. 更改 **模式** 以 **捕获特定窗口**
5. 窗口：[AltspaceVR.exe]：AltspaceVR
6. 窗口匹配优先级：匹配标题，否则查找同一可执行文件的窗口
7. 向下滚动到"捕获光标：untick"
8. 选择“确定”

这应该会使 AltspaceVR 显示在 OBS 中。 现在，若要在 OBS 中设置以下属性，请转到"**文件>设置"：**

|选项卡|设置|
|---|---|
| **常规** | 保留默认值 |
| **Stream** | 保留默认值 |
| 输出模式 | 切换到"高级" |
| “流式处理”选项卡 | 音频轨道 1 <br> 编码器：x264 <br> 重新缩放输出：未标点 <br> 速率控制：CBR <br> 比特率：6000 (6000 表示 30 fps，9000 表示 60 fps)  <br> 关键帧间隔 = 2 <br> CPU 使用率预设 = 非常快 |
| "录制"选项卡 | 类型：标准 <br> 录制路径：D：/Video (浏览到要保存到视频文件的位置)  <br> 录制格式：mp4 (如果在录制时发生一些崩溃，请尝试在此处使用 flv 而不是 mp4，如果崩溃，视频仍可以使用 flv)  <br> 音频轨道 1 <br> 编码器：使用流编码器 |
| "音频"选项卡 | 音频比特率：160 (所有轨迹)  |
| "重播缓冲区"选项卡 | 保留默认值 |
| **音频：** | 采样率：48khz <br> 频道：立体声 <br> 桌面音频设备：默认值 <br> 桌面音频设备 2：禁用 <br> 麦克风/Aux 音频设备：默认值 |
| **视频** | 基本 (画布) 分辨率：1920x1080 <br> 输出 (缩放) 分辨率：1920x1080 <br> 纵向缩减筛选器：双 (缩放，16 个样本)  <br> 常见 FPS 值：30 |
| **热键** | 保留默认值 |
| **高级** | 进程优先级：正常 | <br>

<br>现在，请确保选择"应用 **"，** 然后选择" **确定** "以保存所有 OBS 设置。 

1. Alt-Tab AltspaceVR，进入正确的空间/世界/事件，并排好相机 (即，你的头像) 我们即将录制视频！
2. Alt-Tab OBS，准备就绪后，单击"开始 **录制"。**

你将在 OBS 的右下角看到 REC： 将开始计数，点为红色，这意味着要录制！

对此进行测试录制： 
1. 在 AltspaceVR 中打开/关闭/滚动菜单以发出 UI 声音
2. 请确保未静音（例如"Sibilance，Sibilance"）或让其他用户以正常音量与用户交谈。
3. 在这样做时，查看桌面音频和麦克风/Aux 级别，看其是否正常工作。

录制时，我们通常会将麦克风/Aux 静音。 继续选择麦克风/Aux 的扬声器图标，它将以 X 为红色。

* 很难匹配音频和其他用户的音频，因此在录制事件时麦克风最好静音。
* 音频的另一个问题就是 OBS 的设置方式。 它会从计算机捕获所有音频，因此，如果你正在电脑上观看 YouTube，它会录制该音频或一些用户通知。
* 若要仅录制来自 AltspaceVR 的音频，请转到音量调音器 (右键单击 Windows) 右下角的扬声器图标，将系统声音、浏览器等静音，但不要将 OBS 或 AltspaceVR 静音。

> [!IMPORTANT]
> 请不要忘记在录制后重新启用这些音量调音器设置。

现在，导航回 OBS，然后从"文件"选择"停止录制 **>显示录制内容"。** 这会打开包含 OBS 视频文件的文件夹，然后双击测试视频。

有时，录制声音很大，因此请降低桌面音频的滑块，然后进行另一个录制以进行测试。


## <a name="live-streaming-to-youtube-in-altspacevr-2d-mode-on-pc"></a>在电脑上以 AltspaceVR 2D 模式实时流式传输到 YouTube

### <a name="the-short-version"></a>短版本

已安装 AltspaceVR 和 OBS。 在 2D 模式下启动 AltspaceVR，启动 OBS，在 YouTube 上实时流式传输或创建"新建直播活动"，使用 YouTube Stream 密钥设置 OBS，在 OBS 中开始流式传输，在 YouTube 上开始流式传输，然后开始直播比赛！

### <a name="the-slightly-longer-version"></a>稍微长一点的版本

1. 访问 [https://obsproject.com/](https://obsproject.com/)
2. 选择 **Windows** 下载 OBS (此帖子使用的是 OBS v22.0.2) 
3. 安装 OBS

在运行 OBS 之前，在 2D 模式下运行 AltspaceVR
1. 从网站下载 AltspaceVR： [https://account.altvr.com/downloads](https://account.altvr.com/downloads)
2. 若要确保在 2D 模式下启动 AltspaceVR，请从电脑拔下 HMD 的 USB 电缆，或者如果你有一个 Rift：Ctrl+Alt+Del、服务、Oculus VR 运行时服务，请右键单击，停止。 这会禁用 Oculus Home，在 2D 模式下启动 AltspaceVR，重复这些步骤并再次启动以获取 VR 模式。

3. Alt-Tab OBS

4. 在"源"下，选择 **+** ，选择"游戏捕获"，新建，将文本编辑为"AltspaceVR 捕获"，勾选"使源可见"，"确定"
5. 双击 AltspaceVR 捕获
6. 模式：捕获特定窗口
7. 窗口：[AltspaceVR.exe]：AltspaceVR
8. 窗口匹配优先级：匹配标题，否则查找同一可执行文件的窗口
9. 向下滚动到"捕获光标：取消提示""确定"

这应该会使 AltspaceVR 显示在 OBS 中。 很好！

现在，在 OBS 中转到"文件>设置：

| 选项卡 | 设置 |
|---|---|
| 常规 | 在流式传输 ("自动记录"，这会将视频文件记录到计算机，以及实时流式处理)  |
| Stream | 流类型：流式处理服务 <br> 服务：YouTube/YouTube 游戏 (也可以流式传输到 Twitch、Mixer、Facebook Live 等) <br>服务器：主 YouTube ingest 服务器 <br>流键：粘贴 YouTube 中的流密钥 (请参阅下面的"在 YouTube 上设置实时)  |
| 输出 | 输出模式：切换到"高级" |
| 流式处理 | 音频轨道 1 <br>编码器：x264 <br>强制实施流式处理服务编码器设置：时钟周期 <br>重新缩放输出：未标点 <br>速率控制：CBR <br>比特率：6000 (6000 表示 30 fps，9000 表示 60 fps)  <br>关键帧间隔 = 2 <br>CPU 使用率预设 = 非常快 |
| 记录 | 类型：标准 <br>录制路径：D：/video (之前选择"流式传输时自动录制"时，浏览到要保存到的视频文件)  <br>录制格式：mp4 (如果在录制时发生一些崩溃，请尝试在此处使用 flv 而不是 mp4，如果崩溃，视频仍可以使用 flv)  <br>音频轨道 1 <br>编码器：使用流编码器 |
| 音频 | 音频比特率：160 (，适用于所有轨迹) 采样率：48khz <br>频道：立体声 <br>桌面音频设备：默认值 <br>桌面音频设备 2：禁用 <br>麦克风/Aux 音频设备：默认值 |
| 重播缓冲区 | 保留默认值 |
| 视频 | 基本 (画布) 分辨率：1920x1080 <br>输出 (缩放) 分辨率：1920x1080 <br>纵向缩减筛选器：双 (缩放，16 个样本)  <br>常见 FPS 值：30 |
| 热键 | 保留默认值 |
| 高级 | 进程优先级：正常 |
|||

<br>现在，请确保单击"应用"，然后单击"确定"，然后关闭并重新打开 OBS。 这将保存所有 OBS 设置。 看起来不错：) 

请参阅上面的"如何在电脑上录制 2D 模式下的 AltspaceVR"部分，了解如何使用本地录制而不是实时流测试录制，以及如何在录制前先设置相机拍摄设置。

音频的另一个问题就是 OBS 的设置方式。 它会从计算机捕获所有音频，因此，如果你正在观看 YouTube，它将录制该音频、Teams 消息或通知声音。

若要仅录制来自 AltspaceVR 的音频，请转到音量调音器 (右键单击 Windows) 右下角的扬声器图标，将系统声音、浏览器等静音，但不要将 OBS 或 AltspaceVR 静音。

请不要忘记在录制后重新打开音频;) 

恭喜你是 AltspaceVR 视频录制器！

## <a name="setting-up-live-streaming-on-youtube"></a>在 YouTube 上设置实时流式处理

可以在 Stream 中快速获取 (流) 或设置未来的实时流事件 (**管理) 。** 我可能会建议你以"管理"方式设置它。

1. 打开浏览器并登录 [https://www.youtube.com/](https://www.youtube.com/) ，然后转到 [https://www.youtube.com/my_live_events](https://www.youtube.com/my_live_events)
2. 在右上方的"帐户"图标上选择，然后从下拉列表中选择"Creator Studio"
3. 页面左侧的"实时流式处理"。

'**Stream now**' 方法：

* 选择"编辑"以输入实时流信息<br>
* 在"流设置"下，保留默认值<br>
* 流式 (粘贴到编码器) ，选择"显示"并复制此密钥，以便将其粘贴到 OBS 中<br>
* 打开 OBS/设置/流<br>
* 将 YouTube 中的流密钥粘贴到 OBS 中的"流密钥"字段<br>
* 应用，然后确定<br>
* 选择"在 OBS 中启动流式处理"<br>
* 切换到 YouTube，你将看到你现在在 YouTube 上实时观看！<br>
* 若要查看实际的 YouTube 实时流视频页面，需要选择右上角的"共享"图标。<br>
* 将"视频链接"复制并粘贴到新的浏览器选项卡中，你将看到 YouTube 实时流页面。<br>
* 此 URL 是实时流链接，可以共享到所有社交频道：) <br>
* 若要停止实时流，请选择"停止 OBS 上的流式处理"，这将结束 YouTube 上的实时流。<br>
* 然后停止 YouTube 上的流<br>

"**管理**"方法：
* 选择"计划流"
* 如果已设置以前的托管实时流，请新建或重复使用设置
* 添加标题、日期、开始时间、说明、上传缩略图和标记 – 不要忘记标记 AltspaceVR ：) 
* 从下拉菜单中选择"公共 (默认值为"未列出") 
* 使用默认值
* 复制流密钥 (粘贴到编码器) 
* 若要查看实际的 YouTube 实时流视频页面，需要选择右上角的"共享"图标。 这是 YouTube 实时流事件链接，可以在实际活动之前通过社交方式共享！
* 现在打开 OBS
* 文件/设置
* Stream
* 将复制的流密钥粘贴到"流密钥"字段中
* 应用，然后确定
* 选择"开始流式处理"
* 返回到 YouTube，你将看到"预览"窗口显示你的流，并且"上一个实时"现在在右上方亮起。
* 选择"上一个活动"
* 你现在是实时的！
* 转到浏览器选项卡，并打开"在观看页上查看"链接，确保视频看起来不错。 请记住，你不会听到音频，因为你在 Windows 音量调音器中将其静音时，你已从浏览器关闭音频。 检查手机上的音频，或要求朋友检查音频。
* 看起来不错！
* Alt-Tab AltspaceVR 移动相机 (，即头像) 在活动中四处移动。
* 完成实时流后，返回到 YouTube"实时控制房间"页
* 选择"停止流式处理"
* 对话框随即打开，询问是否要停止流式传输直播活动，确定
* 转到"OBS"，然后选择"停止流式处理"。
* 恭喜，你现在是 AltspaceVR 流式处理器！

对于奖励点，在社交媒体上与世界共享视频，并确保标记我们 @AltspaceVR ：) 