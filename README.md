# Template for WordPress projects with Composer

A bare minimum composer template for setting up and managing a WordPress project with Composer.

## How To Setup:

Please see requirements below before moving on to the steps.

### Requirements:
- Server with PHP / Apache (or Nginx) / MySQL (or PostreSQL)
- Git
- Composer

### Steps:

1. Clone this repository into your website projects folder:

```
git clone git@github.com:martingrondein/wordpress-composer-base.git
```

2. Install this desired setup with Composer:

```
cd wordpress-composer-base
composer install
```

3. Copy web/index.php to your project folder. You can do this from the command line with

```
cp web/index.php ./index.php
```

4. Slightly modify index.php in your project root. The index.php in the root of your project (the one you just created via a copy command) should be modified.

So...
```
require( dirname( __FILE__ ) . '/wp-blog-header.php' );
```
... becomes ...
```
require( dirname( __FILE__ ) . '/web/wp-blog-header.php' );
```
--- 
Please note: This is a no-frills composer.json template.
