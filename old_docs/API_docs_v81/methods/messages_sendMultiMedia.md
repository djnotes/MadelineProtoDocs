---
title: messages.sendMultiMedia
description: Send an album
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Method: messages.sendMultiMedia  
[Back to methods index](index.md)


Send an album

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|silent|[Bool](../types/Bool.md) | Disable notifications? | Optional|
|background|[Bool](../types/Bool.md) | Disable background notification? | Optional|
|clear\_draft|[Bool](../types/Bool.md) | Clear draft? | Optional|
|peer|[Username, chat ID, Update, Message or InputPeer](../types/InputPeer.md) | Where to send the album | Optional|
|reply\_to\_msg\_id|[int](../types/int.md) | Reply to message by ID | Optional|
|multi\_media|Array of [InputSingleMedia](../types/InputSingleMedia.md) | The album | Yes|


### Return type: [Updates](../types/Updates.md)

### Can bots use this method: **YES**


### MadelineProto Example:


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$Updates = $MadelineProto->messages->sendMultiMedia(['silent' => Bool, 'background' => Bool, 'clear_draft' => Bool, 'peer' => InputPeer, 'reply_to_msg_id' => int, 'multi_media' => [InputSingleMedia, InputSingleMedia], ]);
```

### [PWRTelegram HTTP API](https://pwrtelegram.xyz) example (NOT FOR MadelineProto):

### As a bot:

POST/GET to `https://api.pwrtelegram.xyz/botTOKEN/madeline`

Parameters:

* method - messages.sendMultiMedia
* params - `{"silent": Bool, "background": Bool, "clear_draft": Bool, "peer": InputPeer, "reply_to_msg_id": int, "multi_media": [InputSingleMedia], }`



### As a user:

POST/GET to `https://api.pwrtelegram.xyz/userTOKEN/messages.sendMultiMedia`

Parameters:

silent - Json encoded Bool

background - Json encoded Bool

clear_draft - Json encoded Bool

peer - Json encoded InputPeer

reply_to_msg_id - Json encoded int

multi_media - Json encoded  array of InputSingleMedia




Or, if you're into Lua:

```lua
Updates = messages.sendMultiMedia({silent=Bool, background=Bool, clear_draft=Bool, peer=InputPeer, reply_to_msg_id=int, multi_media={InputSingleMedia}, })
```

