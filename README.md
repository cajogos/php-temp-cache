# TempCache [![Latest Stable Version](https://poser.pugx.org/cajogos/php-temp-cache/v/stable)](https://packagist.org/packages/cajogos/php-temp-cache) [![License](https://poser.pugx.org/cajogos/php-temp-cache/license)](https://packagist.org/packages/cajogos/php-temp-cache) [![Monthly Downloads](https://poser.pugx.org/cajogos/php-temp-cache/d/monthly)](https://packagist.org/packages/cajogos/php-temp-cache)

A simple PHP caching class that uses the temporary files (`/tmp/`) folder of a Linux distribution.

## Simple to Use

The class has been written to be dead easy to use and should be familiar to anyone who has used any caching before. However, beware that the main aim of this cache is **not to be the fastest caching mechanism out there**, but to simplify the lives of those who just want to have a simple caching system in place to avoid hitting API limits, although from my experience it is pretty fast!

### Storing (put)

```php
// $expire is time in seconds for validity.

TempCache::put($key, $value, $expire);
```

### Retrieving (get)

```php
TempCache::get($key);
```

### Deleting (remove)

```php
TempCache::remove($key);
```

## Features

* No need to install extra plugins or PHP modules.
* Works out of the box. (As long as your web server use has enough privileges).
* Extremely use to implement to avoid hitting those API limits.

## Getting Started

**Warning**: You need PHP >= 5.3 to use TempCache.

### Using Composer

```javascript
{
	"require": {
		"cajogos/php-temp-cache": "1.0.1"
	}
}
```

### Download and use

The class is **self-contained** so you can use it in any project you already have by using:

```php
require_once 'classes/TempCache.php';
```

## Contributors
- [Carlos Ferreira](https://github.com/cajogos)

Want to help contribute or thank me? Get in touch via <c@rlos.rocks>.

_You are awesome!_