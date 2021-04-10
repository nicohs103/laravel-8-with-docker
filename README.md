Requirements

- PHP 7
- Docker
- Composer 2
- Optional: MySQL Workbench
- Optional: Kitematic


--------------------------------------------------


Installation

-> Open terminal:
git clone https://github.com/nicohs103/laravel-8-with-docker
cd laravel-8-with-docker
composer install
./vendor/bin/sail up

-> Config Mysql Workbench (Or use console)
localhost:3306
User: root
No password

-> In the MySql container:
CREATE SCHEMA `databasename` DEFAULT CHARACTER SET utf8 COLLATE utf8_spanish2_ci;

-> In the app container
php artisan migrate --seed

-> Navigate to localhost !!
--------------------------------------------------

This project make the containers for php server, mysql, redis, mailhog, meilisearch, selenium
