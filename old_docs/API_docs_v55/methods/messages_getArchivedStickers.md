---
title: messages.getArchivedStickers
description: Get all archived stickers
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Method: messages.getArchivedStickers  
[Back to methods index](index.md)


Get all archived stickers

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|offset\_id|[long](../types/long.md) | Sticker ID offset | Yes|
|limit|[int](../types/int.md) | Number of stickers to fetch | Yes|


### Return type: [messages\_ArchivedStickers](../types/messages_ArchivedStickers.md)

### Can bots use this method: **NO**


### MadelineProto Example:


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$messages_ArchivedStickers = $MadelineProto->messages->getArchivedStickers(['offset_id' => long, 'limit' => int, ]);
```

### [PWRTelegram HTTP API](https://pwrtelegram.xyz) example (NOT FOR MadelineProto):



### As a user:

POST/GET to `https://api.pwrtelegram.xyz/userTOKEN/messages.getArchivedStickers`

Parameters:

offset_id - Json encoded long

limit - Json encoded int




Or, if you're into Lua:

```lua
messages_ArchivedStickers = messages.getArchivedStickers({offset_id=long, limit=int, })
```

