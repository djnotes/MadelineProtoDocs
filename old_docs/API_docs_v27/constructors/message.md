---
title: message
description: Message
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: message  
[Back to constructors index](index.md)



Message

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|id|[int](../types/int.md) | Yes|ID|
|from\_id|[int](../types/int.md) | Yes|From ID|
|to\_id|[Peer](../types/Peer.md) | Yes|To ID|
|fwd\_from\_id|[int](../types/int.md) | Optional|Forwarded from ID|
|fwd\_date|[int](../types/int.md) | Optional|Forwarded date|
|reply\_to\_msg\_id|[int](../types/int.md) | Optional|Reply to msg ID|
|date|[int](../types/int.md) | Yes|Date|
|message|[string](../types/string.md) | Yes|Message|
|media|[MessageMedia](../types/MessageMedia.md) | Optional|Media|



### Type: [Message](../types/Message.md)


### Example:

```php
$message = ['_' => 'message', 'id' => int, 'from_id' => int, 'to_id' => Peer, 'fwd_from_id' => int, 'fwd_date' => int, 'reply_to_msg_id' => int, 'date' => int, 'message' => 'string', 'media' => MessageMedia];
```  

[PWRTelegram](https://pwrtelegram.xyz) json-encoded version:

```
{"_": "message", "id": int, "from_id": int, "to_id": Peer, "fwd_from_id": int, "fwd_date": int, "reply_to_msg_id": int, "date": int, "message": "string", "media": MessageMedia}
```


Or, if you're into Lua:

```lua
message={_='message', id=int, from_id=int, to_id=Peer, fwd_from_id=int, fwd_date=int, reply_to_msg_id=int, date=int, message='string', media=MessageMedia}

```


