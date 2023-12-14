# Endpoint: `GET /api/libros/{id}`

Permite obtener información detallada sobre un libro mediante su identificador único.

## Parámetros de URL
- `{id}` (obligatorio): Identificador único del libro que se desea recuperar.

## Ejemplo de Solicitud
```http
GET /api/libros/1
Respuesta Exitosa (Código 200 OK)
{
  "id": 1,
  "titulo": Pesadilla,
  "autor": Kevin Ocon,
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
  "error_description": "Ocurrió un problema al obtener información detallada del libro."
}