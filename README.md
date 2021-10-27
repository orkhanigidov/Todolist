# Todo List App with Laravel and Vue.js

## Table of contents

- [About Application](#about-application)
- [Technologies](#technologies)
- [API Endpoints](#api-endpoints)
- [Setup Docker](#setup-docker)
- [Configuration](#configuration)
- [Install Dependencies](#install-dependencies)
- [Run Migration](#run-migration)
- [Run Application](#run-application)
- [Testing](#testing)

## About Application

- Create and update todos
- Delete or mark todo as complete

## Technologies

- [Laravel](https://laravel.com/)
- [Vue.js](https://vuejs.org/)
- [Laravel Sail](https://laravel.com/docs/8.x/sail)
- [MySQL](https://www.mysql.com/)
- [PHPUnit](https://phpunit.de/)
- [Docker](https://www.docker.com/)

## API Endpoints

Method | Route | Description
--- | --- | ---
`GET` | `/api/items` | Fetch all the todos
`POST` | `/api/item/store` | Create an todo
`PUT` | `api/item/:id` | Update the todo
`DELETE` | `/api/item/:id` | Delete the todo

## Setup Docker

```
$ git clone https://github.com/orkhanigidov/Todolist.git
$ cd Todolist
$ docker-compose up
$ cp .env.example .env
```

## Configuration

Fill out relevant items in your `.env` file, including:

```
DB_DATABASE=
DB_USERNAME=
DB_PASSWORD=
```

## Install Dependencies

```
$ composer install
$ npm install
```

## Run Migration

```
$ php artisan migrate
```

## Run Application

```
$ php artisan serve
$ npm run watch
```
Open http://127.0.0.1:80/ in the browser

## Testing

```
$ ./vendor/bin/phpunit
```

## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
