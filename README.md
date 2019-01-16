# Laravel HiveOS Api
Laravel package for interacting with Hive OS api

## Installation

[PHP](https://php.net) 7.1+ and [Composer](https://getcomposer.org) are required.

To get the latest version of HiveOs api, simply run the code below in your project.

```
"composer require krios-mane/hive-os"
```
Once Laravel HiveOs is installed, You need to register the service provider. Open up `config/app.php` and add the following to the `providers` key.

* `KriosMane\HiveOs\app\Providers\HiveOsServiceProvider::class,`

Also, register the Facade like so:

```php
'aliases' => [
    ...
    'HiveOs' => KriosMane\HiveOs\app\Facades\HiveOs::class,
    ...
]
```

## Configuration

You can publish the configuration file using this command:

```bash
php artisan vendor:publish --provider="KriosMane\HiveOs\app\Providers\HiveOsServiceProvider"
```

A configuration-file named `hiveos.php` with default settings will be placed in your `config` directory:

You can visit this link to get your HiveOS api

```
https://the.hiveos.farm/login
```

## Usage

Open your .env file and add the following in this format. Ensure you must have gotten your api key:

```php
HIVEOS_LOGIN=johndoe
HIVEOS_PASSWORD=password
HIVEOS_ACCESS_TOKEN=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ91e123asdas
```

## USING /KRIOS-MANE/HIVE-OS PACKAGE 
```
Add the following line to your controller

use \HiveOs;
```


## Contributing

Please feel free to fork this package and contribute by submitting a pull request to enhance the functionalities.

## How can I thank you?

Why not star the github repo? I'd love the attention! Why not share the link for this repository on Twitter or HackerNews? Spread the word!


Thanks!
Krios Mane

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.

