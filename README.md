# pesantren
Web untuk pesantren bersama Maskur (Masjid sebagai Kampus untuk Rakyat)

<p align="center"><img src="https://res.cloudinary.com/dtfbvvkyp/image/upload/v1566331377/laravel-logolockup-cmyk-red.svg" width="400"></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/d/total.svg" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/v/stable.svg" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/license.svg" alt="License"></a>
</p>

## About Pesantren
- [Based on Laravel 6.x](https://laravel.com)
- [User Management by jeremykenedy](https://github.com/jeremykenedy/laravel-users).
- [User Role by jeremykenedy](https://github.com/jeremykenedy/laravel-roles).

## How to Start
- Create a MySQL database locally named ```pesantren``` utf8_general_ci
- Install [composer](https://getcomposer.org)
- Clone this project ```git clone https://github.com/kovzone/pesantren.git```
- Rename .env.example file to ```.env``` and fill the database information
- Run ```composer install```
- Run ```php artisan key:generate```
- Run ```php artisan migrate```
- Run ```php artisan db:seed```
- Run ```php artisan serve```
- Open [http://127.0.0.1:8000](http://127.0.0.1:8000)
- Register Admin User
- Update database ```pesantren``` using ```phpmyadmin``` or other tools. Insert data to ```user_role``` like this commands:
```
INSERT INTO `role_user` (`id`, `role_id`, `user_id`, `created_at`, `updated_at`, `deleted_at`) VALUES (NULL, '1', '1', NULL, NULL, NULL);
```