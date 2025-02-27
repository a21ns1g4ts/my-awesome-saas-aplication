# Filament SaaS

[![GitHub license](https://img.shields.io/github/license/gothinkster/laravel-realworld-example-app.svg)](/LICENSE)

## Introduction

The purpose of this project is provide a simple way to create web aplications. We use [Laravel](https://laravel.com/) framework with [Filament Admin](https://filamentphp.com/).

## Getting started

### Installation

Please check the official laravel installation guide for server requirements before you start. [Official Documentation](https://laravel.com/docs/5.8/installation#installation)

Clone the repository:

    git clone https://github.com/A2Insights/filament-saas-template.git

Switch to the repo folder:

    cd filament-saas-template

Install all php dependencies using composer:

    composer install

Install all node dependencies using npm:

    npm install

Compile the css and javascript assets:

    npm run dev

Copy the example env file and config the database credentials.

    cp .env.example .env

> See all env vars available in the .env.example file.

Generate a new application key:

    php artisan key:generate

Flush de application cache:

    php artisan config:clear
    php artisan view:clear

Run the database migrations.

    php artisan migrate

PS: Make sure you set the correct database connection information before running the migrations.

Start the local development server:

    php artisan serve

You can now access the server at <http://127.0.0.1:8000>

### Using Laravel Sail to develop

make .env config:

    DB_CONNECTION=mysql
    DB_HOST=sail
    DB_PORT=3306
    DB_DATABASE=mydb
    DB_USERNAME=sail
    DB_PASSWORD=password

And run:

    php artisan config:clear

    sail up

You can now access the server at <http://localhost>

### Install app

To install, run the following command:

    php artisan filament-saas:install

This command will install the filament-saas app. You can find the implementation details of this command [here](https://github.com/A2Insights/filament-saas/blob/main/src/Commands/FilamentSaasCommand.php).

got to <http://127.0.0.1:8000/sysadmin/login> and login with the following credentials:

#### Super Admin
- **Email:** `super_admin@filament-saas.dev`
- **Senha:** `123456`

#### Admin 
- **Email:** `admin@filament-saas.dev`
- **Senha:** `123456`

#### User 
- **Email:** `user@filament-saas.dev`
- **Senha:** `123456`


**For more information: <https://laravel.com/docs/sail>**

## Changelog

Please see [CHANGELOG](CHANGELOG.md) for more information what has changed recently.

## Contributing

Please see [CONTRIBUTING](CONTRIBUTING.md) for details.

## Security

If you discover any security related issues, please email atila.danvi@outlook.com instead of using the issue tracker.

## Credits

-   [Atila Silva](https://github.com/a21ns1g4ts)
-   [All Contributors](../../contributors)

## License

The MIT License. Please see [license file](LICENSE.md) for more information.
