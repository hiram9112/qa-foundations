# Caso de Prueba: Validación de estructura del recurso post

## ID del Caso de Prueba
API-SCHEMA-001

## Descripción
Verificar que la API devuelve un recurso post con la estructura esperada, incluyendo los campos obligatorios y sus tipos de datos correctos.

## Endpoint
GET /posts/{id}

## URL completa
https://jsonplaceholder.typicode.com/posts/1

## Precondiciones
- La API se encuentra disponible.
- No se requiere autenticación.

## Pasos de prueba
1. Enviar una petición GET al endpoint `/posts/1`.

## Resultado esperado
- El servidor responde con código de estado **200 OK**.
- La respuesta se devuelve en formato **JSON**.
- El cuerpo de la respuesta contiene los siguientes campos obligatorios:
  - `userId` (number)
  - `id` (number)
  - `title` (string)
  - `body` (string)
- No se incluyen campos inesperados en la respuesta.

## Resultado obtenido
La API responde con **200 OK** y devuelve un objeto JSON que contiene los campos `userId`, `id`, `title` y `body`, todos con el tipo de dato esperado.

## Resultado de la prueba
✅ Correcto
