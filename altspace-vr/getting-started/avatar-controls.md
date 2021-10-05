---
title: 在 2D 电脑模式下使用鼠标/键盘的头像控件
description: 了解如何在新的和经典控制方案之间切换，以在 2D PC 模式下使用鼠标和键盘移动头像。
ms.date: 10/4/2021
author: qianw211
ms.author: v-qianwen
ms.topic: article
keywords: 头像， 鼠标， 键盘， 2d， 电脑模式， 控件
ms.openlocfilehash: bacaf5e267ab28cc410b5659a34273b12ad36be5
ms.sourcegitcommit: 44cb9f91859001dbda7d15e0f25f94284708a715
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2021
ms.locfileid: "129446291"
---
# <a name="avatar-controls-with-mousekeyboard-in-2d-pc-mode"></a>在 2D 电脑模式下使用鼠标/键盘的头像控件

使用鼠标和键盘的 2D 电脑模式有两种不同的控制方案：
* 新电脑控件，这是新帐户的默认设置
* 经典电脑控件

可以切换到"菜单"或"经典控件"，> 设置 >"输入 **">"经典电脑** 控件"，然后打开或关闭该选项。

## <a name="new-pc-controls"></a>新电脑控件

使用"新建电脑"控件时，有两种不同的模式："光标模式"和"查找模式"。 右键单击笔记本电脑或鼠标，以使用 **光标/外观切换** 在两种模式之间切换。

* **光标模式** 允许与菜单交互。 当你在视图左下角看到 AltspaceVR 徽标/菜单按钮时，你会知道你处于光标模式：

    ![包含菜单的光标模式](images/avatar-controls-img-01.png)

* **使用"** 查找模式"可以四处查看，如果使用的是笔记本电脑触控板，则它非常不错。 可以使用"查找模式"和键盘同时查看/移动。 如果视图左下角如以下屏幕截图所示，你将了解你位于"查找模式"中：

    ![查找模式](images/avatar-controls-img-02.png)

### <a name="new-pc-controls-for-keyboard--mouse"></a>键盘/鼠标的新电脑控件

![具有输入映射的键盘和鼠标](images/keyboard-mouse-controls.svg)

## <a name="classic-pc-controls"></a>经典电脑控件 

### <a name="mouse-controls"></a>鼠标控件

**移动**

| 输入 | 操作 |
|---|---|
| 左键单击 | 远程端口到目标位置 |
| 按住左键单击 | 预览目标位置 |
| 中间单击 | 向前移动 |
| 右键单击"+ 移动鼠标" | 旋转/平移照相机四处查看 |
| 右键单击"+ 中间滚轮"，向前/向后滚动 | 放大/缩小相机 |

**菜单选项**

| 输入 | 操作 |
|---|---|
| 左键 (按钮)  | 选择按钮 |
| 按住左键单击 + 右键单击 | 隐藏 AltspaceVR 菜单 |

### <a name="keyboard-controls"></a>键盘控件

**移动**

| 操作 | 键 | 备用键 |
|---|---|---|
| 向前移动 | W | 向上键 |
| 向后移动 | S | 向下键 |
| 左侧的 Strafe | A | 空值 |
| Strafe right | D | 空值 |
| 向前运行 | Shift + W | Shift + 向上键 |
| 向后运行 | Shift + S | Shift + 向下键 |
| 向左运行 | Shift + A | 空值 |
| 右运行 | Shift + D | 空值 |
| 向左旋转"舒适模式" | Q | 向左键 |
| "舒适模式"向右旋转 | E | 向右键 |

**菜单选项**

| 操作 | 键 | 备用键 |
|---|---|---|
| 切换菜单 | Esc | 空值 |
| 全屏切换应用 | Alt + Enter | 空值 |
| 切换麦克风 | 空格键 | Ctrl + Alt + T |