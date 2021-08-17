---
title: 其他用户听不见我说话
description: 了解如何识别和修复与其他用户无法在 AltspaceVR 中听到我相关的问题。
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

首先，确定 AltspaceVR 是否正在检测麦克风的音频。 您可以通过查看您的视图左下方的麦克风图标来确定这一点。 如果说话时图标闪烁，则麦克风工作正常。 如果该图标为红色，则表示你处于静音。 选择要静音或取消静音的图标。

如果在将后看不到麦克风图标闪烁，则可能需要在 AltspaceVR 中调整麦克风设置，然后选择 "打开" 菜单/"设置/音频/音频输入"。 然后，使用箭头按钮选择要使用的 Mic。
 
## <a name="oculus-quest"></a>Oculus Quest 

在安装 AltspaceVR 时，请确保授予使用 Mic 音频的权限。 可以执行的另一项检查是查找： "菜单"/"设置"/"音频/音频/音频输入"，并将其设置为 "Android 音频输入" (，这是 "Quest2's"/"默认 mic) "。
 
## <a name="windows-mixed-reality-oculus-rift-htc-vive-or-2d-mode"></a>Windows Mixed Reality、Oculus Rift、HTC naopak 或2d 模式

请确保在 AltspaceVR： Menu/设置/音频/音频输入选择中具有正确的麦克风设置。 然后，使用箭头按钮选择要使用的 Mic。

在启动 AltspaceVR 之前，请确保将正确的麦克风设置为 Windows 中的默认录制设备。 Oculus Rift 和 HTC Naopak 都有内置麦克风，如果已插入其他麦克风，AltspaceVR 可能尝试使用该设备。
 
若要更改 Windows 中的默认录制设备：
* 右键单击 "Windows 中的扬声器图标，然后选择"**播放设备**"
* 导航到 " **录制** " 选项卡
* 找到想要使用的麦克风。 HTC Naopak 麦克风将标记为 " **麦克风-USB 音频设备** "，Oculus Rift 麦克风将标记为 " **麦克风-Rift 音频**"。
* 右键单击该麦克风，然后选择 "**设置为默认设备**"
* 重新启动 AltspaceVR 后，将立即选取麦克风
 
如果在执行这些步骤后仍遇到问题，则可能会影响你：
* 如果你 Alt-Tab 超过30秒，AltspaceVR 将 automute 你，你可以通过使用键盘快捷方式将其禁用：空格键以开启/关闭静音。
* AltspaceVR 音频系统的音量阈值可能低于此阈值。 将麦克风级别设置为 "最大"，将 "麦克风" 设置为离你的嘴近，并在正常音量上说话。
* 退出 VR，尝试将你的 USB 电缆从耳机插入到备用 USB 3.0 端口。 在我们的经验中，某些 USB 3.0 端口会导致问题。

AltspaceVR 可能无法识别在游戏过程中所做的声音设置更改，因此你可能需要重启上述麦克风更改才能生效。  重新输入游戏时，请查看麦克风图标，看看它是否闪烁。 如果图标闪烁，则麦克风工作正常。