# Django 
---------------------------------------------------------------------------
[Ref Link](https://docs.djangoproject.com/en/1.10/intro/tutorial02/)
### Show Python Version

      python --version

### Checking Django version

- Import django and show version

      import django
      django.VERSION
      django-admin --version


### Create django project 
- Create a project names `mycoolproject`

      django-admin.py startproject mycoolproject

### Run project
- Find the location of `manage.py` and open termanl on that location and run:

      python manage.py runserver

### Add module
- create a new app names `users`; after this command you need to update `INSTALLED_APPS` in `settings.py` file, `urlpatters` in `urls.py`

      python manage.py startapp users

### Models Migration
- make migration files; e.g. here `users` is the name of model
  
      python manage.py makemigrations users

- show migration sql

      python manage.py sqlmigrate users 0001

- apply database migration
  
      python manage.py migrate

### Create a django user
    
      python manage.py createsuperuser

### Load init Model data
- Load initial data from a file names `initdata_fixture.json` to your application database

      python manage.py loaddata initdata_fixture.json

### Dump Model data
- Dump users data to a json file

      python manage.py dumpdata users  > users_initdata_fixture.json

### Add Model to Admin panel
- update `admin.py` by adding line like: `admin.site.register(User)`; here `User` is the model name

### django restframework 

[Ref Link](http://www.django-rest-framework.org/)

- Install djangorestframework 

      pip install djangorestframework

- Markdown support for the browsable API.
    
      pip install markdown       

- Filtering support
    
      pip install django-filter  
    
    
