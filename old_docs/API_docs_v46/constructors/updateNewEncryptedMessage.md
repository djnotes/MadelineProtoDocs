---
title: updateNewEncryptedMessage
description: Update new encrypted message
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: updateNewEncryptedMessage  
[Back to constructors index](index.md)



Update new encrypted message

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|encr\_message|[EncryptedMessage](../types/EncryptedMessage.md) | Yes|Encr message|
|qts|[int](../types/int.md) | Yes|Qts|



### Type: [Update](../types/Update.md)


### Example:

```php
$updateNewEncryptedMessage = ['_' => 'updateNewEncryptedMessage', 'encr_message' => EncryptedMessage, 'qts' => int];
```  

[PWRTelegram](https://pwrtelegram.xyz) json-encoded version:

```
{"_": "updateNewEncryptedMessage", "encr_message": EncryptedMessage, "qts": int}
```


Or, if you're into Lua:

```lua
updateNewEncryptedMessage={_='updateNewEncryptedMessage', encr_message=EncryptedMessage, qts=int}

```


