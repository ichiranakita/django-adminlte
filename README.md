# Django AdminLTE

Django AdminLTE is a smart admin based on adminLTE and django

[![Build Status](https://travis-ci.org/beastbikes/django-adminlte.svg?branch=master)](https://travis-ci.org/beastbikes/django-adminlte)

## Install

```shell
pip install django-adminlte-admin
```

## Quick start

1 Add "adminlte" to your INSTALLED_APPS setting like this::

```python
INSTALLED_APPS = [
    ...
    'adminlte.apps.AdminlteConfig',
]
```

2 Include the adminlte URLconf in your project urls.py like this::

```python
url(r'^adminlte/', include('adminlte.urls')),
```

3 Start the development server and visit http://127.0.0.1:8000/adminlte/
   to create a poll (you'll need the Admin app enabled).

4 Visit http://127.0.0.1:8000/adminlte/ to participate in the adminlte.

5 Look the examples in the code to see how to start.


## Settings

### ADMINLTE_LOGIN_VIEW

adminlte login view. default is `adminlte.login`

### ADMINLTE_IS_LOGIN_FUNC

adminlte login validate method. if `required_login=False` will not validate login


## Develop

```shell
rm dist/*
python setup.py sdist bdist_wheel
twine upload dist/*
```
