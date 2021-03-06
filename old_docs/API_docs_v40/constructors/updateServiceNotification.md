---
title: updateServiceNotification
description: Update service notification
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: updateServiceNotification  
[Back to constructors index](index.md)



Update service notification

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|type|[string](../types/string.md) | Yes|Type|
|message|[string](../types/string.md) | Yes|Message|
|media|[MessageMedia](../types/MessageMedia.md) | Optional|Media|
|popup|[Bool](../types/Bool.md) | Yes|Popup?|



### Type: [Update](../types/Update.md)


### Example:

```php
$updateServiceNotification = ['_' => 'updateServiceNotification', 'type' => 'string', 'message' => 'string', 'media' => MessageMedia, 'popup' => Bool];
```  

[PWRTelegram](https://pwrtelegram.xyz) json-encoded version:

```
{"_": "updateServiceNotification", "type": "string", "message": "string", "media": MessageMedia, "popup": Bool}
```


Or, if you're into Lua:

```lua
updateServiceNotification={_='updateServiceNotification', type='string', message='string', media=MessageMedia, popup=Bool}

```


