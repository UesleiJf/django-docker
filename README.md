# README

## Description

This application was developed using the Python language and Django for web framework.

For the development of the Rest API, the use of the DRF.

### Work environment details

* OS: Ubuntu 16.04 LTS
* IDE: PyCharm Community
* Terminal: Terminal
* Database: sqlite3
* Docker
* Docker Compose

### Library Versions

* Python:   3.6
* Django:   2.2
* Babel: 2.6.0
* Django Rest Framework: 3.9.3
* dj-database-url: 0.5.0
* dj-static: 0.0.6
* python-dateutil: 2.8.0
* django-rest-swagger: 2.2.0

### Installation

First, you need to clone this project from Bitbucket:

https://github.com/UesleiJf/django-docker

This project run under Python 3.6 and Django 2.2

After clone, you need to install all the requirements. 

The Python >= 3.3 comes with venv to creating lightweight "virtual environments".

For this project, python3.6 was used

For full documentation for venv, you can see here:
https://docs.python.org/3/library/venv.html

To create an enviroment, run:

    python3.6 -m venv /path/to/new/virtual/environment

Run the command below to update the pip and avoid dependency conflicts when installing requirements.txt

    pip install --upgrade pip

Navigate to the directory /systemcall/ and execute the commands below

Now, you can install al the project requirements:

    pip install -r requirements.txt

After this, just execute the commands makemigrations and migrate to create project tables

    python3.6 manage.py makemigrations

    python3.6 manage.py migrate

    python3.6 manage.py collectstatic

Now, you can start the project:

    docker-compose up
