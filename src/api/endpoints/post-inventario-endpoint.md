# Endpoint: `POST /api/inventario`

Permite crear un nuevo elemento en el inventario.

## Ejemplo de Solicitud
```http
POST /api/inventario
Content-Type: application/json

{
  "nombre": Libro 3,
  "cantidad": 20,
}

Respuesta Exitosa (Código 200 OK)
{
  "id": 3,
  "nombre": Libro 3,
  "cantidad": 20,
}

Respuestas de Errores Posibles

Código 400 Bad Request:
{
  "errno": 400,
  "error": "bad_request",
  "error_description": "Error al procesar la solicitud de creación del nuevo elemento en el inventario."
}

Código 500 Internal Server Error:
{
  "errno": 500,
  "error": "internal_error",
  "error_description": "Ocurrió un problema al crear el nuevo elemento en el inventario."
}