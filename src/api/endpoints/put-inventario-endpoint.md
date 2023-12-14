# Endpoint: `PUT /api/inventario/{id}`

Permite modificar totalmente un elemento existente en el inventario.

## Parámetros de URL
- `{id}` (obligatorio): Identificador único del elemento en el inventario que se desea modificar.

## Ejemplo de Solicitud
```http
PUT /api/inventario/2
Content-Type: application/json

{
  "nombre": Libro 2,
  "cantidad": 15,
}

Respuesta Exitosa (Código 200 OK)
{
  "id": 2,
  "nombre": Libro 2,
  "cantidad": 15,
}

Respuestas de Errores Posibles

Código 404 Not Found:
{
  "errno": 404,
  "error": "not_found",
  "error_description": "No se encontró el elemento en el inventario con el ID proporcionado."
}

Código 400 Bad Request:
{
  "errno": 400,
  "error": "bad_request",
  "error_description": "Error al procesar la solicitud de modificación total del elemento en el inventario."
}

Código 500 Internal Server Error:
{
  "errno": 500,
  "error": "internal_error",
  "error_description": "Ocurrió un problema al modificar totalmente el elemento en el inventario."
}