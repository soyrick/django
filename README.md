# 🚀 Task List App

## ✨ Sobre el proyecto
Este es un mini proyecto de lista de tareas construido con Django. Incluye una app `tasks` que muestra tareas usando una vista genérica basada en clases y plantillas Django, con estilos estáticos básicos.

## 🧰 Tecnologías usadas
- **Python**
- **Django 6.0.x**
- **SQLite** (base de datos por defecto de Django)
- **Django Templates**
- **HTML5**
- **CSS3**
- **Django Static Files**
- **Git**

## 🚀 Características
- Vista de lista de tareas con `ListView`
- Estructura de app Django modular (`tasks`)
- Plantillas con herencia (`_base.html`)
- Estilos CSS simples en `static/css/base.css`
- Base de datos SQLite local (`db.sqlite3`)

## 📁 Estructura del proyecto
```
/task_list
├── base_project/
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── tasks/
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── models.py
│   ├── tests.py
│   └── views.py
├── templates/
│   └── tasks/
│       ├── _base.html
│       └── tasks_list.html
├── static/
│   └── css/
│       └── base.css
├── db.sqlite3
├── manage.py
└── requirements.txt
```

## 🛠️ Cómo ejecutar el proyecto
1. Clona este repositorio.
2. En la carpeta del proyecto, crea un entorno virtual:
   ```powershell
   python -m venv .venv
   .\.venv\Scripts\activate
   ```
3. Instala las dependencias:
   ```powershell
   python -m pip install -r requirements.txt
   ```
4. Aplica las migraciones:
   ```powershell
   python manage.py migrate
   ```
5. Ejecuta el servidor de desarrollo:
   ```powershell
   python manage.py runserver
   ```
6. Abre `http://127.0.0.1:8000/` en tu navegador.

## 💡 Sugerencias de mejora
- Agregar creación y edición de tareas
- Añadir autenticación de usuarios
- Implementar búsqueda y filtros
- Mejorar el estilo con CSS moderno o un framework como Tailwind

## 📌 Notas
El proyecto usa la configuración estándar de Django con una app `tasks` que renderiza tareas mediante `TaskListView` y una plantilla base compartida.
