## renefernandez.com personal website

[![Build Status](https://travis-ci.org/renefs/personal-site.svg?branch=master)](https://travis-ci.org/renefs/personal-site)

[![Maintainability](https://api.codeclimate.com/v1/badges/656018ee193b8014f31a/maintainability)](https://codeclimate.com/github/renefs/personal-site/maintainability)

[![Test Coverage](https://api.codeclimate.com/v1/badges/656018ee193b8014f31a/test_coverage)](https://codeclimate.com/github/renefs/personal-site/test_coverage)

Featuring:

- Docker v1.10.3
- Docker Compose v1.6.2
- Docker Machine v0.6.0
- Python 3.5

Blog post -> https://realpython.com/blog/python/django-development-with-docker-compose-and-machine/

### OS X Instructions

1. Start new machine - `docker-machine create -d virtualbox dev;`
1. Build images - `docker-compose build`
1. Start services - `docker-compose up -d`
1. Create migrations - `docker-compose run web /usr/local/bin/python manage.py migrate`
1. Grab IP - `docker-machine ip dev` - and view in your browser

    python manage.py makemessages -l <LANGUAGE_CODE>
    python manage.py makemessages -a
    python manage.py compilemessages