---
title: updateDeleteChannelMessages
description: Update delete channel messages
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: updateDeleteChannelMessages  
[Back to constructors index](index.md)



Update delete channel messages

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|channel\_id|[int](../types/int.md) | Yes|Channel ID|
|messages|Array of [int](../types/int.md) | Yes|Messages|
|channel\_pts|[int](../types/int.md) | Yes|Channel pts|
|channel\_pts\_count|[int](../types/int.md) | Yes|Channel pts count|



### Type: [Update](../types/Update.md)


### Example:

```php
$updateDeleteChannelMessages = ['_' => 'updateDeleteChannelMessages', 'channel_id' => int, 'messages' => [int, int], 'channel_pts' => int, 'channel_pts_count' => int];
```  

[PWRTelegram](https://pwrtelegram.xyz) json-encoded version:

```
{"_": "updateDeleteChannelMessages", "channel_id": int, "messages": [int], "channel_pts": int, "channel_pts_count": int}
```


Or, if you're into Lua:

```lua
updateDeleteChannelMessages={_='updateDeleteChannelMessages', channel_id=int, messages={int}, channel_pts=int, channel_pts_count=int}

```


