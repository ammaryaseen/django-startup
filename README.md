# Django Organized Startup Project

This project is built to create more organized startup Django project with meaningful backend and applications folders. 

# Project Layout
* The main folder has been renamed to `Backend` folder.
* The applications have been moved to be in one folder which is `Apps` folder.
* `Templates` direcotry has been used as global templates folder.

Project is built with : Django 2.2

# Quick start 
Please ensure that you have installed `Python`, `pip` and `virtualenv`:

* `git clone https://github.com/ammaryaseen/djangostartup.git`
* `cd djangostartup`
* `virtualenv venv`
* `source venv/bin/activate`
* `pip install requirements.txt`

## Adding new application
To add new application to the project:
* Create a new application with the following command:
```
python manage.py startapp NewApplication
```

* Move the new application to `Apps` folder

* Go to `Apps > NewApplication > apps.py` and change `name` value to:
```
name = 'Apps.NewApplication'
```
* Add the new application to the `INSTALLED_APPS` in the `Backend > settings.py`:

```
INSTALLED_APPS = [
    .....

    # Your Applications
    ........
    'Apps.NewApplication.apps.NewApplicationConfig'
    
]
```

* Done!


