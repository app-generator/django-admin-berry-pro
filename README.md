# **[Django Admin Berry PRO](https://appseed.us/product/berry-dashboard-pro/django/)**

**Django** starter styled with **[Berry Dashboard PRO](https://appseed.us/product/berry-dashboard-pro/django/)**, a premium `Boostrap 5` design from [CodedThemes](https://codedthemes.com/?ref=appseed)
The product is designed to deliver the best possible user experience with highly customizable feature-rich pages. 

> 👉 **NOTE**: This product `requires a License` in order to access the theme:

**Private REPO**: `git+https://github.com/app-generator/priv-django-admin-berry-pro`

<br />

## Features: 

- **UI Kit**: Berry BS5 PRO `v1.0.1` by CodedThemes
- [Django Berry PRO](https://appseed.us/product/berry-dashboard-pro/django/) - `sample project`
- **Sections Covered**: 
  - `Admin Section`, reserved for `superusers`
  - `All pages` managed by `Django.contrib.AUTH`
  - `Registration` page
  - `Misc pages`: colors, icons, typography, blank-page 

<br />

![Berry Bootstrap 5 PRO - Premium Template Django Template.](https://user-images.githubusercontent.com/51070104/210833058-be0b3e87-4f2b-4765-b84d-3795ba03c6a1.jpg)

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

![Berry Pro - Premium full-stack starter crafted by AppSeed.](https://user-images.githubusercontent.com/51070104/210833261-af09bc29-0894-4d21-84ad-8e8853f8cbe1.jpg)

<br />

> **Django Berry PRO** - `Kanban Board`

![Berry Pro, Kanban Board - Premium full-stack starter crafted by AppSeed](https://user-images.githubusercontent.com/51070104/210833567-e26f67e1-53c8-430a-8add-e4d6c874266a.jpg)

<br />

> **Django Berry PRO** - `Kanban Board`

![Berry Pro, Widgets page - Premium full-stack starter crafted by AppSeed](https://user-images.githubusercontent.com/51070104/210833737-76643967-02f6-4342-9545-1ffaba68343f.jpg)

<br />

> **Django Berry PRO** - `eCommerce`

![Berry Pro, eCommerce page - Premium full-stack starter crafted by AppSeed](https://user-images.githubusercontent.com/51070104/210834456-344fbcb5-4a32-45ed-964e-b808dbc53356.jpg)

<br />

---
**[Django Admin Berry PRO](https://appseed.us/product/berry-dashboard-pro/django/)** - Modern Admin Interface provided by **[AppSeed](https://appseed.us/)**
