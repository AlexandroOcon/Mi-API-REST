# Endpoint: `GET /api/inventario`

Permite recuperar la lista de todos los elementos en el inventario disponibles.

## Ejemplo de Solicitud
```http
GET /api/inventario

Respuesta Exitosa (Código 200 OK)
[
  {
    "id": 1,
    "nombre": "Producto 1",
    "cantidad": 10,
  },
  {
    "id": 2,
    "nombre": "Producto 2",
    "cantidad": 5,
  }
]

Respuesta Exitosa para GET /api/inventario/{id} (Código 200 OK)
{
  "id": 1,
  "nombre": "Producto 1",
  "cantidad": 10,
  // Otros campos del elemento en el inventario
}

Respuestas de Errores Posibles

Código 500 Internal Server Error:
{
  "errno": 500,
  "error": "internal_error",
  "error_description": "Ocurrió un problema al recuperar la lista del inventario o al obtener información detallada de un elemento en el inventario."
}