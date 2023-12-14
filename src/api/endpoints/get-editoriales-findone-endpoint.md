# Endpoint: `GET /api/editoriales/{id}`

Permite obtener información detallada sobre una editorial mediante su identificador único.

## Parámetros de URL
- `{id}` (obligatorio): Identificador único de la editorial que se desea recuperar.

## Ejemplo de Solicitud
```http
GET /api/editoriales/1
Respuesta Exitosa (Código 200 OK)
{
  "id": 1,
  "nombre": "Editorial 1",
  "descripcion": "Descripción de la Editorial 1"
}

Respuestas de Errores Posibles

Código 404 Not Found:
{
  "errno": 404,
  "error": "not_found",
  "error_description": "No se encontró la editorial con el ID proporcionado."
}

Código 500 Internal Server Error:
{
  "errno": 500,
  "error": "internal_error",
  "error_description": "Ocurrió un problema al obtener información detallada de la editorial."
}