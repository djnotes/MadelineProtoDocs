---
title: channelAdminLogEventActionChangePhoto
description: Change photo
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: channelAdminLogEventActionChangePhoto  
[Back to constructors index](index.md)



Change photo

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|prev\_photo|[ChatPhoto](../types/ChatPhoto.md) | Optional|Previous photo|
|new\_photo|[ChatPhoto](../types/ChatPhoto.md) | Optional|New photo|



### Type: [ChannelAdminLogEventAction](../types/ChannelAdminLogEventAction.md)


### Example:

```php
$channelAdminLogEventActionChangePhoto = ['_' => 'channelAdminLogEventActionChangePhoto', 'prev_photo' => ChatPhoto, 'new_photo' => ChatPhoto];
```  

[PWRTelegram](https://pwrtelegram.xyz) json-encoded version:

```
{"_": "channelAdminLogEventActionChangePhoto", "prev_photo": ChatPhoto, "new_photo": ChatPhoto}
```


Or, if you're into Lua:

```lua
channelAdminLogEventActionChangePhoto={_='channelAdminLogEventActionChangePhoto', prev_photo=ChatPhoto, new_photo=ChatPhoto}

```


