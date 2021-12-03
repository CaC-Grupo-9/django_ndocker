# django_ndocker

Primero necesito prepar mi entorno para correr django.

1- Instalar Python 3+
2- Instalar MySQL/MariaDB
3- (Opcional si no quieren instalar Django en la carpeta de python del sistema)Crear un entorno virtual de Python
4- Corren el comando pip -r install requirements.txt

## Crear mi proyecto de Django corriendo el siguiente comando:

django-admin startproject <REPLACE BY PROJECT NAME> .

## Configurando django

* Corres el initial.sql en la base de datos para asegurar la creacion del schema de la DB.

* modifcar setting.py con lo siguiente:
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'django',
        'USER': 'userdjango',
        'PASSWORD': 'passworddjango',
        'HOST': 'localhost',
        'PORT': 3306,
    }
}


## Ahora puedo crear mi primer App dentro del proyecto de django corriendo el siguiente comando:

python manage.py startapp <REPLACE BY APP NAME>