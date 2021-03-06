---
title: messages.getDocumentByHash
description: Get document by SHA256 hash
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Method: messages.getDocumentByHash  
[Back to methods index](index.md)


Get document by SHA256 hash

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|sha256|[bytes](../types/bytes.md) | `hash('sha256', $filename, true);` | Yes|
|size|[int](../types/int.md) | The file size | Yes|
|mime\_type|[string](../types/string.md) | The mime type of the file | Yes|


### Return type: [Document](../types/Document.md)

### Can bots use this method: **YES**


### MadelineProto Example:


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$Document = $MadelineProto->messages->getDocumentByHash(['sha256' => 'bytes', 'size' => int, 'mime_type' => 'string', ]);
```

### [PWRTelegram HTTP API](https://pwrtelegram.xyz) example (NOT FOR MadelineProto):

### As a bot:

POST/GET to `https://api.pwrtelegram.xyz/botTOKEN/madeline`

Parameters:

* method - messages.getDocumentByHash
* params - `{"sha256": {"_": "bytes", "bytes":"base64 encoded bytes"}, "size": int, "mime_type": "string", }`



### As a user:

POST/GET to `https://api.pwrtelegram.xyz/userTOKEN/messages.getDocumentByHash`

Parameters:

sha256 - Json encoded bytes

size - Json encoded int

mime_type - Json encoded string




Or, if you're into Lua:

```lua
Document = messages.getDocumentByHash({sha256='bytes', size=int, mime_type='string', })
```

### Errors this method can return:

| Error    | Description   |
|----------|---------------|
|SHA256_HASH_INVALID|The provided SHA256 hash is invalid|


