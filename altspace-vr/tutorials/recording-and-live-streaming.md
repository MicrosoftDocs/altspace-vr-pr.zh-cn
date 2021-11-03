---
title: 录制和实时流式传输
description: 了解如何从电脑录制 AltspaceVR 活动并实时流式传输，以便推广和与用户共享。
author: qianw211
ms.author: v-qianwen
ms.date: 11/1/2021
ms.topic: article
keywords: 流式处理， 录制， 视频， 音频， youtube， obs， 实时
ms.openlocfilehash: e82960097103df25c50f0b03b76d21e10b1cbbd6
ms.sourcegitcommit: 20605c50a93852f93a3464c5c339f6a7da67a047
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "131278973"
---
# <a name="recording-and-live-streaming"></a>录制和实时流式传输

录制和实时流式传输 AltspaceVR 体验以向全球其他人展示是推广活动、AltspaceVR 和 VR 的一种很好的方法！ 请看下面的内容，了解如何开始操作。

本文将指导如何进行以下操作：

* [在电脑上录制 2D 模式下的 AltspaceVR](#recording-altspacevr-in-2d-mode-on-pc)
* [在电脑上以 2D 模式实时流式传输到 AltspaceVR 中的 YouTube](#live-streaming-to-youtube-in-altspacevr-2d-mode-on-pc)

## <a name="recording-altspacevr-in-2d-mode-on-pc"></a>在电脑上以 2D 模式录制 AltspaceVR

### <a name="the-short-version"></a>短版本

1. 已安装 AltspaceVR 和 OBS (Open 用户) 软件。 在 2D 模式下启动 AltspaceVR，启动 OBS，将 OBS 设置为录制 AltspaceVR 并记录离开！

### <a name="the-slightly-longer-version"></a>稍微长一点的版本

1. 访问 [https://obsproject.com/](https://obsproject.com/)
2. 选择 **Windows** 以下载 OBS。 本文使用 **OBS v26.1.1**
3. 安装 OBS

### <a name="have-altspacevr-running-before-you-run-obs"></a>在运行 OBS 之前，运行 AltspaceVR

1. 从网站下载并安装 AltspaceVR：altvr.com/get [](https://altvr.com/getaltspacevr)
2. 若要稳定 VR 视频并消除头部抖动，请确保使用 2D 客户端，或者从电脑拔下头戴显示设备的 USB 电缆，在 2D 模式下启动 AltspaceVR。 如果有 Rift，请按 Ctrl+Alt+Del，选择"服务"，**选择"Oculus VR 运行时** 服务"，右键单击并选择"停止 **"。** 这将禁用 Oculus，并启动 2D 模式下的 AltspaceVR。 重复这些步骤，并使用"启动"重新获取 VR 模式。
3. 还可以在 VR 模式下使用游戏捕获和 OBS 来记录体验

现在，Alt-Tab OBS：

1. 在 **"场景**"下 **+** ，选择并命名新场景
2. 接下来，在" **源"** 下，选择 **"+ > Game Capture">"新建"**
2. 将文本编辑为"AltspaceVR Capture"，勾选 **"使源可见**"，然后选择"确定 **"**
3. 双击"源 **"下的 AltspaceVR** **捕获**
4. 更改 **模式** 以 **捕获特定窗口**
5. 窗口：[AltspaceVR.exe]：AltspaceVR
6. 窗口匹配优先级：匹配标题，否则查找同一可执行文件的窗口
7. 向下滚动到" **捕获光标**：untick"
8. 选择“确定”
9. 这应该会使 AltspaceVR 显示在 OBS 中。

现在，若要在 OBS 中设置以下属性，请转到"**文件> 设置：**

|选项卡|设置|
|---|---|
| **常规** | 保留默认值 |
| **流** | 保留默认值 |
| **输出** | 切换到"高级" |
| **-"流式处理"选项卡** | 音频轨道 1 <br> 编码器：x264 <br> 重新缩放输出：未标点 <br> 速率控制：CBR <br> 比特率：6000 (6000 表示 30 fps，9000 表示 60 fps)  <br> 关键帧间隔 = 2 <br> CPU 使用率预设 = 非常快 |
| **-"录制"选项卡** | 类型：标准 <br> 录制路径：D：/video (浏览到要保存视频文件的位置)  <br> 录制格式：mp4 (如果在录制时发生崩溃，请尝试在此处使用 flv 而不是 mp4，如果崩溃，视频仍可与 flv)  <br> 音频轨道 1 <br> 编码器：使用流编码器 |
| **-Audio 选项卡** | 音频比特率：160 (所有轨迹)  |
| **-Replay 缓冲区选项卡** | 保留默认值 |
| **音频：** | 采样率：44.1khz <br> 频道：立体声 <br> 桌面音频：默认值 <br> 桌面音频 2：禁用 <br> 麦克风/Aux 音频：默认值 |
| **视频** | 基本 (画布) 分辨率：1920x1080 <br> 输出 (缩放) 分辨率：1920x1080 <br> 纵向缩减筛选器：双 (化缩放，16 个样本)  <br> 常见 FPS 值：30 (或 60)  |
| **热键** | 保留默认值 |
| **高级** | 进程优先级：正常 | <br>

<br>现在，请确保选择"应用 **"，** 然后选择" **确定** "以保存所有 OBS 设置。 

1. Alt-Tab AltspaceVR，进入正确的空间/世界/事件，并排好相机 (即你的头像) 我们即将录制视频！
2. Alt-Tab OBS，准备就绪后，单击"开始 **录制"。**

你将在 OBS 的右下角看到 **REC：** 将开始计数，点为红色，这意味着要录制！

对此进行测试录制： 
1. 在 AltspaceVR 中打开/关闭/滚动菜单以发出 UI 声音
2. 确保未静音（例如"Sibilance，Sibilance"）或让其他用户以正常音量与用户交谈。
3. 在这样做 **时，** 查看桌面音频和 **麦克风/Aux** 级别，看它是否正确选取了音频。

录制时，我们通常会将麦克风/Aux 静音。 继续选择麦克风/Aux 的扬声器图标，它将以 X 为红色。

* 很难将麦克风音频级别与其他用户的音频匹配，因此在录制事件时麦克风最好静音。
* 音频的另一个问题就是 OBS 的设置方式。 它会从计算机捕获所有音频，因此，如果你正在观看 YouTube 或在电脑上收到通知声音，它将录制该音频。
* 若要仅录制来自 AltspaceVR 的音频，请转到打开音量调音 **器 (右** 键单击 Windows) 右下角的扬声器图标，将系统声音、浏览器等静音，但不要将 OBS 或 AltspaceVR 静音。

> [重要]请不要忘记在录制后取消排列这些音量调音器设置。

现在，导航回 OBS 并选择"**停止录制"。** 若要查找刚录制的视频，请转到"文件 **">"显示录制内容"。** 这会打开包含 OBS 视频文件的文件夹，然后双击测试视频。

有时，录制非常响，因此降低 OBS 中桌面音频的滑块，然后进行另一个录制以进行测试。

Pro提示：使用 Ctrl+Alt+P 切换"飞行模式"，它会从视图中删除 UI，以获得很好的干净快照。

恭喜你是 AltspaceVR 视频录制器！

## <a name="live-streaming-to-youtube-in-altspacevr-2d-mode-on-pc"></a>在电脑上以 AltspaceVR 2D 模式实时流式传输到 YouTube

### <a name="the-short-version"></a>短版本

已安装 AltspaceVR 和 OBS。 启动 AltspaceVR 和 OBS。 你可以实时流 "立即" 或在 "以后一天"。 在 YouTube 上，设置 OBS 与 YouTube 流密钥。 开始在 OBS 和 YouTube 上进行流式处理，并且你对比赛非常熟悉！

### <a name="the-slightly-longer-version"></a>略长版本

请参阅本页顶部的 "在 [计算机上2d 模式下记录 AltspaceVR](#recording-altspacevr-in-2d-mode-on-pc) " 部分，以获取有关如何使用本地录制而不是实时流测试录制的说明，以及如何设置照相机截图。

## <a name="setting-up-live-streaming-on-youtube"></a>设置 YouTube 上的实时流式处理

你可以获取实时流 "立即运行"，或者使用 "以后的日期" 设置将来的实时流。

1. 打开浏览器并 [https://www.youtube.com/](https://www.youtube.com/) 登录到 [https://studio.youtube.com/](https://studio.youtube.com/)
2. 查看右上方，选择 " **创建** "， **然后上线**

**"马上"** 方法：

1. 选择 "**立即/开始**"
1. 选择 **流式处理软件/中转**
1. 选择 " **编辑**"、"右上方" 以编辑视频详细信息和自定义
1. 在 " **Stream 设置** 下，保留默认值
1. **在 "流密钥" (粘贴到编码器)** 中，**复制** 密钥，以便可以将其粘贴到 OBS 中。
1. 打开 OBS/**设置**  /  **流**
1. 在 " **服务** " 下拉菜单中，选择 " **YouTube-RTMPS**
1. 将 Stream 密钥从 YouTube 粘贴到 OBS 中的 **流密钥** 字段。
1. 单击 " **应用**"，然后单击 **"确定"**
1. 选择 OBS 中的 **开始流式处理**
1. 切换到 YouTube，你会看到你现在已在 YouTube 上生活！
1. 若要查看实际的 YouTube 实时流视频页面，需要选择右上角的共享图标
1. 单击 "视频链接"，你会看到并听到你的 YouTube 实时流 
1. 此 URL 是你的实时流链接，可共享到你的所有社交渠道： ) 
1. 若要停止实时流，请在 YouTube 上选择 "结束流"，然后在 OBS 上停止流式处理

"**后续日期**" 方法：
1. 在左上方，选择 " **管理** " 图标
1. 选择 **计划流**，右上
1. 添加标题、说明、类别、缩略图 (1280x720) ， **然后再**
1. Live chat 选项， **接下来**
1. 专用、未列出或公用 (选择公共) 
1. 计划要生效的日期和时间，然后 **完成**

 **准备好以后开始实时流时：**
1. 在 "Stream 设置下，保留默认值
1. **在 "流密钥" (粘贴到编码器)** 中，**复制** 密钥，以便可以将其粘贴到 OBS 中。
1. 打开 OBS/**设置**  /  **流**
* 在 " **服务** " 下拉菜单中，选择 " **YouTube-RTMPS**
1. 将 Stream 密钥从 YouTube 粘贴到 OBS 中的 **流密钥** 字段。
1. 单击 " **应用**"，然后单击 **"确定"**
1. 选择 OBS 中的 **开始流式处理**
1. 切换到 YouTube，你会看到你现在已在 YouTube 上生活！
1. 若要查看实际的 YouTube 实时流视频页面，需要选择右上角的共享图标
1. 单击 "视频链接"，你会看到并听到你的 YouTube 实时流 
1. 此 URL 是你的实时流链接，可共享到你的所有社交渠道： ) 
1. 若要停止实时流，请在 YouTube 上选择 "**结束流**"，然后在 OBS 上 **停止流式处理**

对于奖分，请在社交上共享视频并确保标记为 @AltspaceVR ： ) 