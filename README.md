# Davee's Django Rest API Template

## Author: Davee Sok

## Links & Resources

- [Django](https://docs.djangoproject.com/en/3.2/)
- [Django Rest Framework](https://www.django-rest-framework.org/)

## Overview/ Motivation

work in progess....

Starting up a Django api can be time consuming. This template is meant to get up and running fast

## Tools & Dependencies

- Django
- Django Rest Framework
- Black
- Docker

## Getting Started

### 1. Create a New Secret Key by running the following command in the terminal:

```iterm
python -c 'from django.core.management.utils import get_random_secret_key; \
            print(get_random_secret_key())'
```

### 2. You will get a 50 digit key. Add new key to settings.py line 23

```python
SECRET_KEY = "django-insecure-INSERT_NEW_SECRET_KEY_HERE"
```

### 3. App folder currently called "Example". Replace all occurences of "Example" with a name of your choosing

- These steps will change the app name and all occurences of "Example"
- Replace "Example" folder name (pick any name, make it lowercase)
- Replace "Example" on line 6 in app.py with the name you picked
- Fix urlpatterns on line 19 in a_project.settings.py
- This step requires using a Capital Letter: Do a global search of "Example" and replace all occurences with the name you chose earlier. Remember to select "Match Case" and "Match Whole Word" option.

### 4. In terminal run the following commands:

```iterm
poetry install
python manage.py makemigrations
python manage.py migrate
```

---

#### Other Commands To Know

```python
poetry export -f requirements.txt -o requirements.txt
docker-compose up
docker-compose -d
docker-compose down
docker-compose logs
docker-compose up --build
```
