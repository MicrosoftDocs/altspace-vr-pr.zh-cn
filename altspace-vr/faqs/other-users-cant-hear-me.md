---
title: 其他用户听不见我说话
description: 了解如何识别和修复与其他用户在 AltspaceVR 中无法听到我说话相关的问题。
ms.date: 03/11/2021
ms.topic: article
keywords: 常见问题
ms.openlocfilehash: 189d96790207085a2a2c47e964c0db8a08ed95a76d91d2ced3026ba3455b45e3
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/11/2021
ms.locfileid: "119128086"
---
# <a name="other-users-cant-hear-me"></a>其他用户听不见我说话

首先，确定 AltspaceVR 是否正在检测来自麦克风的音频。 可以通过查看在讲话时，视图左下角的麦克风图标是否闪烁来确定这一点。 如果在说话时图标闪烁，则麦克风将正常工作。 如果图标为红色，则你已静音。 选择图标以将自己静音或取消静音。

如果在取消静音后看不到麦克风图标闪烁，可能需要在 AltspaceVR 中调整麦克风设置，请转到"菜单"/"设置"/"音频"/"音频输入选择"。 然后使用箭头按钮选择要使用的麦克风。
 
## <a name="oculus-quest"></a>Oculus Quest 

确保在安装 AltspaceVR 时授予使用麦克风音频的权限。 可以执行的另一项检查是：菜单/设置/音频/音频输入选择，确保它设置为 Android 音频输入 (这是 Quest/Quest2 的默认麦克风) 。
 
## <a name="windows-mixed-reality-oculus-rift-htc-vive-or-2d-mode"></a>Windows Mixed Reality、Oculus Rift、WINDOWS MIXED REALITY Vive 或 2D 模式

请确保 AltspaceVR：菜单/音频输入选择设置麦克风设置正确。 然后使用箭头按钮选择要使用的麦克风。

在启动 AltspaceVR 之前，请确保将正确的麦克风设置为默认录制设备，Windows。 如果 AltspaceVR 中插入了另一个麦克风，则 Oculus Rift 和它都有内置麦克风，则可能会尝试使用该设备。
 
若要更改默认录制设备，Windows：
* 右键单击扬声器图标 **，Windows"播放设备"**
* 导航到" **录制"** 选项卡
* 找到要使用的麦克风。 将标记为"麦克风 " **-"USB** 音频设备" ，"Oculus Rift 麦克风" 将标记为"麦克风 **- Rift 音频"**。
* 右键单击该麦克风，然后选择" **设置为默认设备"**
* 重启 AltspaceVR 后，现在将拾取麦克风
 
如果执行这些步骤后仍遇到问题，则还有其他一些问题，这些问题可能会影响你：
* 如果Alt-Tab超过 30 秒，AltspaceVR 会自动静音，可以使用键盘快捷方式来禁用此功能：空格键可切换关闭/打开静音。
* AltspaceVR 音频系统的音量阈值可能低于该阈值。 将麦克风级别设置为最大值，将麦克风设置得更近，然后以正常音量说话。
* 退出 VR，尝试将 USB 线从头戴显示设备插入备用 USB 3.0 端口。 在我们的体验中，某些 USB 3.0 端口会导致问题。

AltspaceVR 可能无法识别在游戏期间进行的声音设置更改，因此可能需要重启上述麦克风更改的 AltspaceVR 才能生效。  重新输入游戏时，查看麦克风图标，看其是否闪烁。 如果图标闪烁，则麦克风将正常工作。