---
title: account.initTakeoutSession
description: Start account exporting session
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Method: account.initTakeoutSession  
[Back to methods index](index.md)


Start account exporting session

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|contacts|[Bool](../types/Bool.md) | Export contacts? | Optional|
|message\_users|[Bool](../types/Bool.md) | Export users? | Optional|
|message\_chats|[Bool](../types/Bool.md) | Export chats? | Optional|
|message\_megagroups|[Bool](../types/Bool.md) | Export supergroups? | Optional|
|message\_channels|[Bool](../types/Bool.md) | Export channel messages? | Optional|
|files|[Bool](../types/Bool.md) | Export files? | Optional|
|file\_max\_size|[int](../types/int.md) | Export only files smaller than this size | Optional|


### Return type: [account\_Takeout](../types/account_Takeout.md)

### Can bots use this method: **YES**


### MadelineProto Example:


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$account_Takeout = $MadelineProto->account->initTakeoutSession(['contacts' => Bool, 'message_users' => Bool, 'message_chats' => Bool, 'message_megagroups' => Bool, 'message_channels' => Bool, 'files' => Bool, 'file_max_size' => int, ]);
```

### [PWRTelegram HTTP API](https://pwrtelegram.xyz) example (NOT FOR MadelineProto):

### As a bot:

POST/GET to `https://api.pwrtelegram.xyz/botTOKEN/madeline`

Parameters:

* method - account.initTakeoutSession
* params - `{"contacts": Bool, "message_users": Bool, "message_chats": Bool, "message_megagroups": Bool, "message_channels": Bool, "files": Bool, "file_max_size": int, }`



### As a user:

POST/GET to `https://api.pwrtelegram.xyz/userTOKEN/account.initTakeoutSession`

Parameters:

contacts - Json encoded Bool

message_users - Json encoded Bool

message_chats - Json encoded Bool

message_megagroups - Json encoded Bool

message_channels - Json encoded Bool

files - Json encoded Bool

file_max_size - Json encoded int




Or, if you're into Lua:

```lua
account_Takeout = account.initTakeoutSession({contacts=Bool, message_users=Bool, message_chats=Bool, message_megagroups=Bool, message_channels=Bool, files=Bool, file_max_size=int, })
```

