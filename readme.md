# Laravel & PHP & NGINX & MYSQL - Dockerised

![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![Laravel](https://img.shields.io/badge/laravel-%23FF2D20.svg?style=for-the-badge&logo=laravel&logoColor=white)
![MySQL](https://img.shields.io/badge/mysql-%2300f.svg?style=for-the-badge&logo=mysql&logoColor=white)
![PHP](https://img.shields.io/badge/php-%23777BB4.svg?style=for-the-badge&logo=php&logoColor=white)
![Nginx](https://img.shields.io/badge/nginx-%23009639.svg?style=for-the-badge&logo=nginx&logoColor=white)
![NPM](https://img.shields.io/badge/NPM-%23000000.svg?style=for-the-badge&logo=npm&logoColor=white)
![NodeJS](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white)

An empty sample Laravel project for Docker,
Using:
PHP @ 8.1
NGINX @ Stable
MYSQL @ Latest
Composer & Npm with NodeJS @ Latest

## How to run the project

1. Copy the mysql.env.example in the env folder to mysql.env and fill out the project details

2. Install the vendor dependencies<br>
   `docker-compose run --rm composer install`

3. Copy the .env.example found in <strong>src</strong> to .env and fill out the project details making sure they match the mysql.env values.

4. Generate a new app key by running<br>
   `docker-compose run --rm artisan key:generate`

5. Start the server and start developing<br>
   `docker-compose up -d server`

### Other commands:

> You can stop the server with `docker-compose down`<br>
> All artisan commands with `docker-compose run --rm artisan [your input]`<br>
> All composer commands with `docker-compose run --rm composer [your input]`<br>
> All npm commands with `docker-compose run --rm npm [your input]`<br>

### Sidenote:

Database is not persistent, let me know if you need it to be 😉
