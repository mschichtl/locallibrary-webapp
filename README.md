# locallibrary-webapp

## Source
Following this tutorial [https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/skeleton_website].

## Steps to create blank app
Using Anaconda prompt and an environment with Python3 and Django pre-installed:
```
django-admin startproject locallibrary
python manage.py startapp catalog
```

## Settings
- Registered catalog app in `.\locallibrary\locallibrary\settings.py` under `INSTALLED_APPS`
- No changes to `DATABASES` settings necessary for now, will use SQLite
- Updated timezone to Europe/Berlin
