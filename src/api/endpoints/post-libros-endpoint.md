# Endpoint: `POST /api/libros`

Permite crear un nuevo libro.

## Ejemplo de Solicitud
```http
POST /api/libros
Content-Type: application/json

{
  "titulo": Caperusita,
  "autor": Alexandro,
}

Respuesta Exitosa (Código 200 OK)
{
  "id": 3,
  "titulo": Caperusita,
  "autor": Alexandro,
}

Respuestas de Errores Posibles

Código 400 Bad Request:
{
  "errno": 400,
  "error": "bad_request",
  "error_description": "Error al procesar la solicitud de creación del nuevo libro."
}

Código 500 Internal Server Error:
{
  "errno": 500,
  "error": "internal_error",
  "error_description": "Ocurrió un problema al crear el nuevo libro."
}