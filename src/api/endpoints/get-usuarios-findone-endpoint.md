# Endpoint: `GET /api/usuarios/{id}`

Permite obtener información detallada sobre un post mediante su identificador único.

## Parámetros de URL
- `{id}` (obligatorio): Identificador único del post que se desea recuperar.

## Ejemplo de Solicitud
GET /api/usuarios/:id

Respuesta Exitosa (Código 200 OK)

{
  "id": 1,
  "nombre": "Kevin Alexandro Ocon Zaragoza",
  "email": "kevin_ocon@hotmail.com"
}

Respuestas de Errores Posibles

Código 404 Not Found:
{
  "errno": 404,
  "error": "not_found",
  "error_description": "No se encontró el usuario con los criterios proporcionados."
}

Código 500 Internal Server Error:
{
  "errno": 500,
  "error": "internal_error",
  "error_description": "Ocurrió un problema al encontrar el usuario."
}