---
title: inputMessageVideoNote
description: Video note message
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: inputMessageVideoNote  
[Back to constructors index](index.md)



Video note message

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|video\_note|[InputFile](../types/InputFile.md) | Yes|Video note to send|
|thumb|[inputThumb](../constructors/inputThumb.md) | Yes|Video thumb, if available|
|duration|[int](../types/int.md) | Yes|Duration of the video in seconds|
|length|[int](../types/int.md) | Yes|Video width and height, should be positive and not greater than 640|



### Type: [InputMessageContent](../types/InputMessageContent.md)


