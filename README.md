# Proyecto de web playground en Django
Proyecto avanzado en Django, centrado puramente en el backend. Incluye el manejo de la autenticación y el registro de usuarios, creación de secciones internas solo para usuarios identificados, perfiles de usuario y un sistema de mensajería privada.
Basado en el curso [Curso Práctico de Django: Desarrollo Web Backend con Python](udemy.com/course/curso-django-2-practico-desarrollo-web-python-3/).

Conceptos utilizados:
- Qué son y cómo utilizar las CBV (Class Based Views).
-	Generar vistas CRUD con formularios utilizando CBV.
-	Formularios de modelos, mixins y decoradores.
-	Sistema de autenticación de usuarios (login y logout).
-	Sistema de registro de usuarios básico con CBV.
-	Extensión del formulario de registro con un email obligatorio.
-	Funcionalidad de restaurar la contraseña a través de email.
-	Sistema de perfiles de usuarios con avatar, biografía y enlace.
-	Funcionalidad de editar los campos email y contraseña.
-	Introducción a las señales y a las pruebas unitarias.
-	Optimización del espacio ocupado por el avatar.
-	Creación de una App para manejar perfiles públicos (práctica).
-	Funcionalidad de paginar resultados fácilmente en ListView.
-	Creación de una App de mensajería privada.
-	Introducción al TDD desarrollando las funciones básicas.
-	Envío de mensajes asíncronos utilizando Javascript


## Instalación con Pipenv
- Instalación de paquetes
```bash
pipenv install django django-ckeditor-5 Pillow pylint pylint-django pylint-celery
```

- Creación del proyecto
```bash
pipenv run django-admin startproject django-webplayground
```

## Ejecución del proyecto
- Ejecución directa
```bash
pipenv run python django-webplayground/manage.py runserver
```

- Añadiendo script en Pipfile
```bash
[scripts]
webplayground = "python django-playground/manage.py runserver"
```

La ejecución se realiza con:
```bash
pipenv run webplayground
```

## Creación de aplicaciones
- Creación de una aplicación
```bash
python manage.py startapp core
```

## Creación de modelos
- Creación de una aplicación
```bash
python manage.py startapp services
```

- Ejecución de la migración
```bash
python manage.py makemigrations
```

- Aplicación de la migración a la base de datos
```bash
python manage.py migrate
```

- Creación del superusuario
```bash
python manage.py createsuperuser
```
