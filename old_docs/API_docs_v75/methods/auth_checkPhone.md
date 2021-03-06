---
title: auth.checkPhone
description: Check if this phone number is registered on telegram
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Method: auth.checkPhone  
[Back to methods index](index.md)


Check if this phone number is registered on telegram

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|phone\_number|[string](../types/string.md) | The phone number to check | Yes|


### Return type: [auth\_CheckedPhone](../types/auth_CheckedPhone.md)

### Can bots use this method: **NO**


### MadelineProto Example:


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$auth_CheckedPhone = $MadelineProto->auth->checkPhone(['phone_number' => 'string', ]);
```

### [PWRTelegram HTTP API](https://pwrtelegram.xyz) example (NOT FOR MadelineProto):



### As a user:

POST/GET to `https://api.pwrtelegram.xyz/userTOKEN/auth.checkPhone`

Parameters:

phone_number - Json encoded string




Or, if you're into Lua:

```lua
auth_CheckedPhone = auth.checkPhone({phone_number='string', })
```

### Errors this method can return:

| Error    | Description   |
|----------|---------------|
|PHONE_NUMBER_BANNED|The provided phone number is banned from telegram|
|PHONE_NUMBER_INVALID|The phone number is invalid|
|PHONE_NUMBER_INVALID|The phone number is invalid|


