# trydjango
Setting up Django server for the first time. These should be the instructions to clone the project.

1. git clone https://github.com/harryyy27/trydjango
2. virtualenv -p python 3
3. cd into root directory
4. source bin/activate
5. pip install -r requirements.txt
6. cd into src
7. set up config.py in src directory and type in a SECRET_KEY1 variable. Set it to any string
8. set up a postgres DB in settings.py
  ```
  DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql_psycopg2',
        'NAME': 'db_name',
        'USER': 'name',
        'PASSWORD': '',
        'HOST': 'localhost',
        'PORT': '',
    }
}
```
9. python manage.py migrate
10. python manage.py createsuperuser
11. python manage.py runserver
12. voila!
