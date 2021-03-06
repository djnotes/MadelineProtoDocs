---
title: channels.readMessageContents
description: Mark channel/supergroup messages as read
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Method: channels.readMessageContents  
[Back to methods index](index.md)


Mark channel/supergroup messages as read

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|channel|[Username, chat ID, Update, Message or InputChannel](../types/InputChannel.md) | The channel | Optional|
|id|Array of [int](../types/int.md) | List of message IDs | Yes|


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

$Bool = $MadelineProto->channels->readMessageContents(['channel' => InputChannel, 'id' => [int, int], ]);
```

### [PWRTelegram HTTP API](https://pwrtelegram.xyz) example (NOT FOR MadelineProto):



### As a user:

POST/GET to `https://api.pwrtelegram.xyz/userTOKEN/channels.readMessageContents`

Parameters:

channel - Json encoded InputChannel

id - Json encoded  array of int




Or, if you're into Lua:

```lua
Bool = channels.readMessageContents({channel=InputChannel, id={int}, })
```

### Errors this method can return:

| Error    | Description   |
|----------|---------------|
|CHANNEL_INVALID|The provided channel is invalid|
|CHANNEL_PRIVATE|You haven't joined this channel/supergroup|


