---
title: 使用多媒体控制台
description: 了解如何在 AltspaceVR 体验中开始配置、发布和 controling 多媒体控制台。
ms.date: 03/11/2021
ms.topic: article
keywords: 控制台，多媒体
ms.openlocfilehash: 601328eb6f266dbcfc9d81fc4f1c2d09ac62b318
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2021
ms.locfileid: "107211929"
---
# <a name="using-the-multimedia-console"></a>使用多媒体控制台

多媒体控制台是一个工具，可用于在事件和世界中共享媒体。 可以使用它来共享图像、演示文稿、livestreams、视频、播放列表等。 下面是有关如何使用多媒体控制台 **v 0.5.0 +** 的分步说明。 

## <a name="getting-started"></a>入门

多媒体控制台入门是一个由两个部分组成的过程。  首先，你将使用 web 门户为环境中放置的多媒体控制台会话生成和发布配置。  其次是在您的环境中放置实际的多媒体控制台应用程序，并设置它应使用的配置代码。

### <a name="configuring-the-multimedia-console-with-the-web-portal"></a>通过 web 门户配置多媒体控制台

1. 首先，您需要确保您的内容已联机托管，因为您需要 URL。  (可以将照片上传到 altvr.com，或将视频文件联机或使用 Twitch 实时流链接： https://www.twitch.tv/ninja) 
2. 导航到多媒体控制台的 web 门户，网址为： [https://multimedia-console.altvr.com/](https://multimedia-console.altvr.com/)
3. 从 web 门户中，可以为多媒体控制台生成和发布配置。  有关) 的各种属性的详细信息，请参阅下面的 (。
4. 将媒体输入媒体列表并配置了 "常规设置" 后，在应用程序的右上部分选择 "发布" 按钮。
5. 发布完成后，将弹出一个对话框，其中包含两个 word 代码，你可以在其中进入你所放置的多媒体控制台。
  
### <a name="placing-the-multimedia-console-in-your-environment"></a>将多媒体控制台放置在您的环境中

1. 选择 "在 **世界编辑器 > 编辑器" 面板 > SDK 应用 > 多媒体控制台**。  (不会转向 **> 基本 > SDK 应用程序的全球编辑器**-这适用于未注册的应用程序。 )   
2. 将多媒体控制台定位到最适合你的空间和受众。
3. 单击 "橙色编辑模式" 按钮即可退出编辑模式。
4. 系统将提示你 **是否是 media player 所有者？** 如果你是此多媒体控制台会话的官方所有者，请确认并继续。  (其他授权角色也可用。 请参阅下面的详细列表。 ) 
5. 选择 "是" 以确认你是主主机。  
6. 将弹出一个对话框，要求您从 web 门户或有效的 JSON 输入一个代码。  输入来自 web 门户的两个单词代码，包括短划线并单击 "确定"。  (JSON 是如下所述的高级配置) 
7. 多媒体控制台应在几秒钟后使用在 web 门户中生成的配置加载。

### <a name="controlling-the-multimedia-console"></a>控制多媒体控制台

1. 输入代码并完成配置过程后，会看到控件按钮显示在媒体显示下方。 
    * **播放** 会启动媒体查看器 (或在当前项重新启动（如果以前已停止）)  
    * **停止** 停止 media viewer，并隐藏当前媒体。  
    * **下一个/** 上一个跳转到下一个或上一个媒体 
    * **x/x**  在媒体列表中显示当前索引，并允许跳转到列表中的任何点
    * **Config** 允许重新从 web 门户重新设置新的代码，以便在控制台中设置新的配置。 

现在，你已设置为通过多媒体控制台开始共享！  
 
## <a name="working-with-the-web-portal"></a>使用 web 门户

Web 门户是一个 web 应用，可用于配置多媒体控制台的各种功能。  这些功能分为两类：常规媒体控制台设置和 media play 列表。

### <a name="multimedia-console-general-settings"></a>多媒体控制台常规设置

**Playback 设置**

媒体列表的常规播放设置

* **循环媒体列表**-确定一旦到达列表的末尾，介质列表是否应该循环进入。
* **启动方法** -选择多媒体控制台应启动的方法。
    * 手动-在启动媒体之前等待按下 "播放" 按钮
    * 自动开始开始-从列表的开头自动启动媒体列表
    * 自动启动随机-自动从列表中的随机起始点启动媒体

**角色**

用于控制和配置多媒体控制台的角色分配。    这些角色分为以下几组：

* **仅所有者** -用户是多媒体控制台会话的所有者
* **提升的用户** -在最初配置多媒体控制台的空间中具有仲裁者、主机或表示者角色的用户
* **所有用户** -所有用户

这些角色堆栈的意义在于，此列表中所选的所有角色都将被授予使用该功能的权限。  示例： **提升的用户** 包括 **所有者** ，即使他们不是 AltspaceVR 中的仲裁者、主机或表示器 * *。 由角色分配控制的功能如下所示

* **可以控制 media player** -确定哪些角色可以控制多媒体控制台的媒体播放按钮
* **可以配置 media player** -确定哪些角色可以通过向 " **配置** " 按钮授予访问权限来配置多媒体控制台

### <a name="adding-photos-and-videos-to-the-media-list"></a>将照片和视频添加到媒体列表

媒体是多媒体控制台的核心。  支持在多媒体控制台中将图像和视频链接作为媒体类型。  若要添加新媒体，请选择 " **添加映像** " 或 " **添加视频** " 图标以显示一个对话框，以输入媒体信息和设置。  下面是媒体类型和相关设置的细目分类

**图像**

图像应为标准图像类型，如 jpeg、png 和儿子。 它们需要托管在某个位置，并使用公用链接。

* **名称** - (需要用来标识映像的) 名称。
* **图像 URL** - (所需) 图像的公共 URL
* "**跳过**"-之后应跳过图像的秒数

**视频**

视频可以通过 Twitch 和 DLive 托管视频或实时流。   (其他支持可能会使用额外的工作来获取正确的流 url，但在多媒体控制台内不完全受支持) 

* **名称** - (需要用来标识视频的) 名称。
* **视频 URL** - (所需的) 视频所托管的公共 URL，或提供实时流。
* "**跳过**"-之后应跳过视频的秒数
* **卷** -从 0 (最小) -1 (最大) 值的视频量。
* **开始时间** -从视频开始开始的秒数（以秒为单位）。
* **开始距离** -在离开多媒体控制台时，在世界上以米为单位开始衰减的距离
* **视频结束操作** -到达视频末尾后要执行的操作。
    * 停止-媒体列表在视频结束后停止
    * 循环-视频将循环，直到手动跳过
    * 下一步-在当前视频结束后，介质列表中的下一个介质将启动。

## <a name="working-with-json-directly-advancedoptional"></a>直接使用 JSON (高级/可选) 

多媒体控制台支持直接在 AltspaceVR 中的控制台提示符下输入 JSON。  JSON 是一种内部机制，使用它可以实现媒体播放器配置。 通过公开设置 JSON 的功能，可使更高级的用户能够构建自己的工作流，这些工作流可满足其需求并熟悉 JSON。  下面是 JSON 结构的简短说明，以及 JSON 的验证架构。 有关以下属性的更多详细说明，请参阅上一节介绍了如何配置多媒体控制台。  本部分重点介绍用于 JSON 数据的架构示例和结构。

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

媒体列表是 JSON 结构的根目录中的属性集，如角色和播放设置。  它是一个简单的数组，它可以包含以下媒体配置结构之一。  (参见上面的属性说明了解每个操作的详细信息。 ) 

**图像示例**

*必填字段： "name" 和 "imageUrl"*

```json
{
    "name": "Altspace Screenshot",
    "imageUrl": "https://pbs.twimg.com/media/CxJ-fJqUsAAFtd9.jpg",
    "skipAfter": 10
}
```

**视频示例**

*必填字段： "name" 和 "videoUrl"*

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
> 多媒体控制台 v 0.5.0 的最新版本