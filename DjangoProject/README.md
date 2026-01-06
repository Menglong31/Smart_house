#Django Project Setup Guide
##Requirements

bash
```python3 --version```
```pip3 --version```

##Create Project Directory

```mkdir django-project```
```cd django-project```

##Create Virtual Environment

```python3 -m venv venv```

##Activate Virtual Environment

###Linux / macOS

```source venv/bin/activate```

###Windows

```venv\Scripts\activate```

##Install Django

```pip install django```

##Verify Django Installation

```django-admin --version```

##Create Django Project

```django-admin startproject config .```

##Create Django App

```python manage.py startapp students```

##Register App

###Add the app to config/settings.py:

```
INSTALLED_APPS = [
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',
    'students',
]
```

##Database Migration

```python manage.py makemigrations```
```python manage.py migrate```

##Create Superuser

```python manage.py createsuperuser```

##Run Development Server

```python manage.py runserver```

Open in browser:

http://127.0.0.1:8000/
http://127.0.0.1:8000/admin/


