---
title: Installation
description: There are various ways to install MadelineProto:
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Installation

There are various ways to install MadelineProto:

* [Simple](#simple)
* [Simple (manual)](#simple-manual)
* [Composer from scratch](#composer-from-scratch)
* [Composer from existing project](#composer-from-existing-project)


## Simple

```php
<?php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
require_once 'madeline.php';
```

This code will automatically download, auto-update and include MadelineProto.


## Simple (manual)

Download [madeline.php](https://phar.madelineproto.xyz/madeline.php), put it in the same directory as your script, and then put the following code in your PHP file:
```php
<?php
require_once 'madeline.php';
```

## Composer from scratch

composer.json:
```
{
    "name": "yourname/yourproject",
    "description": "Project description",
    "type": "project",
    "require": {
        "danog/madelineproto": "dev-master",
        "amphp/dns": "dev-master#861cc857b1ba6e02e8a7439c30403682785fce96 as 0.9.9",
        "amphp/file": "dev-master#5a69fca406ac5fd220de0aa68c887bc8046eb93c as 0.3.3",
        "amphp/uri": "dev-master#f3195b163275383909ded7770a11d8eb865cbc86 as 0.1.3"
    },
    "repositories": [
        {
            "type": "git",
            "url": "https://github.com/danog/phpseclib"
        }
    ],
    "minimum-stability": "dev",
    "license": "AGPL-3.0-only",
    "authors": [
        {
            "name": "Daniil Gentili",
            "email": "daniil.gentili.dg@gmail.com"
        }
    ],
    "autoload": {
        "psr-0": {
            "Your\\Project\\": "src/"
        }
    }
}
```

Then run:
```bash
composer update
```

Put the following code in your PHP file:
```php
<?php
require_once 'vendor/autoload.php';
```

## Composer from existing project

Once you have all the requirements installed properly (on dev as well as production), add this to the ```composer.json``` file:

```
"repositories": [
    {
        "type": "git",
        "url": "https://github.com/danog/phpseclib"
    }
],
```

Make sure you also have these set in the composer.json:

```
"minimum-stability": "dev",
```

Then you can require the package by addding the following lines to the require section:

```
"danog/madelineproto":"dev-master",
"amphp/dns": "dev-master#861cc857b1ba6e02e8a7439c30403682785fce96 as 0.9.9",
"amphp/file": "dev-master#5a69fca406ac5fd220de0aa68c887bc8046eb93c as 0.3.3",
"amphp/uri": "dev-master#f3195b163275383909ded7770a11d8eb865cbc86 as 0.1.3"

```

<a href="https://docs.madelineproto.xyz/docs/UPDATES.html">Next section</a>
