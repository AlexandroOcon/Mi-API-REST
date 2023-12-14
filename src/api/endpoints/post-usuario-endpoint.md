# Endpoint: `POST /api/usuarios/{id}`

Permite obtener información detallada sobre un post mediante su identificador único.

## Parámetros de URL
- `{id}` (obligatorio): Identificador único del post que se desea recuperar.

## Ejemplo de Solicitud
POST /api/usuarios
Content-Type: application/json

{
  "nombre": Noe,
  "email": nocon@gmail.com,
}

Respuesta Exitosa (Código 200 OK)
{
  "id": 4,
  "nombre": Noe,
  "email": nocon@gmail.com,
}

Respuestas de Errores Posibles
Código 400 Bad Request:
{
  "errno": 400,
  "error": "bad_request",
  "error_description": "Error al procesar la solicitud de creación de usuario."
}

Código 500 Internal Server Error:
{
  "errno": 500,
  "error": "internal_error",
  "error_description": "Ocurrió un problema al crear un nuevo usuario."
}