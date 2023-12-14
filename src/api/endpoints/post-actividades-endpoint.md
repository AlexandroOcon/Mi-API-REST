# Endpoint: `POST /api/actividades`

Permite crear una nueva actividad.

## Ejemplo de Solicitud
```http
POST /api/actividades
Content-Type: application/json

{
  "nombre": Leer 2,
  "descripcion": Vamos a leer denuevo,
}

Respuesta Exitosa (Código 200 OK)
{
  "id": 2,
  "nombre": Leer 2,
  "descripcion": Vamos a leer denuevo,
}

Respuestas de Errores Posibles
Código 400 Bad Request:
{
  "errno": 400,
  "error": "bad_request",
  "error_description": "Error al procesar la solicitud de creación de la actividad."
}

Código 500 Internal Server Error:
{
  "errno": 500,
  "error": "internal_error",
  "error_description": "Ocurrió un problema al crear la nueva actividad."
}