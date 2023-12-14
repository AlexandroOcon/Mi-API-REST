# Endpoint: `GET /api/inventario/{id}`

Permite obtener información detallada sobre un elemento en el inventario mediante su identificador único.

## Parámetros de URL
- `{id}` (obligatorio): Identificador único del elemento en el inventario que se desea recuperar.

## Ejemplo de Solicitud
```http
GET /api/inventario/1

Respuesta Exitosa (Código 200 OK)
{
  "id": 1,
  "nombre": "Producto 1",
  "cantidad": 10,
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
  "error_description": "Ocurrió un problema al obtener información detallada del elemento en el inventario."
}