# Caso de Prueba: Validación de headers de la respuesta del recurso post

## ID del Caso de Prueba
API-HEADERS-001

## Descripción
Verificar que la API devuelve los headers correctos al solicitar un recurso existente, garantizando que el cliente pueda interpretar correctamente el contenido de la respuesta.

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
- El header `Content-Type` está presente.
- El valor del header `Content-Type` es coherente con el formato del cuerpo de la respuesta (**application/json**).
- No se incluyen headers que indiquen errores del servidor.

## Resultado obtenido
La API responde con **200 OK** y devuelve el header `Content-Type: application/json; charset=utf-8`, coherente con el cuerpo de la respuesta en formato JSON. No se observan headers de error.

## Resultado de la prueba
✅ Correcto
