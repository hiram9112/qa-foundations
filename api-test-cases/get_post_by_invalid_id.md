# Caso de Prueba: Obtener post con ID inválido (escenario negativo)

## ID del Caso de Prueba
API-GET-002


## Descripción
Verificar que la API gestiona correctamente una solicitud GET cuando se proporciona un identificador de post que no existe, devolviendo el código de estado adecuado y sin errores inesperados.

## Endpoint
GET /posts/{id}

## URL completa
https://jsonplaceholder.typicode.com/posts/99999

## Precondiciones
- La API se encuentra disponible.
- No se requiere autenticación.

## Pasos de prueba
1. Enviar una petición GET al endpoint `/posts/99999`.

## Resultado esperado
- El servidor responde con el código de estado **404 Not Found**.
- La respuesta no contiene datos del recurso solicitado.
- No se produce ningún error interno  del  servidor.

## Resultado obtenido
El servidor responde con **404 Not Found** y no devuelve contenido en el cuerpo de la respuesta.

## Resultado de la prueba
✅ **Correcto**
