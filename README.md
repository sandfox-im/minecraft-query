# Minecraft Server Query

**This library is not maintained. Please use some supported library like this one: https://github.com/xPaw/PHP-Minecraft-Query**

A PHP library for checking the status of an enabled Minecraft server ported from python
[https://github.com/Dinnerbone/mcstatus](https://github.com/Dinnerbone/mcstatus)

## Installation

Add the following code to your composer file.

```json
{
    "require": {
        "sandfox-im/bencode": "^1.0"
    }
}
```

## Usage

```php
<?php

$minecraft = new \SandFoxIM\Minecraft\ServerQuery($argv[1], $argv[2], 2);

echo "Basic info:\n";
var_export($minecraft->getStatus());

echo "Full info:\n";
var_export($minecraft->getRules());
```
