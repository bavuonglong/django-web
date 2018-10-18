# Django Web Application

This is a full functionality web application using Django framework

### Run

To start project up, use

```
python manage.py runserver
```

To create an app inside the project, use

```
python manage startapp blog
```

For the first time running the project, we need to create admin user, to do that, we need

```
python manage.py migrate
python manage.py createsuperuser
```

After creating database models, we need to:
```
python manage.py makemigrations
```
Then it's going to generate migration script under migrations folder

To view what SQL statement actually run behind the scence, we can
```
python manage.py sqlmigrate blog 0001
```
with `blog` is application name, 0001 is id of migration script

To actually run migration script, we have to:
```
python manage.py migrate
```

To access shell command line:
```
python manage.py shell
```

Create users app
```
python manage.py startapp users
```
