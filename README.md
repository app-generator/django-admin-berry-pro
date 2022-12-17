# **Django Admin Berry PRO**

**Django** starter styled with **Berry Dashboard PRO**, a premium `Boostrap 5` design from [CodedThemes](https://codedthemes.com/?ref=appseed)
The product is designed to deliver the best possible user experience with highly customizable feature-rich pages. 

> 👉 **NOTE**: This product `requires a License` in order to access the theme:

**Private REPO**: `git+https://github.com/app-generator/priv-django-admin-berry-pro`

<br />

## Features: 

- **UI Kit**: Berry BS5 PRO `v1.0.1` by CodedThemes
- [Django Berry Dashboard](https://github.com/app-generator/django-berry-dashboard-pro) - `sample project`
- **Sections Covered**: 
  - `Admin Section`, reserved for `superusers`
  - `All pages` managed by `Django.contrib.AUTH`
  - `Registration` page
  - `Misc pages`: colors, icons, typography, blank-page 

<br />

![Berry Bootstrap 5 - Dark-Mode ready, Open-source Template.](https://user-images.githubusercontent.com/51070104/207091062-e805b36c-663a-4a01-acb8-9c55ab914f4f.jpg)

<br />

## Why `Django Admin Berry PRO`

- Modern [Bootstrap 5](https://www.admin-dashboards.com/bootstrap-5-templates/) Design
- `Responsive Interface`
- `Minimal Template` overriding
- `Easy integration`

Berry Dashboard comes with error/bug-free, well structured codebase that renders nicely in all major browsers and devices. 

<br />

## How to use it

<br />

> **Install the package** via `PIP` 

```bash
$ pip install git+https://github.com/app-generator/priv-django-admin-berry-pro.git
```

<br />

> Add `admin_berry` application to the `INSTALLED_APPS` setting of your Django project `settings.py` file (note it should be before `django.contrib.admin`):

```python
    INSTALLED_APPS = (
        ...
        'admin_berry_pro.apps.AdminBerryProConfig',
        'django.contrib.admin',
    )
```

<br />

> Add `LOGIN_REDIRECT_URL` and `EMAIL_BACKEND` of your Django project `settings.py` file:

```python
    LOGIN_REDIRECT_URL = '/'
    # EMAIL_BACKEND = 'django.core.mail.backends.smtp.EmailBackend'
    EMAIL_BACKEND = 'django.core.mail.backends.console.EmailBackend'
```

<br />

> Add `admin_berry_pro` urls in your Django Project `urls.py` file

```python
    from django.urls import path, include

    urlpatterns = [
        ...
        path('', include('admin_berry_pro.urls')),
    ]
```

<br />

> **Collect static** if you are in `production environment`:

```bash
$ python manage.py collectstatic
```

<br />

> **Start the app**

```bash
$ # Set up the database
$ python manage.py makemigrations
$ python manage.py migrate
$
$ # Create the superuser
$ python manage.py createsuperuser
$
$ # Start the application (development mode)
$ python manage.py runserver # default port 8000
```

Access the `admin` section in the browser: `http://127.0.0.1:8000/`

<br />

## Screenshots

@todo

---
**Django Admin Berry PRO** - Modern Admin Interface provided by **[AppSeed](https://appseed.us/)**
