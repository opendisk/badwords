# Bad Words Filter Out for PHP

A php script to filter out bad words

## Installation:

```bash
composer require opendisk/badwords
```

### Usage:

```php
<?php

include 'vendor/autoload.php';

use Opendisk\Helper\Badwords;

$keyword = 'kamu sering nonton bokep';

$results1 = Badwords::isDirty($keyword); //when string contains bad words, it returns true

$results2 = Badwords::strip($keyword); //when string contains bad words, it replaces vocal chars in bad word with asterix

echo '<pre>';
print_r($results1);
echo '<br>';
print_r($results2);
```

**Result:** 
```
1
kamu sering nonton b*k*p
```
