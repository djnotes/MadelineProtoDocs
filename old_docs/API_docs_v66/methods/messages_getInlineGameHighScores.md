---
title: messages.getInlineGameHighScores
description: Get high scores of a game sent in an inline message
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Method: messages.getInlineGameHighScores  
[Back to methods index](index.md)


Get high scores of a game sent in an inline message

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|id|[InputBotInlineMessageID](../types/InputBotInlineMessageID.md) | The inline message | Yes|
|user\_id|[Username, chat ID, Update, Message or InputUser](../types/InputUser.md) | The user that set the high scores | Optional|


### Return type: [messages\_HighScores](../types/messages_HighScores.md)

### Can bots use this method: **YES**


### MadelineProto Example:


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$messages_HighScores = $MadelineProto->messages->getInlineGameHighScores(['id' => InputBotInlineMessageID, 'user_id' => InputUser, ]);
```

### [PWRTelegram HTTP API](https://pwrtelegram.xyz) example (NOT FOR MadelineProto):

### As a bot:

POST/GET to `https://api.pwrtelegram.xyz/botTOKEN/madeline`

Parameters:

* method - messages.getInlineGameHighScores
* params - `{"id": InputBotInlineMessageID, "user_id": InputUser, }`



### As a user:

POST/GET to `https://api.pwrtelegram.xyz/userTOKEN/messages.getInlineGameHighScores`

Parameters:

id - Json encoded InputBotInlineMessageID

user_id - Json encoded InputUser




Or, if you're into Lua:

```lua
messages_HighScores = messages.getInlineGameHighScores({id=InputBotInlineMessageID, user_id=InputUser, })
```

### Errors this method can return:

| Error    | Description   |
|----------|---------------|
|MESSAGE_ID_INVALID|The provided message id is invalid|
|USER_BOT_REQUIRED|This method can only be called by a bot|


