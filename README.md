# Flexy Lite Django

Open-Source **Django Dashboard** coded with basic modules, database, ORM and deployment scripts on top of Flexy Bootstrap Lite, a modern Bootstrap dashboard design. [WrapPixel](https://appseed.us/agency/wrappixel)'s **Flexy Bootstrap Lite** is one of the best Bootstrap templates for admin dashboards and control admin panels. This powerful and competent Bootstrap 4 admin template is based on HTML and is built with the CSS framework. 

- 👉 [Django Flexy Lite](#) - product page (soon)
- 👉 [Django Flexy Lite](https://django-flexy-bootstrap.appseed-srv1.com) - LIVE deployment

<br />

> Built with [Flexy Lite Generator](https://appseed.us/generator/flexy-bootstrap/)

- Timestamp: `2022-06-06 18:52`
- Build ID: `0a18bd37-68d9-4f5b-9b6f-541443b274c2`
- **Free [Support](https://appseed.us/support/)** (registered users) via `Email` and `Discord`

<br />

> Features

- `Up-to-date dependencies`
- Database: `mysql`
- UI-Ready app, Django Native ORM
- `Session-Based authentication`, Forms validation

<br />

![Flexy Bootstrap Lite - Starter generated by AppSeed.](https://user-images.githubusercontent.com/51070104/172047573-c39829f2-5496-47f9-ac79-06e246626cae.png)

<br />




## ✨ Set up the MySql Database

**Note:** Make sure your Mysql server is properly installed and accessible. 

> **Step 1** - Create the MySql Database to be used by the app

- `Create a new MySql` database
- `Create a new user` and assign full privilegies (read/write)

<br />

> **Step 2** - Edit the `.env` to match your MySql DB credentials. Make sure `DB_ENGINE` is set to `mysql`.

- `DB_ENGINE`  : `mysql` 
- `DB_NAME`    : default value = `appseed_db`
- `DB_HOST`    : default value = `localhost`
- `DB_PORT`    : default value = `3306`
- `DB_USERNAME`: default value = `appseed_db_usr`
- `DB_PASS`    : default value = `pass`

<br />

Here is a sample:  

```txt
# .env sample

DEBUG=False                   # False enables the MySql Persistence

DB_ENGINE=mysql               # Database Driver
DB_NAME=appseed_flask         # Database Name
DB_USERNAME=appseed_flask_usr # Database User
DB_PASS=STRONG_PASS_HERE      # Password 
DB_HOST=localhost             # Database HOST, default is localhost 
DB_PORT=3306                  # MySql port, default = 3306 
```

<br />


## ✨ How to use it

> Download the code 

```bash
$ # Get the code
$ git clone https://github.com/appseed-projects/0a18bd37-68d9-4f5b-9b6f-541443b274c2.git
$ cd 0a18bd37-68d9-4f5b-9b6f-541443b274c2
```

<br />

### 👉 Set Up for `Unix`, `MacOS` 

> Install modules via `VENV`  

```bash
$ virtualenv env
$ source env/bin/activate
$ pip3 install -r requirements.txt
```

<br />

> Set Up Database

```bash
$ python manage.py makemigrations
$ python manage.py migrate
```

<br />

> Start the app

```bash
$ python manage.py runserver
```

At this point, the app runs at `http://127.0.0.1:8000/`. 

<br />

### 👉 Set Up for `Windows` 

> Install modules via `VENV` (windows) 

```
$ virtualenv env
$ .\env\Scripts\activate
$ pip3 install -r requirements.txt
```

<br />

> Set Up Database

```bash
$ python manage.py makemigrations
$ python manage.py migrate
```

<br />

> Start the app

```bash
$ python manage.py runserver
```

At this point, the app runs at `http://127.0.0.1:8000/`. 

<br />

## ✨ Create Users

By default, the app redirects guest users to authenticate. In order to access the private pages, follow this set up: 

- Start the app via `flask run`
- Access the `registration` page and create a new user:
  - `http://127.0.0.1:8000/register/`
- Access the `sign in` page and authenticate
  - `http://127.0.0.1:8000/login/`

<br />

## ✨ Code-base structure

The project is coded using a simple and intuitive structure presented below:

```bash
< PROJECT ROOT >
   |
   |-- core/                               # Implements app configuration
   |    |-- settings.py                    # Defines Global Settings
   |    |-- wsgi.py                        # Start the app in production
   |    |-- urls.py                        # Define URLs served by all apps/nodes
   |
   |-- apps/
   |    |
   |    |-- home/                          # A simple app that serve HTML files
   |    |    |-- views.py                  # Serve HTML pages for authenticated users
   |    |    |-- urls.py                   # Define some super simple routes  
   |    |
   |    |-- authentication/                # Handles auth routes (login and register)
   |    |    |-- urls.py                   # Define authentication routes  
   |    |    |-- views.py                  # Handles login and registration  
   |    |    |-- forms.py                  # Define auth forms (login and register) 
   |    |
   |    |-- static/
   |    |    |-- <css, JS, images>         # CSS files, Javascripts files
   |    |
   |    |-- templates/                     # Templates used to render pages
   |         |-- includes/                 # HTML chunks and components
   |         |    |-- navigation.html      # Top menu component
   |         |    |-- sidebar.html         # Sidebar component
   |         |    |-- footer.html          # App Footer
   |         |    |-- scripts.html         # Scripts common to all pages
   |         |
   |         |-- layouts/                   # Master pages
   |         |    |-- base-fullscreen.html  # Used by Authentication pages
   |         |    |-- base.html             # Used by common pages
   |         |
   |         |-- accounts/                  # Authentication pages
   |         |    |-- login.html            # Login page
   |         |    |-- register.html         # Register page
   |         |
   |         |-- home/                      # UI Kit Pages
   |              |-- index.html            # Index page
   |              |-- 404-page.html         # 404 page
   |              |-- *.html                # All other pages
   |
   |-- requirements.txt                     # Development modules - SQLite storage
   |
   |-- .env                                 # Inject Configuration via Environment
   |-- manage.py                            # Start the app - Django default start script
   |
   |-- ************************************************************************
```

<br />



## ✨ PRO Version

> For more components, pages and priority on support, feel free to take a look at this amazing starter:

MaterialPRO Dashboard is a premium Bootstrap Design now available for download in Django. Made of hundred of elements, designed blocks, and fully coded pages, Material Dashboard PRO is ready to help you create stunning websites and web apps.

- 👉 [WPX MaterialPro Django](https://appseed.us/product/material-wpx-pro/django/) - Product Page
- 👉 [WPX MaterialPro Django](https://django-material-wpx-pro.appseed-srv1.com/) - LIVE Demo

<br >

![MaterialPRO - Premium starter generated by AppSeed.](https://user-images.githubusercontent.com/51070104/172018257-c203a47a-3103-4a66-8324-f11c6aadef14.png)

<br />

---
Flexy Lite Django - Open-source starter generated by **[AppSeed Generator](https://appseed.us/generator/)**.
