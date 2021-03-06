---
title: geochats.setTyping
description: Send typing notification to geochat
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Method: geochats.setTyping  
[Back to methods index](index.md)


Send typing notification to geochat

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|peer|[InputGeoChat](../types/InputGeoChat.md) | The geochat | Yes|
|typing|[Bool](../types/Bool.md) | Typing or not typing | Yes|


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

$Bool = $MadelineProto->geochats->setTyping(['peer' => InputGeoChat, 'typing' => Bool, ]);
```

### [PWRTelegram HTTP API](https://pwrtelegram.xyz) example (NOT FOR MadelineProto):

### As a bot:

POST/GET to `https://api.pwrtelegram.xyz/botTOKEN/madeline`

Parameters:

* method - geochats.setTyping
* params - `{"peer": InputGeoChat, "typing": Bool, }`



### As a user:

POST/GET to `https://api.pwrtelegram.xyz/userTOKEN/geochats.setTyping`

Parameters:

peer - Json encoded InputGeoChat

typing - Json encoded Bool




Or, if you're into Lua:

```lua
Bool = geochats.setTyping({peer=InputGeoChat, typing=Bool, })
```

