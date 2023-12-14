# Endpoint: `PUT /api/libros/{id}`

Permite modificar totalmente un libro existente.

## Parámetros de URL
- `{id}` (obligatorio): Identificador único del libro que se desea modificar.

## Ejemplo de Solicitud
```http
PUT /api/libros/2
Content-Type: application/json

{
  "titulo": La noche,
  "autor": Kevin Ocon,
}

Respuesta Exitosa (Código 200 OK)
{
  "id": 2,
  "titulo": La noche,
  "autor": Kevin Ocon,
}

Respuestas de Errores Posibles
Código 404 Not Found:
{
  "errno": 404,
  "error": "not_found",
  "error_description": "No se encontró el libro con el ID proporcionado."
}

Código 400 Bad Request:
{
  "errno": 400,
  "error": "bad_request",
  "error_description": "Error al procesar la solicitud de modificación total del libro."
}

Código 500 Internal Server Error:
{
  "errno": 500,
  "error": "internal_error",
  "error_description": "Ocurrió un problema al modificar totalmente el libro."
}