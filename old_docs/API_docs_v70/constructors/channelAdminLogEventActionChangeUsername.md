---
title: channelAdminLogEventActionChangeUsername
description: Change username
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: channelAdminLogEventActionChangeUsername  
[Back to constructors index](index.md)



Change username

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|prev\_value|[string](../types/string.md) | Yes|Prev value|
|new\_value|[string](../types/string.md) | Yes|New value|



### Type: [ChannelAdminLogEventAction](../types/ChannelAdminLogEventAction.md)


### Example:

```php
$channelAdminLogEventActionChangeUsername = ['_' => 'channelAdminLogEventActionChangeUsername', 'prev_value' => 'string', 'new_value' => 'string'];
```  

[PWRTelegram](https://pwrtelegram.xyz) json-encoded version:

```
{"_": "channelAdminLogEventActionChangeUsername", "prev_value": "string", "new_value": "string"}
```


Or, if you're into Lua:

```lua
channelAdminLogEventActionChangeUsername={_='channelAdminLogEventActionChangeUsername', prev_value='string', new_value='string'}

```


