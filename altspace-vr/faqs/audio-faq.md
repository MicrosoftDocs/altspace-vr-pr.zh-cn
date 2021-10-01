---
title: 有关 AltspaceVR 音频的常见问题
description: 与音频相关的问题的故障排除和支持。
ms.date: 8/23/2021
author: qianw211
ms.author: v-qianwen
ms.topic: article
keywords: vr，音频，故障排除，支持
ms.openlocfilehash: 05c8a477b9e50b5067e62b934fe2ff8bd656f06c
ms.sourcegitcommit: 5c452a9092297c0bfbc8efabebf395e7ee31853f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2021
ms.locfileid: "129311841"
---
# <a name="frequently-asked-questions-about-audio"></a>有关音频的常见问题

## <a name="does-my-vr-headset-have-a-built-in-mic"></a>我的 VR 耳机是否有内置麦克风？

### <a name="oculus-riftrift-s-oculus-questquest-2-windows-mixed-reality-and-htc-vive"></a>Oculus Rift/Rift S、Oculus/2、Windows Mixed Reality 和 HTC naopak

是的，这些 VR 耳机有内置麦克风。

### <a name="windows"></a>Windows

对于与 Windows 一起使用的耳机，你应该能够在插入耳机时找到 **录制设备** 下列出的麦克风。

### <a name="further-troubleshooting"></a>进一步的故障排除

* [AltspaceVR 支持-其他用户无法听到我](#what-do-i-do-if-other-users-cant-hear-me)
* [AltspaceVR 支持-管理 Oculus 寻找权限](../getting-started/oculus-controls.md#managing-permissions)

## <a name="is-there-a-push-to-talk-button"></a>有一键通按钮吗？

没有 "按下对话" 按钮。  如果你查看视图的左下方，则可以使用麦克风图标来切换语音。 或者，您可以使用键盘快捷方式、空格键将麦克风静音/取消静音。

如果说话时图标闪烁，则麦克风工作正常！
 
## <a name="what-do-i-do-if-my-audio-is-choppy"></a>如果音频不连贯，我该怎么办？

某些用户注意到，当另一个虚拟形象说话时，音频会以断断续续或普通的下拉方式出现。 其他情况下，其他用户可能会收到自己的音频通过不连贯或机器人发出的通知。

首先要尝试重新进入你所在的空间，甚至重新启动 AltspaceVR （如果此操作失败）。 音频问题并不常见，但发生这种情况通常是一种简单的解决方法。 

如果此操作失败，则可以查看以下内容：

#### <a name="cpu-performance-for-desktop-users"></a>桌面用户的 CPU 性能

查看我们建议用于运行 AltspaceVR 的硬件 [系统规范](../getting-started/system-requirements.md) 。 我们发现，i3 或更低 Cpu 不仅会导致与视频帧速率有关的问题，而且可能会导致出现类似于下拉和质量较差的音频问题。

#### <a name="internet-bandwidth-and-network-connection"></a>Internet 带宽和网络连接

低速 internet 连接 (低于 5mbps) 或 WiFi 的用户可能会遇到音频问题，例如下拉。 建议将以太网电缆的 hardline 连接到计算机，并使用比5mbps 更快的连接。 你可能想要退出可能在后台使用 internet 连接的任何程序。

## <a name="what-do-i-do-if-other-users-cant-hear-me"></a>如果其他用户听不到我该怎么办？

首先，确定 AltspaceVR 是否正在检测麦克风的音频。 您可以通过查看您的视图左下方的麦克风图标来确定这一点。 如果说话时图标闪烁，则麦克风工作正常。 如果该图标为红色，则表示你处于静音。 选择要静音或取消静音的图标。

如果在将后看不到麦克风图标闪烁，则可能需要在 AltspaceVR 中调整麦克风设置，然后选择 "打开" 菜单/"设置/音频/音频输入"。 然后，使用箭头按钮选择要使用的 Mic。
 
### <a name="oculus-questquest-2"></a>Oculus

在安装 AltspaceVR 时，请确保授予使用 Mic 音频的权限。 你可以执行的另一项检查是查找： "菜单"/"设置"/"音频/音频/音频输入"，并将其设置为 "Android 音频输入"，这是 "Quest2's" 默认 mic。
 
### <a name="windows-mixed-reality-oculus-riftrift-s-htc-vive-or-2d-mode"></a>Windows Mixed Reality、Oculus Rift/Rift S、HTC naopak 或2d 模式

请确保在 AltspaceVR： Menu/设置/音频/音频输入选择中具有正确的麦克风设置。 然后，使用箭头按钮选择要使用的 Mic。

在启动 AltspaceVR 之前，请确保将正确的麦克风设置为 Windows 中的默认录制设备。 Oculus Rift/Rift S 和 HTC Naopak 都有内置麦克风，如果有另一个连接到 AltspaceVR 的麦克风，可以尝试使用该设备。
 
若要更改 Windows 中的默认录制设备：

* 右键单击 Windows 的扬声器图标，然后选择 "**打开声音设置**"。
* 导航到 **输入/选择输入设备** 下拉菜单。
* 从下拉菜单中选择要使用的麦克风： 
    * HTC Naopak 麦克风将标记为 " **麦克风-USB 音频设备**"。
    * 将 Oculus Rift 麦克风标记为 **耳机式麦克风 (Oculus Virtual Audio Device)**。
* 重新启动 AltspaceVR 后，将立即选取麦克风
 
如果在执行这些步骤后仍存在问题，可能会影响你的操作：

* 如果你 Alt-Tab 超过30秒，则 AltspaceVR 会自动为你静音。 **当 AltspaceVR 处于空闲状态时，可以在菜单 > 设置 > 音频 > 静音** 中禁用此项。
* AltspaceVR 音频系统的音量阈值可能低于此阈值。 将麦克风级别设置为 "最大"，将 "麦克风" 设置为离你的嘴近，并在正常音量上说话。
* 退出 VR，尝试将你的 USB 电缆从耳机插入到备用 USB 3.0 端口。 在我们的经验中，某些 USB 3.0 端口会导致问题。

AltspaceVR 可能无法识别在游戏过程中所做的声音设置更改，因此，你可能需要重新启动 AltspaceVR 以使上述麦克风更改生效。  重新进入游戏时，请查看麦克风图标，看看它是否闪烁。 如果图标闪烁，则麦克风工作正常。

## <a name="support"></a>支持

AltspaceVR 团队的问题或反馈？ 

> [!div class="nextstepaction"]
> [单击此处发送支持请求](https://help.altvr.com/hc/requests/new)