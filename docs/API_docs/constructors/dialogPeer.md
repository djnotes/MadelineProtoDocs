---
title: dialogPeer
description: Dialog peer
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: dialogPeer  
[Back to constructors index](index.md)



Dialog peer

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|peer|[Peer](../types/Peer.md) | Yes|Peer|



### Type: [DialogPeer](../types/DialogPeer.md)


### Example:

```php
$dialogPeer = ['_' => 'dialogPeer', 'peer' => Peer];
```  

[PWRTelegram](https://pwrtelegram.xyz) json-encoded version:

```
{"_": "dialogPeer", "peer": Peer}
```


Or, if you're into Lua:

```lua
dialogPeer={_='dialogPeer', peer=Peer}

```


