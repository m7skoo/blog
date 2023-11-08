<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400"></a></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## About Simple Blogging API - Laravel

This is a simple REST API for a blogging project built using Laravel. This README will guide you through the process of initializing and running the project.

## Prerequisites
- Before you begin, ensure you have met the following requirements:

Composer: Make sure you have Composer installed. You can download it https://getcomposer.org/download/.

## Getting Started
Follow these steps to get the project up and running:

1. Clone the repository to your local machine:
   git clone https://github.com/m7skoo/blog.git

2. Navigate to the project directory:
 " Make sure you path to save the project file on your device " 

3. Install the project dependencies using Composer:
   Use this command  "composer install"

4. Create a copy of the .env.example file and name it .env. Update the database connection settings, and any other configuration options you need
   cp .env.example .env

5. Generate an application key:
   Use this command  php artisan key:generate

6. Run the database migrations to create the necessary database tables:
  Use this command  php artisan migrate

7.  you can seeder the database with sample data:
    (a) php artisan migrate --seed
    (b) php artisan db:seed PostSeeder
    (C) php artisan db:seed AdminSeeder

8. Start the development server: By default, the application will be accessible at 'http://127.0.0.1:8000'.


## API Endpoints
The API provides the following endpoints:


POST /api/login
POST /api/register
GET /api/posts: Get a list of all blog posts.
GET /api/posts/{id}: Get a specific blog post by ID.
POST /api/posts: Create a new blog post.
PUT /api/posts/{id}: Update a specific blog post by ID.
DELETE /api/posts/{id}: Delete a specific blog post by ID.

Make requests to these endpoints using your preferred API client or tools like Postman or cURL.

## Authentication
  "This project includes authentication JONS file. You may want to implement authentication according to your specific requirements. Alternatively, you can allow users to create a token through the login or registration page. This token gives each user the ability to create a blog. Retrieve a list of all blogs , access a single post by its ID, update an existing blog post by its ID, or delete it by its user ID.”

 
 
 “I hope I conveyed the mission information to you effectively.”


