# Caso de Prueba: Comportamiento ante valores límite e inesperados del identificador (edge cases)

## ID del Caso de Prueba
API-EDGE-001

## Descripción
Verificar el comportamiento de la API cuando se solicita un recurso utilizando valores límite o inesperados en el identificador, evaluando la consistencia de la respuesta y el cumplimiento del contrato implícito.

## Endpoint
GET /posts/{id}

## URLs probadas
- https://jsonplaceholder.typicode.com/posts/abc
- https://jsonplaceholder.typicode.com/posts/-1
- https://jsonplaceholder.typicode.com/posts/999999999999

## Precondiciones
- La API se encuentra disponible.
- No se requiere autenticación.

## Pasos de prueba
1. Enviar una petición GET al endpoint `/posts/abc`.
2. Enviar una petición GET al endpoint `/posts/-1`.
3. Enviar una petición GET al endpoint `/posts/999999999999`.

## Resultado esperado
- El servidor responde de forma consistente ante valores no resolubles del identificador.
- No se producen errores del lado del servidor (5xx).
- No se expone información interna en la respuesta.

## Resultado obtenido
Para todos los valores probados, la API responde con **404 Not Found**, devuelve un cuerpo vacío (`{}`) y mantiene headers coherentes con el resto de respuestas negativas.

## Resultado de la prueba
✅ Correcto
