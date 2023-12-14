# Endpoint: `GET /api/actividades`

Permite recuperar la lista de todas las actividades disponibles.

## Ejemplo de Solicitud
```http
GET /api/actividades

Respuesta Exitosa (Código 200 OK)
[
  {
    "id": 1,
    "nombre": "Leer",
  },
]

Respuestas de Errores Posibles
Código 500 Internal Server Error:
{
  "errno": 500,
  "error": "internal_error",
  "error_description": "Ocurrió un problema al recuperar la lista de actividades."
}