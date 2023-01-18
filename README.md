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

## Views
- Registered catalog app in `.\locallibrary\locallibrary\urls.py`:
```
urlpatterns += [
    path('catalog/', include('catalog.urls')),
]
```
- Adding a redirect from `127.0.0.1:8000` to `127.0.0.1:8000/catalog/`
- Updated URL mapping to serve static files
- Added basic (blank) version of `.\locallibrary\catalog\urls.py`