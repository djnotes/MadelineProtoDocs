---
title: messages.deleteHistory
description: Delete chat history
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Method: messages.deleteHistory  
[Back to methods index](index.md)


Delete chat history

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|peer|[Username, chat ID, Update, Message or InputPeer](../types/InputPeer.md) | Where to clear it | Optional|
|offset|[int](../types/int.md) | Offset | Yes|


### Return type: [messages\_AffectedHistory](../types/messages_AffectedHistory.md)

### Can bots use this method: **NO**


### MadelineProto Example:


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$messages_AffectedHistory = $MadelineProto->messages->deleteHistory(['peer' => InputPeer, 'offset' => int, ]);
```

### [PWRTelegram HTTP API](https://pwrtelegram.xyz) example (NOT FOR MadelineProto):



### As a user:

POST/GET to `https://api.pwrtelegram.xyz/userTOKEN/messages.deleteHistory`

Parameters:

peer - Json encoded InputPeer

offset - Json encoded int




Or, if you're into Lua:

```lua
messages_AffectedHistory = messages.deleteHistory({peer=InputPeer, offset=int, })
```

### Errors this method can return:

| Error    | Description   |
|----------|---------------|
|PEER_ID_INVALID|The provided peer id is invalid|


