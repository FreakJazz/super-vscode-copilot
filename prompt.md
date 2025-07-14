# 🚀 Proyecto Flask CRUD con Bootstrap y SQLite

Este proyecto está pensado para ser generado automáticamente por GitHub Copilot Chat. Se trata de una aplicación web en **Python Flask** que implementa un **CRUD completo para usuarios**, utilizando **Bootstrap 5** en el frontend y **SQLite** con SQLAlchemy en el backend.

---

## 🧠 Prompt para GitHub Copilot Chat

> Copilot, crea un proyecto Flask con esta estructura y comportamiento:

- App web en **Flask** usando **SQLAlchemy** con **SQLite**
- Un CRUD para **usuarios** con los siguientes campos:
  - `id` (entero, autoincremental, clave primaria)
  - `nombre` (string)
  - `email` (string)
  - `telefono` (string)
- Los archivos deben incluir:
  - `app.py` como archivo principal donde se define `Flask(__name__)`, se configura SQLAlchemy y se ejecuta la app
  - `models.py` con el modelo `User`
  - `templates/` con archivos HTML (`base.html`, `index.html`, `create.html`, `edit.html`)
  - `static/` para CSS o JS si hace falta
  - `requirements.txt` con las dependencias (Flask, Flask-SQLAlchemy)
  - `.gitignore` que excluya `/venv/`, `*.pyc`, `__pycache__/`, y `*.db`
- En `app.py`, usar `with app.app_context(): db.create_all()` para inicializar la DB correctamente.
- Agrega rutas para:
  - `GET /` → listar usuarios
  - `GET /create` → mostrar formulario
  - `POST /create` → crear usuario
  - `GET /edit/<int:id>` → formulario de edición
  - `POST /edit/<int:id>` → actualizar usuario
  - `POST /delete/<int:id>` → eliminar usuario
- Usa **Bootstrap 5** para formularios y botones con buen diseño
- Cada HTML debe extender `base.html` usando Jinja2
- El proyecto debe poder ejecutarse con `python app.py`

---

## 📁 Estructura del proyecto

flask_app/
│
├── app.py
├── models.py
├── requirements.txt
├── templates/
│ ├── base.html
│ ├── index.html # Lista de usuarios
│ ├── create.html # Formulario de nuevo usuario
│ └── edit.html # Formulario de edición
└── 


## 📌 Tecnologías

- Python 3.x
- Flask
- Flask-SQLAlchemy
- Bootstrap 5
- SQLite

---

## 🧪 Cómo ejecutar el proyecto

    ```bash
    # Crear entorno virtual
    python -m venv venv

    # Activar entorno (en Windows)
    venv\Scripts\activate

    # Instalar dependencias
    pip install -r requirements.txt

    # Ejecutar la aplicación
    python app.py

    ```


