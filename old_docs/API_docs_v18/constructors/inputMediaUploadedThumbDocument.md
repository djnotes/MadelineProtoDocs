---
title: inputMediaUploadedThumbDocument
description: Media uploaded thumb document
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: inputMediaUploadedThumbDocument  
[Back to constructors index](index.md)



Media uploaded thumb document

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|file|[File path or InputFile](../types/InputFile.md) | Yes|File|
|thumb|[File path or InputFile](../types/InputFile.md) | Yes|Thumbnail|
|file\_name|[string](../types/string.md) | Yes|File name|
|mime\_type|[string](../types/string.md) | Optional|Mime type|



### Type: [InputMedia](../types/InputMedia.md)


### Example:

```php
$inputMediaUploadedThumbDocument = ['_' => 'inputMediaUploadedThumbDocument', 'file' => InputFile, 'thumb' => InputFile, 'file_name' => 'string', 'mime_type' => 'string'];
```  

[PWRTelegram](https://pwrtelegram.xyz) json-encoded version:

```
{"_": "inputMediaUploadedThumbDocument", "file": InputFile, "thumb": InputFile, "file_name": "string", "mime_type": "string"}
```


Or, if you're into Lua:

```lua
inputMediaUploadedThumbDocument={_='inputMediaUploadedThumbDocument', file=InputFile, thumb=InputFile, file_name='string', mime_type='string'}

```


