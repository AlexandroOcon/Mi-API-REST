# Endpoint: `POST /api/editoriales`

Permite crear una nueva editorial.

## Ejemplo de Solicitud
```http
POST /api/editoriales
Content-Type: application/json

{
  "nombre": San Juan,
  "descripcion": Las mejores de colima,
}

Respuesta Exitosa (Código 200 OK)
{
  "id": 2,
  "nombre": "Nueva Editorial",
  "descripcion": "Descripción de la Nueva Editorial"
}

Respuestas de Errores Posibles

Código 400 Bad Request:
{
  "errno": 400,
  "error": "bad_request",
  "error_description": "Error al procesar la solicitud de creación de la nueva editorial."
}

Código 500 Internal Server Error:
{
  "errno": 500,
  "error": "internal_error",
  "error_description": "Ocurrió un problema al crear la nueva editorial."
}