---
title: messageEmpty
description: Empty message
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: messageEmpty  
[Back to constructors index](index.md)



Empty message

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|id|[int](../types/int.md) | Yes|ID|



### Type: [Message](../types/Message.md)


### Example:

```php
$messageEmpty = ['_' => 'messageEmpty', 'id' => int];
```  

[PWRTelegram](https://pwrtelegram.xyz) json-encoded version:

```
{"_": "messageEmpty", "id": int}
```


Or, if you're into Lua:

```lua
messageEmpty={_='messageEmpty', id=int}

```


