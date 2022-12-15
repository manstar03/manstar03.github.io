# Gambling-site
there is serveral gamblings.

##IBEX SOFTWARE

Requirements
 - php >= 8.0;
 - mysql >= 8.0;
 - composer >= 2.3;
 - node >= 14.0;
 - npm >= 7.0;

## Installation
    1.From the projects root folder run: 
        - `composer update`;
        - `php artisan migrate:fresh`;
        - `composer dump-autoload`;
        - `npm install`;
        - `npm run prod`;
    1.1. If you're using local development server:
        - run `php artisan db:seed` - this will create tenamy

## Structure
 - public/images/profiles - users avatar images path;

## Documentation
    Permissions
    In core of permissions checking (not creating) is used spatie/laravel-permission package. For creating and manupulating there's used `App\Services\Permission` service and appropriate fields in profiles database table: role, department.


    run `php artisan tenants:seed NotificationSettingsTableSeeder` to seed notification_settings table

