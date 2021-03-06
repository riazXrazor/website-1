---
prev: 6_retrieve-visits-and-stats
next: 8_clear-and-reset-values
---

# Visits Lists
Top or Lowest list per model type

## Top/Lowest visited items per model
```php
visits('App\Post')->top(10);
```
```php
visits('App\Post')->low(10);
```

## Uncached list
```php
visits('App\Post')->fresh()->top(10);
```
> **Note:** you can always get uncached list by enabling `alwaysFresh` from config/visits.php file.

## By a period of time
```php
visits('App\Post')->period('month')->top(10);
```
> **Note** supported periods can be found in [periods-options](8_clear-and-reset-values.html#periods-options)