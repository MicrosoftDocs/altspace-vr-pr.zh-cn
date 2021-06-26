---
title: 使用多媒体控制台
description: 了解如何开始在 AltspaceVR 体验中配置、发布和控制多媒体控制台。
ms.date: 03/11/2021
ms.topic: article
keywords: 控制台，多媒体
ms.openlocfilehash: 4a51ff76e44d3870972bc17288ae77c1fa888922
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/25/2021
ms.locfileid: "112923004"
---
# <a name="using-the-multimedia-console"></a>使用多媒体控制台

多媒体控制台是一种支持事件和世界媒体共享的工具。 可以使用它来共享图像、演示文稿幻灯片、实时流、视频、播放列表等内容。 下面是有关如何使用多媒体控制台 **v0.5.0+ 的分步说明**。 

## <a name="getting-started"></a>入门

多媒体控制台入门由两部分完成。  首先，使用 Web 门户为环境中放置的多媒体控制台会话生成和发布配置。  其次，将实际多媒体控制台应用放置于环境中，并设置它应该使用的配置代码。

### <a name="configuring-the-multimedia-console-with-the-web-portal"></a>使用 Web 门户配置多媒体控制台

1. 首先，需要确保内容联机托管，因为需要 URL。  (可以将照片上传到 altvr.com、在线托管视频.mp4或使用 Dlive 实时流链接： https://dlive.tv/yourlivestream) 
2. 导航到多媒体控制台的 Web 门户，网址为 [https://multimedia-console.altvr.com/](https://multimedia-console.altvr.com/)
3. 在 Web 门户中，可以生成并发布多媒体控制台的配置。   (请参阅下文，了解有关各种属性) 。
4. 将媒体输入媒体列表并配置常规设置后，选择应用右上方的"发布"按钮。
5. 发布完成后，将弹出一个对话框，其中包含两个单词代码，供你进入放置的多媒体控制台。
  
### <a name="placing-the-multimedia-console-in-your-environment"></a>将多媒体控制台置于环境中

1. 在"世界 **编辑器">"编辑器面板> SDK 应用>"多媒体控制台"。**  (SDK 应用中转到"世界编辑器">">" **基本信息**"-这是针对未注册的应用)   
2. 定位多媒体控制台，以最佳方式设置空间和受众。
3. 单击橙色的"编辑模式"按钮，退出编辑模式。
4. 系统会提示你是 **媒体播放器所有者吗？** 如果你是此多媒体控制台会话的官方所有者，请确认并继续。  (其他权限角色也可用。 有关详细列表，请参阅) 
5. 选择"是"以确认你是主主机。  
6. 应弹出一个对话框，要求你输入 Web 门户中的代码或有效的 JSON。  输入 Web 门户中的两个单词代码（包括短划线）并点击"确定"。  (JSON 是下面所述的高级) 
7. 多媒体控制台应在几秒钟后使用你在 Web 门户中构建的配置进行加载。

### <a name="controlling-the-multimedia-console"></a>控制多媒体控制台

1. 输入代码并完成配置过程后，你将看到控件按钮显示在媒体显示下方。 
    * **如果** 之前已停止 (，Play 将启动媒体查看器，或在当前条目)  
    * **"** 停止"可停止媒体查看器，并隐藏当前媒体。  
    * **Next/Prev** 跳到下一个或上一个媒体 
    * **x/x**  显示媒体列表中的当前索引，并允许跳转到列表中的任意点
    * **配置** 允许从 Web 门户重新输入新代码，以在控制台中设置新配置。 

现在，你已设置为通过多媒体控制台开始共享！  
 
## <a name="working-with-the-web-portal"></a>使用 Web 门户

Web 门户是一个 Web 应用，可用于配置多媒体控制台的各种功能。  这些功能分为两类：常规媒体控制台设置和媒体播放列表。

### <a name="multimedia-console-general-settings"></a>多媒体控制台常规设置

**Playback 设置**

媒体列表的常规播放设置

* **循环媒体列表**- 确定到达列表末尾后，媒体列表是否应该循环。
* **Start 方法** - 选择多媒体控制台启动的方法。
    * 手动 - 在启动媒体之前等待播放按钮按下
    * 自动从开始开始 - 从列表开头自动启动媒体列表
    * 自动启动随机 - 自动从列表中的随机起点启动媒体

**角色**

用于控制和配置多媒体控制台的角色分配。    这些角色分为以下集：

* **仅所有者** - 作为多媒体控制台会话所有者的用户
* **提升的用户** - 在最初配置多媒体控制台的空间内具有审查器或主机角色的用户
* **所有用户** - 所有用户

这些角色堆栈在这样一种意义上说，在此列表中选择的角色之上的所有角色也将被授予使用该功能的权限。  示例： **提升的用户** 包括 **所有者** ，即使他们不是 AltspaceVR 中的审查器或主机。 由角色分配控制的功能如下所示

* **可以控制媒体播放器** - 确定哪些角色可以控制多媒体控制台的媒体播放按钮
* **可以配置媒体播放器**- 通过授予对"配置"按钮的访问权限，确定哪些角色可以配置多媒体 **控制台**

### <a name="adding-photos-and-videos-to-the-media-list"></a>将照片和视频添加到媒体列表

媒体是多媒体控制台的核心。  多媒体控制台中支持将图像和视频链接作为媒体类型。  若要添加新媒体，请选择"添加图像"或"添加 **视频**"图标，弹出一个对话框以输入媒体信息和设置。  下面是媒体类型和关联设置的细分

**Image**

图像应为标准图像类型，例如 jpeg、png 和子图像。 它们需要托管在具有公共链接的某处。

* **名称** - (标识) 的必需名称。
* **图像 URL** - (必需) 图像的公共 URL
* **在** 之后跳过 - 应在之后跳过映像的秒数

**视频**

视频可以通过 Twitch 和 DLive 托管视频或实时流。   (其他支持可能执行额外的工作来获取正确的流 URL，但在多媒体控制台中并不完全支持) 

* **名称** - (标识) 的必需名称。
* **视频 URL** - (必需) 用于托管视频的公共 URL，或者提供实时流。
* **在** 之后跳过 - 在之后应跳过视频的秒数

> [!NOTE]
> 必需：将时间置于与视频长度匹配的时间，使视频能够正确转发。 例如，如果视频长 5 分钟，则 300 秒，否则视频不会跳到下一部分内容。

* **音量** - 视频的音量（从 0 开始 (分钟) - 1 (最大) 值。
* **开始时间** - 从视频开始开始的秒数。
* **关闭起始距离** - 离开多媒体控制台时，音量开始下降的距离（以米为单位）
* **视频结束操作** - 到达视频末尾后要执行的操作。
    * 停止 - 视频结束后，媒体列表停止
    * 循环 - 视频将循环，直到手动跳过
    * 下一步播放 - 媒体列表中的下一个媒体将在当前视频结束后启动。

## <a name="working-with-json-directly-advancedoptional"></a>直接使用 JSON (高级/可选) 

多媒体控制台支持在 AltspaceVR 中的控制台提示符下直接输入 JSON。  JSON 是启用媒体播放器配置的内部机制。 公开直接设置 JSON 的能力可让更高级的用户构建自己的工作流，以满足其需求和熟悉 JSON。  下面简要描述了 JSON 结构和 JSON 的验证架构。 有关以下属性的更详细说明，请参阅上述部分，其中介绍了如何配置多媒体控制台。  本部分主要介绍 JSON 数据的架构示例和结构。

### <a name="global-media-settings"></a>全局媒体设置

```json
{
  "loopMediaList": true | false
  "startMethod": "manual" | "autostart-beginning" | "autostart-random"
  "controlMediaPlayer": "everyone" | "elevated" | "owner"
  "configureMediaPlayer": "elevated" | "owner"
  ...
}
```

### <a name="media-list"></a>媒体列表

媒体列表是在 JSON 结构的根目录下设置的属性，如角色和播放设置。  它是一个简单的数组，可以包含以下媒体配置结构之一。  (请参阅上述属性说明，详细了解每个功能) 

**图像示例**

*必填字段："name"和"imageUrl"*

```json
{
    "name": "Altspace Screenshot",
    "imageUrl": "https://pbs.twimg.com/media/CxJ-fJqUsAAFtd9.jpg",
    "skipAfter": 10
}
```

**视频示例**

*必填字段："name"和"videoUrl"*

```json
{
    "name": "Ninja Twitch Live Stream",
    "videoUrl":"https://www.twitch.tv/ninja",
    "volume":0.2,
    "startTime":0,
    "endOfVideoAction":"play-next"
}
```

### <a name="example-json"></a>示例 JSON

```json
{
  "loopMediaList": false,
  "startMethod": "autostart-beginning",
  "controlMediaPlayer": "everyone",
  "configureMediaPlayer": "elevated",
  "mediaList": [
    {
      "videoUrl": "https://www.twitch.tv/ninja",
      "volume": 0.2,
      "startTime": 0,
      "endOfVideoAction": "play-next"
    },
    {
      "imageUrl": "http://www.hypergridbusiness.com/wp-content/uploads/2016/09/AltspaceVR-highrise.jpg",
      "skipAfter": 10
    },
    {
      "imageUrl": "https://d1qb2nb5cznatu.cloudfront.net/startups/i/333629-6ffd7199b9bcf34d8957e8e09d974a38-medium_jpg.jpg?buster=1423092095",
      "skipAfter": 5
    },
    {
      "imageUrl": "https://pbs.twimg.com/media/CxJ-fJqUsAAFtd9.jpg",
      "skipAfter": 10
    },
    {
      "imageUrl": "https://altvr-wpengine.netdna-ssl.com/wp-content/uploads/2019/05/Educators-in-VR-Social-VR-AltspaceVR.png",
      "skipAfter": 10
    },
    {
      "videoUrl": "https://www.twitch.tv/shroud",
      "volume": 1,
      "startTime": 0,
      "endOfVideoAction": "stop"
    }
  ]
}
```

### <a name="schema"></a>架构

```json
{
  "$schema": "https://json-schema.org/draft-04/schema#",
  "type": "object",
  "required": [
    "mediaList"
  ],
  "properties": {
    "loopMediaList": {
      "type": "boolean",
      "description": "Whether to loop through the media list when reaching the beginning or end of the list."
    },
    "controlMediaPlayer": {
      "type": "string",
      "enum": [
        "everyone",
        "elevated",
        "owner"
      ],
      "default": "owner",
      "description": "What roles are able to control the media player. (Owner can always control player)"
    },
    "configureMediaPlayer": {
      "type": "string",
      "enum": [
        "elevated",
        "owner"
      ],
      "default": "owner",
      "description": "What roles are allowed to configure the media play list.  Note: This role needs to be able to control the media player in order to configure it. (Owner can always configure media)"
    },
    "startMethod": {
      "type": "string",
      "enum": [
        "manual",
        "autostart-beginning",
        "autostart-random"
      ],
      "default": "manual",
      "description": "The method by which the media player should start"
    },
    "mediaList": {
      "description": "A list of images or videos to configure the media player to operate on.",
      "type": "array",
      "items": {
        "oneOf": [
          {
            "title": "Image",
            "type": "object",
            "description": "Configuration for an image media.",
            "properties": {
              "imageUrl": {
                "type": "string",
                "description": "The url for the image to load."
              },
              "skipAfter": {
                "type": "number",
                "minimum": 5,
                "default": null,
                "description": "The number of seconds that should pass before skipping to the next media. (Minimum 5)."
              }
            },
            "required": [
              "imageUrl"
            ]
          },
          {
            "title": "Video",
            "type": "object",
            "description": "Configuration for a video media.",
            "properties": {
              "videoUrl": {
                "type": "string",
                "description": "The url of the video to load."
              },
              "skipAfter": {
                "type": "number",
                "minimum": 5,
                "default": null,
                "description": "The number of seconds that should pass before skipping to the next media. (Minimum 5)."
              },
              "volume": {
                "type": "number",
                "minimum": 0,
                "maximum": 1,
                "default": null,
                "description": "The volume to play the video at. (Minimum 0, maximum 1)"
              },
              "startTime": {
                "type": "number",
                "minimum": 0,
                "default": null,
                "description": "The time in seconds from the start of the video to begin playing the video at. (Minimum of 0)"
              },
              "rolloffStartDistance": {
                "type": "number",
                "minimum": 0,
                "default": null,
                "description": "The distance in meters away from the media player that the volume will begin to fall off. (Minimum 0)"
              },
              "endOfVideoAction": {
                "type": "string",
                "enum": [
                  "stop",
                  "loop",
                  "play-next"
                ],
                "default": null,
                "description": "The type of action to take at the end of the video."
              }
            },
            "required": [
              "videoUrl"
            ]
          }
        ]
      }
    }
  }
}
```

> [!NOTE]
> 多媒体控制台 v0.5.0 是最新的