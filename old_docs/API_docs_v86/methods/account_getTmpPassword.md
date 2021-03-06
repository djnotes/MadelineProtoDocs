---
title: account.getTmpPassword
description: Get temporary password for buying products through bots
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Method: account.getTmpPassword  
[Back to methods index](index.md)


Get temporary password for buying products through bots

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|password|[InputCheckPasswordSRP](../types/InputCheckPasswordSRP.md) | Password | Yes|
|period|[int](../types/int.md) | The validity period | Yes|


### Return type: [account\_TmpPassword](../types/account_TmpPassword.md)

### Can bots use this method: **NO**


### MadelineProto Example:


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$account_TmpPassword = $MadelineProto->account->getTmpPassword(['password' => InputCheckPasswordSRP, 'period' => int, ]);
```

### [PWRTelegram HTTP API](https://pwrtelegram.xyz) example (NOT FOR MadelineProto):



### As a user:

POST/GET to `https://api.pwrtelegram.xyz/userTOKEN/account.getTmpPassword`

Parameters:

password - Json encoded InputCheckPasswordSRP

period - Json encoded int




Or, if you're into Lua:

```lua
account_TmpPassword = account.getTmpPassword({password=InputCheckPasswordSRP, period=int, })
```

### Errors this method can return:

| Error    | Description   |
|----------|---------------|
|PASSWORD_HASH_INVALID|The provided password hash is invalid|
|TMP_PASSWORD_DISABLED|The temporary password is disabled|


