---
title: webPage
description: Web page
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: webPage  
[Back to constructors index](index.md)



Web page

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|id|[long](../types/long.md) | Yes|ID|
|url|[string](../types/string.md) | Yes|URL|
|display\_url|[string](../types/string.md) | Yes|Display URL|
|hash|[int](../types/int.md) | Yes|Hash|
|type|[string](../types/string.md) | Optional|Type|
|site\_name|[string](../types/string.md) | Optional|Site name|
|title|[string](../types/string.md) | Optional|Title|
|description|[string](../types/string.md) | Optional|Description|
|photo|[Photo](../types/Photo.md) | Optional|Photo|
|embed\_url|[string](../types/string.md) | Optional|Embed URL|
|embed\_type|[string](../types/string.md) | Optional|Embed type|
|embed\_width|[int](../types/int.md) | Optional|Embed width|
|embed\_height|[int](../types/int.md) | Optional|Embed height|
|duration|[int](../types/int.md) | Optional|Duration|
|author|[string](../types/string.md) | Optional|Author|
|document|[Document](../types/Document.md) | Optional|Document|
|cached\_page|[Page](../types/Page.md) | Optional|Cached page|



### Type: [WebPage](../types/WebPage.md)


### Example:

```php
$webPage = ['_' => 'webPage', 'id' => long, 'url' => 'string', 'display_url' => 'string', 'hash' => int, 'type' => 'string', 'site_name' => 'string', 'title' => 'string', 'description' => 'string', 'photo' => Photo, 'embed_url' => 'string', 'embed_type' => 'string', 'embed_width' => int, 'embed_height' => int, 'duration' => int, 'author' => 'string', 'document' => Document, 'cached_page' => Page];
```  

[PWRTelegram](https://pwrtelegram.xyz) json-encoded version:

```
{"_": "webPage", "id": long, "url": "string", "display_url": "string", "hash": int, "type": "string", "site_name": "string", "title": "string", "description": "string", "photo": Photo, "embed_url": "string", "embed_type": "string", "embed_width": int, "embed_height": int, "duration": int, "author": "string", "document": Document, "cached_page": Page}
```


Or, if you're into Lua:

```lua
webPage={_='webPage', id=long, url='string', display_url='string', hash=int, type='string', site_name='string', title='string', description='string', photo=Photo, embed_url='string', embed_type='string', embed_width=int, embed_height=int, duration=int, author='string', document=Document, cached_page=Page}

```


