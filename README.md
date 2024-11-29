# cookiecutter-django


Simple cookiecutter for django

## Installation
First you must install [cookiecutter](https://cookiecutter.readthedocs.io/en/stable/installation.html):

    $ pip install cookiecutter

Then you can use it to generate a project:

    $ cookiecutter gh:brianmrdev/cookiecutter-django

## Folder structure
The generated project will be in the folder `my-project` (the name of your project) and will contain the following files:

    .
    ├── apps                                # contains all applications
    │   ├── accounts                        # django app for accounts
    │   │   ├── migrations                  # migrations for accounts app
    │   │   ├── tests                       # tests for accounts app
    │   │   │   └── test_models.py
    │   │   ├── admin.py
    │   │   ├── apps.py
    │   │   ├── models.py                   # models for accounts app
    │   │   ├── urls.py                     # urls for accounts app
    │   │   └── views.py
    │   ├── core                            # core application
    │   │   ├── migrations                  # migrations for core app
    │   │   ├── tests                       # tests
    │   │   │   ├── test_middleware.py
    │   │   │   ├── test_models.py
    │   │   │   ├── test_validators.py
    │   │   ├── apps.py
    │   │   ├── middleware                  # middlewares
    │   │   ├── models.py                   # basic models. Can be used by any application
    ├── config                              # contains all configuration files
    │   ├── settings                        # settings for project
    │   │   ├── base.py                     # base settings
    │   │   ├── develop.py                  # develop settings
    │   │   ├── production.py               # production settings
    │   │   └── staging.py                  # staging settings
    │   ├── asgi.py                         # asgi file (used by uvicorn)
    │   ├── wsgi.py                         # wsgi file (used by gunicorn)
    │   └── urls.py                         # urls main file
    ├── requirements                        # requirements folder
    │   ├── base.txt                        # base requirements
    │   ├── develop.txt                     # develop requirements
    │   ├── production.txt                  # production requirements
    │   ├── staging.txt                     # staging requirements
    │   └── test.txt                        # test requirements
    └── manage.py
