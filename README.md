# Optional (alias)

This package is an alias to [`petrknap/optional`](https://packagist.org/packages/petrknap/optional).
It provides an aliased way to use the base functionality provided by the original package.

```php
use Optional\Optional;

/**
 * @param Optional<string> $nameOption
 */
function hello(Optional $nameOption) {
    echo "Hello, {$nameOption->orElse('World')}!" . PHP_EOL;
}

hello(Optional::empty());
hello(Optional::of('John'));
```

---

Run `composer require optional/optional` to install it.
