# Proyecto Django: home_about1

Este proyecto es una aplicación web desarrollada con Django que incluye páginas de inicio y "acerca de". A continuación, se detallan las características, estructura, instrucciones de instalación y uso.

---

## Índice
- [Descripción](#descripción)
- [Estructura del Proyecto](#estructura-del-proyecto)
- [Requisitos](#requisitos)
- [Instalación](#instalación)
- [Ejecución](#ejecución)
- [Migraciones](#migraciones)
- [Estructura de Directorios](#estructura-de-directorios)
- [Personalización de Plantillas](#personalización-de-plantillas)
- [Licencia](#licencia)

---

## Descripción
Este proyecto es una base para sitios web con páginas de inicio y "acerca de", utilizando Django como framework principal. Incluye una estructura modular y plantillas HTML listas para personalizar.

## Estructura del Proyecto
```
home_about1/
│   db.sqlite3
│   manage.py
│   requirements.txt
│
├── base_project/
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
│
├── pages/
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── models.py
│   ├── tests.py
│   ├── urls.py
│   ├── views.py
│   └── migrations/
│       └── __init__.py
│
└── templates/
    ├── _base.html
    ├── about.html
    └── home.html
```

## Requisitos
- Python 3.8+
- Django 4.x o superior
- (Opcional) Entorno virtual (recomendado)

## Instalación
1. **Clona el repositorio:**
   ```bash
   git clone <url-del-repositorio>
   cd home_about1
   ```
2. **Crea y activa un entorno virtual:**
   ```bash
   python -m venv .venv
   # En Windows
   .venv\Scripts\activate
   # En Mac/Linux
   source .venv/bin/activate
   ```
3. **Instala las dependencias:**
   ```bash
   pip install -r requirements.txt
   ```

## Ejecución
1. **Aplica migraciones:**
   ```bash
   python manage.py migrate
   ```
2. **Inicia el servidor de desarrollo:**
   ```bash
   python manage.py runserver
   ```
3. Accede a la aplicación en [http://localhost:8000](http://localhost:8000)

## Migraciones
Para crear nuevas migraciones después de modificar modelos:
```bash
python manage.py makemigrations
python manage.py migrate
```

## Estructura de Directorios
- **base_project/**: Configuración principal de Django.
- **pages/**: Aplicación principal con vistas, modelos y rutas.
- **templates/**: Plantillas HTML para las páginas.
- **db.sqlite3**: Base de datos SQLite por defecto.
- **requirements.txt**: Dependencias del proyecto.
- **manage.py**: Script de gestión de Django.

## Personalización de Plantillas
Las plantillas HTML se encuentran en la carpeta `templates/`:
- `_base.html`: Base para heredar en otras plantillas.
- `home.html`: Página de inicio.
- `about.html`: Página "Acerca de".

Puedes modificar estas plantillas para personalizar el diseño y contenido del sitio.

## Licencia
Este proyecto se distribuye bajo la licencia MIT. Puedes usarlo, modificarlo y distribuirlo libremente.

---

> **Desarrollado con ❤️ usando Django.**
