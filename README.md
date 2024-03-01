Django Project
==============

This is a Docker (with docker-compose) environment for Django Project development.

# Installation

1. First, clone this repository:

```bash
$ git clone 
```

2. Init project
```bash
$ make
```

3. Show containers:
```bash
$ make ps
```
This results in the following running containers:

```bash
> $ docker-compose ps
Name          Command                          State     Ports
--------------------------------------------------------------------------------------
postgres      docker-entrypoint.sh postgres    Up        0.0.0.0:5432->5432/tcp
adminer       entrypoint.sh docker-php-e ...   Up        0.0.0.0:9000->8080/tcp
core          python manage.py runserver ...   Up        0.0.0.0:8000->8000/tcp
```
