# Proyecto Educativo en Django

Este es un proyecto educativo creado con Django, diseñado para gestionar una lista de estudiantes con sus datos personales. Incluye funcionalidades básicas como visualización de lista de estudiantes, detalle individual y uso de plantillas con herencia.

## Tecnologías Utilizadas

- **Django**: Framework principal para el desarrollo del backend.
- **HTML/CSS**: Para la estructura y estilos del frontend.
- **JavaScript**: Para interactividad básica.
- **SQLite**: Base de datos predeterminada.

---

## Instalación y Configuración

### Requisitos Previos
- Python 3.8 o superior
- pip (Gestor de paquetes de Python)
- Entorno virtual (opcional pero recomendado)

### Pasos para la Configuración
1. Clonar el repositorio:
   ```bash
   git clone <URL_DEL_REPOSITORIO>
   cd proyecto_educativo
   ```

2. Crear un entorno virtual:
   ```bash
   python -m venv venv
   source venv/bin/activate  # En Windows: venv\Scripts\activate
   ```

3. Instalar las dependencias:
   ```bash
   pip install -r requirements.txt
   ```

4. Realizar las migraciones de la base de datos:
   ```bash
   python manage.py migrate
   ```

5. Ejecutar el servidor de desarrollo:
   ```bash
   python manage.py runserver
   ```

6. Accede a la aplicación en [http://127.0.0.1:8000/](http://127.0.0.1:8000/).

---

## Estructura del Proyecto

```
proyecto_educativo/
├── principal/
│   ├── migrations/
│   ├── templates/
│   │   ├── base.html
│   │   ├── home.html
│   │   └── detalle.html
│   ├── static/
│   │   ├── css/
│   │   │   └── styles.css
│   │   ├── js/
│   │   │   └── scripts.js
│   │   └── images/
│   │       └── logo.webp
│   ├── models.py
│   ├── views.py
│   ├── urls.py
├── proyecto_educativo/
│   ├── settings.py
│   ├── urls.py
│   ├── wsgi.py
```

---

## Funcionalidades Principales

1. **Gestión de Estudiantes**:
   - Modelo `Estudiante` que incluye: nombre, apellido, correo, edad y fecha de registro.

2. **Plantillas con Herencia**:
   - `base.html`: Plantilla base con bloques para título y contenido.
   - `home.html`: Lista de estudiantes.
   - `detalle.html`: Detalle de un estudiante seleccionado.

3. **Estáticos**:
   - **CSS**: Diseño básico para la presentación de la interfaz.
   - **JavaScript**: Funcionalidades simples, como alertas.

---

## Archivos Clave

### `settings.py`
Incluye la configuración para plantillas, archivos estáticos y base de datos.

### `urls.py`
Define las rutas para el proyecto y la aplicación principal.

### `models.py`
Modelo `Estudiante` para representar los datos en la base de datos.

### `views.py`
Controladores para gestionar las vistas de la lista y detalles de estudiantes.

### `templates/`
Contiene las plantillas base, de lista y detalle.

### `static/`
Archivos CSS, JavaScript e imágenes utilizados en el frontend.

---

## Contribución

Si deseas contribuir a este proyecto:
1. Haz un fork del repositorio.
2. Crea una rama para tu funcionalidad (`git checkout -b nueva-funcionalidad`).
3. Realiza un pull request.

---

## Licencia

Este proyecto está bajo la licencia MIT. Consulta el archivo `LICENSE` para más detalles.
