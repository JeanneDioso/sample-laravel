# Getting started

## Installation

Please check the official laravel installation guide for server requirements before you start. [Official Documentation](https://laravel.com/docs/5.4/installation#installation)

Alternative installation is possible without local dependencies relying on [Docker](#docker). 

Clone the repository

    git clone git@github.com:JeanneDioso/laravel-exam.git

Switch to the repo folder

    cd laravel-exam

Install all the dependencies using composer

    composer install

Copy the example env file and make the required configuration changes in the .env file

    cp .env.example .env

Generate a new application key

    php artisan key:generate

Generate a new JWT authentication secret key

    php artisan jwt:generate

Run the database migrations (**Set the database connection in .env before migrating**)

    php artisan migrate

Start the local development server

    php artisan serve

You can now access the server. Example: http://127.0.0.1:8000
    
**Make sure you set the correct database connection information before running the migrations** 

    php artisan migrate
    php artisan serve

# Test Endpoints

    /api/auth/register
    /api/auth/login
    /api/products/order

