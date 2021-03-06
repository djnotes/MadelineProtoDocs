---
title: messageMediaVideo
description: Message media video
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: messageMediaVideo  
[Back to constructors index](index.md)



Message media video

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|video|[Video](../types/Video.md) | Optional|Video|
|caption|[string](../types/string.md) | Yes|Caption|



### Type: [MessageMedia](../types/MessageMedia.md)


### Example:

```php
$messageMediaVideo = ['_' => 'messageMediaVideo', 'video' => Video, 'caption' => 'string'];
```  

[PWRTelegram](https://pwrtelegram.xyz) json-encoded version:

```
{"_": "messageMediaVideo", "video": Video, "caption": "string"}
```


Or, if you're into Lua:

```lua
messageMediaVideo={_='messageMediaVideo', video=Video, caption='string'}

```


