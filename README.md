# PHPAuto
PHPAuto is a small cli tool for generating an PHP autoload.php file for your namespace utilizing project.

All you need to do is run this tool in your php root and import the new `autoload.php` file in your php endpoints.

For Single page applications you can easily import it in the start of your `index.php`.

Example:
```bash
cd /var/www/html/mywebsite
phpauto -d # -d is used for dumping the result into an autoload.php file.
```

Add the following to the top of your `index.php`
```php
require(__DIR__ . "/autoload.php");
```

## For development
To install dependencies:

```bash
bun install
```

To run:

```bash
bun run index.ts
```

This project was created using `bun init` in bun v1.1.10. [Bun](https://bun.sh) is a fast all-in-one JavaScript runtime.
