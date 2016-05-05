# my-silex-docker-skeleton

### Installation

```sh
$ git clone [git-repo-url] <project-name>
$ cd <project-name>
$ composer install
```

#### composer.json

Change the namespace

```sh
{
    ...
    "autoload": {
        "psr-4": {
            "<CHANGE-NAMESPACE>\\": "src/"
        }
    }
}
```

#### docker/.env

Set your environment

```sh
# API ENV
DB_HOST=mysql
DB_NAME=app
DB_USERNAME=app
DB_PASSWORD=secret

# MYSQL ENV
MYSQL_DATABASE=app
MYSQL_USER=app
MYSQL_PASSWORD=secret
MYSQL_ROOT_PASSWORD=secret
```

### Run

```sh
$ docker-compose up
```