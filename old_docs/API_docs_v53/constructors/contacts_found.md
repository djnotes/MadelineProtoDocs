---
title: contacts.found
description: Found
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: contacts.found  
[Back to constructors index](index.md)



Found

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|results|Array of [Peer](../types/Peer.md) | Yes|Results|
|chats|Array of [Chat](../types/Chat.md) | Yes|Chats|
|users|Array of [User](../types/User.md) | Yes|Users|



### Type: [contacts\_Found](../types/contacts_Found.md)


### Example:

```php
$contacts_found = ['_' => 'contacts.found', 'results' => [Peer, Peer], 'chats' => [Chat, Chat], 'users' => [User, User]];
```  

[PWRTelegram](https://pwrtelegram.xyz) json-encoded version:

```
{"_": "contacts.found", "results": [Peer], "chats": [Chat], "users": [User]}
```


Or, if you're into Lua:

```lua
contacts_found={_='contacts.found', results={Peer}, chats={Chat}, users={User}}

```


