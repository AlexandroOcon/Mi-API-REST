# Endpoint: `GET /api/libros`

Permite recuperar la lista de todos los libros disponibles.

## Ejemplo de Solicitud
```http
GET /api/libros
Respuesta Exitosa (Código 200 OK)
[
  {
    "id": 1,
    "titulo": Pesadilla,
    "autor": Kevin Ocon,
  },
  {
    "id": 2,
    "titulo": "Libro 2",
    "autor": "Autor 2",
  }
]

Respuesta Exitosa para GET /api/libros/{id} (Código 200 OK)
{
  "id": 1,
  "titulo": Pesadilla,
  "autor": Kevin Ocon,
}

Respuestas de Errores Posibles

Código 500 Internal Server Error:
{
  "errno": 500,
  "error": "internal_error",
  "error_description": "Ocurrió un problema al recuperar la lista de libros o al obtener información detallada del libro."
}