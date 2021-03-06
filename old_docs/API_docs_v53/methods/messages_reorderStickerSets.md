---
title: messages.reorderStickerSets
description: Reorder sticker sets
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Method: messages.reorderStickerSets  
[Back to methods index](index.md)


Reorder sticker sets

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|order|Array of [long](../types/long.md) | The order | Yes|


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

$Bool = $MadelineProto->messages->reorderStickerSets(['order' => [long, long], ]);
```

### [PWRTelegram HTTP API](https://pwrtelegram.xyz) example (NOT FOR MadelineProto):



### As a user:

POST/GET to `https://api.pwrtelegram.xyz/userTOKEN/messages.reorderStickerSets`

Parameters:

order - Json encoded  array of long




Or, if you're into Lua:

```lua
Bool = messages.reorderStickerSets({order={long}, })
```

