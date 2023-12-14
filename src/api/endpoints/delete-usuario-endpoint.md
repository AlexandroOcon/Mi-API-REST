# Endpoint: `DELETE /api/usuarios/{id}`

Permite eliminar (soft delete) un usuario específico.

## Parámetros de URL
- `{id}` (obligatorio): Identificador único del usuario que se desea eliminar.

## Ejemplo de Solicitud
```http DELETE /api/usuarios/2

Respuesta Exitosa (Código 200 OK)
{
  "mensaje": "Usuario eliminado con éxito"
}

Respuestas de Errores Posibles

Código 404 Not Found:
{
  "errno": 404,
  "error": "not_found",
  "error_description": "No se encontró el usuario con el ID proporcionado."
}

Código 500 Internal Server Error:
{
  "errno": 500,
  "error": "internal_error",
  "error_description": "Ocurrió un problema al eliminar el usuario."
}