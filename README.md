# API Formulario de Contacto

Esta es la API para la gestión de formularios de contacto en el portfolio de Vanessa Fernandez.

## Descripción

La API permite crear, obtener, actualizar y eliminar contactos. Está diseñada para integrarse con el  y el backend del portfolio, proporcionando un punto de contacto para los visitantes.

## Endpoints

### Crear un contacto

- **POST /contacts**
  - Crea un nuevo contacto.
  - Requiere un cuerpo JSON con los campos: `name`, `phone`, `email`, `message`.

### Obtener todos los contactos

- **GET /contacts**
  - Obtiene una lista de todos los contactos.
  - Soporta paginación con los parámetros: `page`, `pageSize`.

### Obtener un contacto por ID

- **GET /contacts/{id}**
  - Obtiene los detalles de un contacto específico por ID.

### Actualizar parcialmente un contacto

- **PATCH /contacts/{id}**
  - Actualiza los campos `name` y `phone` de un contacto específico por ID.

### Eliminar un contacto

- **DELETE /contacts/{id}**
  - Elimina un contacto específico por ID.

## Seguridad

Esta API usa autenticación con API Key y Bearer Token. Incluye la clave de autenticación en los encabezados de la solicitud:

```http
Authorization: Bearer YOUR_TOKEN
Authorization: API_KEY

## Pruebas con Swagger

Puedes probar y explorar la API usando Swagger UI.Para levantar el entorno de Swagger UI localmente, utiliza Docker Compose con el
archivo 'docker-compose.yml' incluido en el proyecto.

## Pasos para levantar Swagger UI con Docker Compose

1. **Asegurate de tener Docker y Docker Compose intalados en tu máquina.
2. **En la raíz del proyecto ejecuta el comando  docker-compose up
3. **Abre tu navegador web y visita http://localhost:8080 para acceder a la documentación interactiva de Swagger.



### Notas Adicionales

1. **Enlace al Swagger UI**: El enlace proporcionado (`http://localhost:8080`) es para el Swagger UI levantado localmente con Docker Compose. Esto permite a los usuarios acceder a la documentación y probar la API de manera interactiva.


