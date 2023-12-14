# Endpoint: `DELETE /api/actividades/{id}`

Permite eliminar (soft delete) una actividad específica.

## Parámetros de URL
- `{id}` (obligatorio): Identificador único de la actividad que se desea eliminar.

## Ejemplo de Solicitud
```http
DELETE /api/actividades/1

Respuesta Exitosa (Código 200 OK)
{
  "mensaje": "Actividad eliminada con éxito"
}

Respuestas de Errores Posibles

Código 404 Not Found:
{
  "errno": 404,
  "error": "not_found",
  "error_description": "No se encontró la actividad con el ID proporcionado."
}

Código 500 Internal Server Error:
{
  "errno": 500,
  "error": "internal_error",
  "error_description": "Ocurrió un problema al eliminar la actividad."
}