# Caso de Prueba: Obtener post con ID válido (escenario positivo)

## ID del Caso de Prueba
API-GET-001

## Descripción
Verificar que la API devuelve correctamente un recurso existente cuando se solicita mediante un identificador válido.

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
- El cuerpo de la respuesta contiene los campos esperados del recurso.
- El campo `id` tiene el valor **1**.

## Resultado obtenido
El servidor responde con **200 OK** y devuelve un objeto JSON con los campos `userId`, `id`, `title` y `body`.

## Resultado de la prueba
✅ Correcto
