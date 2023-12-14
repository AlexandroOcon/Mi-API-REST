# Endpoint: `DELETE /api/libros/{id}`

Permite eliminar (soft delete) un libro específico.

## Parámetros de URL
- `{id}` (obligatorio): Identificador único del libro que se desea eliminar.

## Ejemplo de Solicitud
```http
DELETE /api/libros/1

Respuesta Exitosa (Código 200 OK)
{
  "mensaje": "Libro eliminado con éxito"
}

Respuestas de Errores Posibles

Código 404 Not Found:
{
  "errno": 404,
  "error": "not_found",
  "error_description": "No se encontró el libro con el ID proporcionado."
}

Código 500 Internal Server Error:
{
  "errno": 500,
  "error": "internal_error",
  "error_description": "Ocurrió un problema al eliminar el libro."
}