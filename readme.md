# Sentinel for Laravel 5.2

A basic implementation of the [Sentinel 2](https://cartalyst.com/manual/sentinel/2.0) authorization and authentication package for [laravel 5.2](https://laravel.com/docs/5.2) framework. Visitors can sign in as user, moderator or administrator and make use of their privileges. Only admin are allowed to manage users. Frontend theme is [bootstrap blog](http://startbootstrap.com/template-overviews/blog-home). 

## Installation

Make sure you have a running web server on your computer (for example xampp). Open your favorite CLI and move to the folder that will hold the project (typically C:\xampp\htdocs for xampp users). Then type the following commands: 

First clone the repo
```
git clone https://jeanquark@bitbucket.org/jeanquark/sentinel.git
```

Install all dependencies
```
composer install
```

Generate application key 
```
php artisan key:generate
```

Create a database that will hold sentinel tables. You can do so with phpmyadmin.
Open the .env.example file, edit it to match your database name, username and password and save it as .env file. Then build tables with command

```
php artisan migrate
```

Now fill the tables
```
php artisan db:seed
```

Nice. You should be good to go. Open your web browser and go to the login page of the application project (if you followed above-mentioned directives with xampp, path is: http://localhost/sentinel/public/login). Enter provided admin credentials and start managing users from the admin area.

## Features

1. Sign in page
2. Admin area with users management functionality.

## Screenshots

![homepage](https://github.com/jeanquark/sentinel/raw/master/public/homepage.png "Homepage")
![login](https://github.com/jeanquark/sentinel/raw/master/public/login.png "Login")
![alt text](https://github.com/jeanquark/sentinel/raw/master/public/admin.png "Admin")

### License
Please refer to [Sentinel 2 The BSD 3-Clause License](https://github.com/cartalyst/sentinel/blob/2.0/LICENSE).
