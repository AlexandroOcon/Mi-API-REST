# Endpoint: `GET /api/usuarios/{id}`

Permite obtener información detallada sobre un post mediante su identificador único.

## Parámetros de URL
- `{id}` (obligatorio): Identificador único del post que se desea recuperar.

## Ejemplo de Solicitud
GET /api/posts/1

Respuesta Exitosa (Código 200 OK)

{
  "data": {
    "title": "Título del Post",
    "content": "Contenido del Post"
  }
}

Respuestas de Errores Posibles

Código 404 Not Found:
{
  "errno": 404,
  "error": "not_found",
  "error_description": "No se encontró el post con el ID {id}."
}

Código 500 Internal Server Error:
{
  "errno": 500,
  "error": "internal_error",
  "error_description": "Ocurrió un problema para procesar la solicitud"
}
