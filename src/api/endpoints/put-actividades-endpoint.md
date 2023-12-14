# Endpoint: `PUT /api/actividades/{id}`

Permite modificar totalmente una actividad existente.

## Parámetros de URL
- `{id}` (obligatorio): Identificador único de la actividad que se desea modificar.

## Ejemplo de Solicitud
```http
PUT /api/actividades/2
Content-Type: application/json

{
  "nombre": Comer,
  "descripcion": Vamos a comer,
}

Respuesta Exitosa (Código 200 OK)
{
  "id": 3,
  "nombre": Comer,
  "descripcion": Vamos a comer,
}

Respuestas de Errores Posibles

Código 404 Not Found:
{
  "errno": 404,
  "error": "not_found",
  "error_description": "No se encontró la actividad con el ID proporcionado."
}

Código 400 Bad Request:
{
  "errno": 400,
  "error": "bad_request",
  "error_description": "Error al procesar la solicitud de modificación total de la actividad."
}

Código 500 Internal Server Error:
{
  "errno": 500,
  "error": "internal_error",
  "error_description": "Ocurrió un problema al modificar totalmente la actividad."
}