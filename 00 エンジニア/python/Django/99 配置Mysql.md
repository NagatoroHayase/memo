* pip install mysqlclient
* cd settings.py
```PY
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME'  : 'mysql',
        'USER'  : 'root',
        'PASSWORD' : 'root',
        'HOST'  : 'localhost',
        'PORT'  : '3306',
    }
}
```