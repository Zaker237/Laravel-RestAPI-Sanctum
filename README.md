# REST API with Laravel using Sanctum for Auth

This repos is a simple RestFull API with Laravel using Santum for Auth.

## Requirements

The requirement to test this are:

* A Web server
* php >= 7.0.0
* Composer 
* A database

## Setup the database

To setup the database, create a .env file at the Root of the project and copy the content of the file .env.example in that file. The following database ca be used:

* Postgres
* MySQL
* SQL Server
* MariaDB
* Sqlite

In our case we are using sqlite and our config are the following and the database will be a file with the name `database.sqlite` in the folder `database`.

```
DB_CONNECTION=sqlite
DB_HOST=127.0.0.1
DB_PORT=3306
```

To use another database, just update this configs. The following comfig can work with MYSQL:

```
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=<database>
DB_USERNAME=<username>
DB_PASSWORD=<password>
```

## How to run

To test just clone the repo and run the migration using the following command at the root of the project.

```console
php artisan migrate
```

After running The migration you can now start the web server and start to browse the endpoints.