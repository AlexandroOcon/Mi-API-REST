# Endpoint: `DELETE /api/inventario/{id}`

Permite eliminar (soft delete) un elemento específico en el inventario.

## Parámetros de URL
- `{id}` (obligatorio): Identificador único del elemento en el inventario que se desea eliminar.

## Ejemplo de Solicitud
```http
DELETE /api/inventario/1

Respuesta Exitosa (Código 200 OK)
{
  "mensaje": "Elemento en el inventario eliminado con éxito"
}

Respuestas de Errores Posibles

Código 404 Not Found:
{
  "errno": 404,
  "error": "not_found",
  "error_description": "No se encontró el elemento en el inventario con el ID proporcionado."
}

Código 500 Internal Server Error:
{
  "errno": 500,
  "error": "internal_error",
  "error_description": "Ocurrió un problema al eliminar el elemento en el inventario."
}
