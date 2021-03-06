---
title: userContact
description: User contact
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: userContact  
[Back to constructors index](index.md)



User contact

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|id|[int](../types/int.md) | Yes|ID|
|first\_name|[string](../types/string.md) | Yes|First name|
|last\_name|[string](../types/string.md) | Yes|Last name|
|username|[string](../types/string.md) | Yes|Username|
|access\_hash|[long](../types/long.md) | Yes|Access hash|
|phone|[string](../types/string.md) | Yes|Phone|
|photo|[UserProfilePhoto](../types/UserProfilePhoto.md) | Optional|Photo|
|status|[UserStatus](../types/UserStatus.md) | Optional|Status|



### Type: [User](../types/User.md)


### Example:

```php
$userContact = ['_' => 'userContact', 'id' => int, 'first_name' => 'string', 'last_name' => 'string', 'username' => 'string', 'access_hash' => long, 'phone' => 'string', 'photo' => UserProfilePhoto, 'status' => UserStatus];
```  

[PWRTelegram](https://pwrtelegram.xyz) json-encoded version:

```
{"_": "userContact", "id": int, "first_name": "string", "last_name": "string", "username": "string", "access_hash": long, "phone": "string", "photo": UserProfilePhoto, "status": UserStatus}
```


Or, if you're into Lua:

```lua
userContact={_='userContact', id=int, first_name='string', last_name='string', username='string', access_hash=long, phone='string', photo=UserProfilePhoto, status=UserStatus}

```


