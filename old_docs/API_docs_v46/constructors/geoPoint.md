---
title: geoPoint
description: Geo point
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: geoPoint  
[Back to constructors index](index.md)



Geo point

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|longitude|[double](../types/double.md) | Yes|Longitude|
|latitude|[double](../types/double.md) | Yes|Latitude|



### Type: [GeoPoint](../types/GeoPoint.md)


### Example:

```php
$geoPoint = ['_' => 'geoPoint', 'longitude' => double, 'latitude' => double];
```  

[PWRTelegram](https://pwrtelegram.xyz) json-encoded version:

```
{"_": "geoPoint", "longitude": double, "latitude": double}
```


Or, if you're into Lua:

```lua
geoPoint={_='geoPoint', longitude=double, latitude=double}

```


