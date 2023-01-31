# **[Django Admin Berry PRO](https://appseed.us/product/berry-dashboard-pro/django/)**

**Django** starter styled with **[Berry Dashboard PRO](https://appseed.us/product/berry-dashboard-pro/django/)**, a premium `Bootstrap 5` design from [CodedThemes](https://codedthemes.com/?ref=appseed)
The product is designed to deliver the best possible user experience with highly customizable feature-rich pages. 

> 👉 **NOTE**: This product `requires a License` in order to access the theme:

**Private REPO**: `git+https://github.com/app-generator/priv-django-admin-berry-pro`

<br />

## Features: 

- **UI Kit**: Berry BS5 PRO `v1.0.1` by CodedThemes
- [Django Berry PRO](https://appseed.us/product/berry-dashboard-pro/django/) - `Product` that uses the library
  - `Features`: Fully-configured, `CI/CD` via Render
- **Sections Covered**: 
  - `Admin Section`, reserved for `superusers`
  - `All pages` managed by `Django.contrib.AUTH`
  - `Registration` page
  - `Misc pages`: colors, icons, typography, blank-page 

<br />

![Berry Bootstrap 5 PRO - Premium Template Django Template.](https://user-images.githubusercontent.com/51070104/215728155-9b9cfe26-96e8-49c3-8a08-131d96f4f2eb.png)

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

> Add `admin_berry_pro` application to the `INSTALLED_APPS` setting of your Django project `settings.py` file (note it should be before `django.contrib.admin`):

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

## How to Customize 

When a template file is loaded in the controller, `Django` scans all template directories starting from the ones defined by the user, and returns the first match or an error in case the template is not found. 
The  theme used to style this starter provides the following files: 

```bash
< LIBRARY_ROOT >                      # This exists in ENV: LIB/admin_berry_pro
   |
   |-- templates/                     # Root Templates Folder 
   |    |          
   |    |-- accounts/       
   |    |    |-- login-v1.html        # Sign IN Page
   |    |    |-- register-v1.html     # Sign UP Page
   |    |
   |    |-- includes/       
   |    |    |-- footer.html          # Footer component
   |    |    |-- sidebar.html         # Sidebar component
   |    |    |-- navigation.html      # Navigation Bar
   |    |    |-- scripts.html         # Scripts Component
   |    |
   |    |-- layouts/       
   |    |    |-- base.html            # Masterpage
   |    |    |-- base-fullscreen.html # Masterpage for Auth Pages
   |    |
   |    |-- pages/       
   |         |-- index.html           # INDEX page
   |         |-- dashboard/index.html # Main dashboard page
   |         |-- widgets/data.html    # Widgets page
   |         |-- *.html               # All other pages
   |    
   |-- ************************************************************************
```

When the project requires customization, we need to copy the original file that needs an update (from the virtual environment) and place it in the template folder using the same path. 

For instance, if we want to customize the `footer.html` these are the steps:

- `Step 1`: create the `templates` DIRECTORY inside your app 
- `Step 2`: configure the project to use this new template directory
  - Edit `settings.py` TEMPLATES section 
- `Step 3`: copy the `footer.html` from the original location (inside your ENV) and save it to the `YOUR_APP/templates` DIR
  - Source PATH: `<YOUR_ENV>/LIB/admin_berry_pro/includes/footer.html`
  - Destination PATH: `YOUR_APP/templates/includes/footer.html`
- Edit the footer (Destination PATH)    

At this point, the default version of the `footer.html` shipped in the library is ignored by Django.

In a similar way, all other files and components can be customized easily.

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
