---
title: messages.getWebPage
description: Get webpage preview
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Method: messages.getWebPage  
[Back to methods index](index.md)


Get webpage preview

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|url|[string](../types/string.md) | URL | Yes|
|hash|Array of [int](../types/int.md) |  the hash parameter of the previous result of this method | Optional|


### Return type: [WebPage](../types/WebPage.md)

### Can bots use this method: **NO**


### MadelineProto Example:


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$WebPage = $MadelineProto->messages->getWebPage(['url' => 'string', 'hash' => [int, int], ]);
```

### [PWRTelegram HTTP API](https://pwrtelegram.xyz) example (NOT FOR MadelineProto):



### As a user:

POST/GET to `https://api.pwrtelegram.xyz/userTOKEN/messages.getWebPage`

Parameters:

url - Json encoded string

hash - Json encoded  array of int




Or, if you're into Lua:

```lua
WebPage = messages.getWebPage({url='string', hash={int}, })
```

### Errors this method can return:

| Error    | Description   |
|----------|---------------|
|WC_CONVERT_URL_INVALID|WC convert URL invalid|


