---
title: messages.uninstallStickerSet
description: Remove a sticker set
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Method: messages.uninstallStickerSet  
[Back to methods index](index.md)


Remove a sticker set

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|stickerset|[InputStickerSet](../types/InputStickerSet.md) | The sticker set to remove | Optional|


### Return type: [Bool](../types/Bool.md)

### Can bots use this method: **NO**


### MadelineProto Example:


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$Bool = $MadelineProto->messages->uninstallStickerSet(['stickerset' => InputStickerSet, ]);
```

### [PWRTelegram HTTP API](https://pwrtelegram.xyz) example (NOT FOR MadelineProto):



### As a user:

POST/GET to `https://api.pwrtelegram.xyz/userTOKEN/messages.uninstallStickerSet`

Parameters:

stickerset - Json encoded InputStickerSet




Or, if you're into Lua:

```lua
Bool = messages.uninstallStickerSet({stickerset=InputStickerSet, })
```

### Errors this method can return:

| Error    | Description   |
|----------|---------------|
|STICKERSET_INVALID|The provided sticker set is invalid|


