---
title: account.resetAuthorization
description: Delete a certain session
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Method: account.resetAuthorization  
[Back to methods index](index.md)


Delete a certain session

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|hash|[long](../types/long.md) | The session hash, obtained from $MadelineProto->account->getAuthorizations | Yes|


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

$Bool = $MadelineProto->account->resetAuthorization(['hash' => long, ]);
```

### [PWRTelegram HTTP API](https://pwrtelegram.xyz) example (NOT FOR MadelineProto):



### As a user:

POST/GET to `https://api.pwrtelegram.xyz/userTOKEN/account.resetAuthorization`

Parameters:

hash - Json encoded long




Or, if you're into Lua:

```lua
Bool = account.resetAuthorization({hash=long, })
```

### Errors this method can return:

| Error    | Description   |
|----------|---------------|
|HASH_INVALID|The provided hash is invalid|


