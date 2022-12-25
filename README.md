# LAB - Class 29

## Project: API deployment

### Author: Walaa' Atiyh  && Amani M Al-Zoubi

### databass `elephantsql`

#### How to initialize/run your application (where applicable)

1. **Create the venv and activate it.**

    `python3.10 -m venv .venv`
    `source .venv/bin/activate`


2. **install  requirements.txt**

   `pip3 install -r requirements.txt`


##  work with  docker
  1.  `docker-compose up --build`
  2.   `docker-compose run web python manage.py migrate`
  3.  `docker-compose run web python manage.py createsuperuser`

  4.  the admin

          username :Amani
                passward :amani
   5. the normal

            username :Walaa
            passward :walaa



Template Project for starting up CRUD API with Django Rest Framework

## Customization Steps

- DO NOT migrate yet
- add additional dependencies as needed
  - Re-export requirements.txt as needed
- change `things` folder to the app name of your choice
- Search through entire code base for `Thing`,`Things` and `things` to modify code to use your resource
  - `project/settings.py`
  - `project/urls.py`
  - App's files
    - `views.py`
    - `urls.py`
    - `admin.py`
    - `serializers.py`
    - `permissions.py`
- Update ThingModel with fields you need
  - Make sure to update other modules that would be affected by Model customizations. E.g. serializers, tests, etc.
- Rename `project/.env.sample` to `.env` and update as needed
- Run makemigrations and migrate commands
- Run `collectstatic` if needed.
- Optional: Update `api_tester.py`
- test 
