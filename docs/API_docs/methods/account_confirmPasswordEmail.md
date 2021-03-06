---
title: account.confirmPasswordEmail
description: Confirm password recovery using email
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Method: account.confirmPasswordEmail  
[Back to methods index](index.md)


Confirm password recovery using email

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|code|[string](../types/string.md) | Code | Yes|


### Return type: [Bool](../types/Bool.md)

### Can bots use this method: **YES**


### MadelineProto Example:


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$Bool = $MadelineProto->account->confirmPasswordEmail(['code' => 'string', ]);
```

### [PWRTelegram HTTP API](https://pwrtelegram.xyz) example (NOT FOR MadelineProto):

### As a bot:

POST/GET to `https://api.pwrtelegram.xyz/botTOKEN/madeline`

Parameters:

* method - account.confirmPasswordEmail
* params - `{"code": "string", }`



### As a user:

POST/GET to `https://api.pwrtelegram.xyz/userTOKEN/account.confirmPasswordEmail`

Parameters:

code - Json encoded string




Or, if you're into Lua:

```lua
Bool = account.confirmPasswordEmail({code='string', })
```

