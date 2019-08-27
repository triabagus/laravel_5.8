<p align="center"><img src="https://laravel.com/assets/img/components/logo-laravel.svg"></p>

# Tutorial Laravel 5.8

## 1. Setting file .env 
    Create Database mysql and update
~~~php
    DB_DATABASE=Name_Database
    DB_USERNAME=Username_Database
    DB_PASSWORD=Password_Database
~~~

## 2. Setting Models Folder
```    
    1. Create Folder Models in App
    2. Move User.php to Folder Models
    3. Update namespace in file auth.php , User.php , RegisterController.php 
```
> auth.php
~~~php
    'providers' => [
        'users' => [
            'driver' => 'eloquent',
            'model' => App\Models\User::class, //update same is it.
        ],
~~~
> User.php
~~~php
    namespace App\Models; //update is it.
~~~
> RegisterController.php
~~~php
    use App\Models\User; //update is it.
~~~
