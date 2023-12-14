# Endpoint: `PUT /api/usuarios/{id}`

Permite obtener información detallada sobre un post mediante su identificador único.

## Parámetros de URL
- `{id}` (obligatorio): Identificador único del post que se desea recuperar.

## Ejemplo de Solicitud
PUT /api/usuarios/2
Content-Type: application/json

{
  "nombre": Norman Ocon,
  "email": nococon@gmail.com,
}

Respuesta Exitosa (Código 200 OK)
{
  "id": 2,
  "nombre": Norman Ocon,
  "email": nococon@gmail.com,
}

Respuestas de Errores Posibles
Código 404 Not Found:
{
  "errno": 404,
  "error": "not_found",
  "error_description": "No se encontró el usuario con el ID proporcionado."
}
Código 400 Bad Request