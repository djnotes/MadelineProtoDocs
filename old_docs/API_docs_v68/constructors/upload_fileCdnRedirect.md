---
title: upload.fileCdnRedirect
description: File cdn redirect
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: upload.fileCdnRedirect  
[Back to constructors index](index.md)



File cdn redirect

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|dc\_id|[int](../types/int.md) | Yes|DC ID|
|file\_token|[bytes](../types/bytes.md) | Yes|File token|
|encryption\_key|[bytes](../types/bytes.md) | Yes|Encryption key|
|encryption\_iv|[bytes](../types/bytes.md) | Yes|Encryption iv|



### Type: [upload\_File](../types/upload_File.md)


### Example:

```php
$upload_fileCdnRedirect = ['_' => 'upload.fileCdnRedirect', 'dc_id' => int, 'file_token' => 'bytes', 'encryption_key' => 'bytes', 'encryption_iv' => 'bytes'];
```  

[PWRTelegram](https://pwrtelegram.xyz) json-encoded version:

```
{"_": "upload.fileCdnRedirect", "dc_id": int, "file_token": {"_": "bytes", "bytes":"base64 encoded bytes"}, "encryption_key": {"_": "bytes", "bytes":"base64 encoded bytes"}, "encryption_iv": {"_": "bytes", "bytes":"base64 encoded bytes"}}
```


Or, if you're into Lua:

```lua
upload_fileCdnRedirect={_='upload.fileCdnRedirect', dc_id=int, file_token='bytes', encryption_key='bytes', encryption_iv='bytes'}

```


