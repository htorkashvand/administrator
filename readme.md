# Laravel Administrator

Administrator is an administrative interface builder for [Laravel](http://laravel.com). With Administrator you can visually manage your Eloquent models and their relations, and also create stand-alone settings pages for storing site data and performing site tasks.

- **Author:** Hamed Torkashvand
- **Website:** [http://htorkashvand.github.io]
- **Version:** 1.0.0

[![Build Status](https://travis-ci.org/FrozenNode/Laravel-Administrator.png?branch=master)](https://travis-ci.org/FrozenNode/Laravel-Administrator)

<img src="https://raw.github.com/FrozenNode/Laravel-Administrator/master/examples/images/overview.jpg" />

## Composer

To install Administrator as a Composer package to be used with Laravel 5, simply run:

```sh
composer require htorkashvand/administrator

```

Once it's installed, you can register the service provider in `config/app.php` in the `providers` array:

```php
'providers' => [
	Frozennode\Administrator\AdministratorServiceProvider::class,
]
```

Then publish Administrator's assets with `php artisan vendor:publish`. This will add the file `config/administrator.php`. This [config file](http://administrator.frozennode.com/docs/configuration) is the primary way you interact with Administrator. This command will also publish all of the assets, views, and translation files.

```php

for use first time :

1- add auth to laravel like: 'php artisan make:auth' ,
2- register user ... ,
3- add 'users' in 'administrator.php' Like :'menu' => ['users'] ,
4- add directory to config directory: 'administrator/settings' ,
5- add file users.php in directory administrator ,
6- config users for use in panel admin .


```


## Documentation

The complete docs for Administrator can be found at http://administrator.frozennode.com. You can also find the docs in the `/src/docs` directory.