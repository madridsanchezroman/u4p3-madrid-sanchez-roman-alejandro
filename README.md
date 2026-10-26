# U4S8 — Madrid Sánchez Román Alejandro

## Demo en vivo (producción)

https://u4s8-madrid-sanchez-roman-alejandro.onrender.com

**Estado:** Pendiente de desplegar en Render durante la Semana 8.

## Qué hace este proyecto

Este proyecto es una aplicación web desarrollada con Django que permite administrar un catálogo de servicios. Los usuarios pueden registrarse, iniciar sesión y gestionar sus propios servicios mediante operaciones CRUD (crear, consultar, editar y eliminar).

Cada servicio contiene un título, descripción, precio y categoría. La información se almacena en una base de datos MySQL alojada en Aiven.

El sistema utiliza autenticación para proteger las operaciones y permitir que cada usuario administre únicamente sus propios servicios.

## Stack técnico

- Python y Django
- MySQL (Aiven)
- HTML5 y Tailwind CSS
- Render (despliegue en producción)
- Git y GitHub

## Cómo se prueba el aislamiento por usuario

1. Registrar dos usuarios diferentes.
2. Iniciar sesión con el primer usuario.
3. Crear uno o varios servicios.
4. Cerrar sesión.
5. Iniciar sesión con el segundo usuario.
6. Verificar que no aparecen los servicios del primer usuario.
7. Comprobar que cada usuario únicamente puede consultar, modificar y eliminar sus propios servicios.

El aislamiento se implementa relacionando cada servicio con su propietario y filtrando las consultas mediante el usuario autenticado.

## Historial de unidades

- **Unidad 1:** Creación del portafolio personal utilizando HTML5 y Tailwind CSS.
- **Unidad 2:** Desarrollo del proyecto Django, conexión con MySQL en Aiven y despliegue en Render.
- **Unidad 3:** Implementación de operaciones CRUD con ModelForms, registro de usuarios, autenticación y sesiones.
- **Unidad 4:** Revisión final del sistema, seguridad, respaldo de datos, despliegue definitivo y defensa oral.

## Cómo ejecutar el proyecto localmente

1. Crear y activar un entorno virtual.
2. Instalar dependencias mediante `pip install -r requirements.txt`.
3. Configurar las variables de entorno en un archivo `.env`.
4. Ejecutar `python manage.py migrate`.
5. Iniciar el servidor mediante `python manage.py runserver`.

## Repositorio

https://github.com/madridsanchezroman/u4s8-madrid-sanchez-roman-alejandro

**Nota:** El repositorio y el servicio de Render de la Semana 8 se crearán en los siguientes pasos.