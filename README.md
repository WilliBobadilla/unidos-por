# unidos-por - Readme

Este proyecto esta en su etapa de inicio, permitirá visualizar todos los eventos para recaudaciones de fondos (Polladas, hamburgueseadas, etc).

A la fecha cuenta con dos templates básicos y en desarrollo.

# Sobre el proyecto :clap:

Se trata de un sitio de eventos que sirven para recaudar fondos para una actividad en específica.

Cualquier persona puede registrar su actividad, proporcionando datos como: Fecha y hora, dirección, costo, entre otros.

## Pre-requisitos

[requerimientos.text](https://github.com/gildarey/unidos-por/)

## Instalación en el local :dvd:

1. clonar la repo

```bash
git clone https://github.com/gildarey/unidos-por
```

2. Ingresar a la carpeta del proyecto

```bash
cd unidos-por
```

3. Crear el entorno Virtual

```bash
python3 -m venv env
```

4. Activar el entorno virtual

```bash
source env/bin/activate
```

5. Instalar requerimientos

```bash
pip3 install -r requirements.txt
```

6. Crear un archivo en la raiz del proyecto llamado .env y agregar las siguientes
   variables con sus datos correspondientes

```bash
SECRET_KEY='algunaclavesecretageneradapornostros'
GOOGLE_MAPS_API_KEY='api key de google sacado de la consola de google'

```

7. Crear el archivo local*settings.py en la carpeta \_Proyecto* con el siguiente contenido:

```bash
import os
from settings import BASE_DIR

DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.sqlite3',
        'NAME': os.path.join(BASE_DIR, 'db.sqlite3'),
    }
}

```

8. Correr las migraciones de la db

```bash
python manage.py migrate
```

9. Correr el server local

```bash
python manage.py runserver
```

## Contribuciones :raised_hands:

[Gilda Rey](https://github.com/gildarey/) - Trabajo inicial

## Versiones

## Autores :woman: :man:

[Gilda Rey](https://github.com/gildarey/) - Trabajo inicial

Consulte también la lista de colaboradores que participaron en este proyecto.
