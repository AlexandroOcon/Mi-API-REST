# Endpoint: `PUT /api/editoriales/{id}`

Permite modificar totalmente una editorial existente.

## Parámetros de URL
- `{id}` (obligatorio): Identificador único de la editorial que se desea modificar.

## Ejemplo de Solicitud
```http
PUT /api/editoriales/2
Content-Type: application/json

{
  "nombre": Kevin,
  "descripcion": Ahuevo,
}

Respuesta Exitosa (Código 200 OK)
{
  "id": 2,
  "nombre": Kevin,
  "descripcion": Ahuevo,
}

Respuestas de Errores Posibles

Código 404 Not Found:
{
  "errno": 404,
  "error": "not_found",
  "error_description": "No se encontró la editorial con el ID proporcionado."
}

Código 400 Bad Request:
{
  "errno": 400,
  "error": "bad_request",
  "error_description": "Error al procesar la solicitud de modificación total de la editorial."
}

Código 500 Internal Server Error:
{
  "errno": 500,
  "error": "internal_error",
  "error_description": "Ocurrió un problema al modificar totalmente la editorial."
}