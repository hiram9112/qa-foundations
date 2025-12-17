# Bug: El sistema permite crear un gasto con cantidad 0

## Entorno
- Aplicación: Gestor de Economía Familiar
- Entorno: Local
- Navegador: Chrome
- Sistema operativo: Linux

## Precondiciones
- El usuario está autenticado en la aplicación.
- El usuario se encuentra en la pantalla de creación de gastos.

## Pasos para reproducir
1. Introducir una cantidad igual a 0.
2. Seleccionar una categoría existente.
3. Introducir una fecha válida.
4. Introducir una descripción opcional.
5. Pulsar el botón de guardar.

## Resultado actual
- El sistema permite guardar el gasto con una cantidad igual a 0.
- El gasto se registra y aparece en el listado de gastos.
- Los totales se actualizan incluyendo el gasto con cantidad 0.

## Resultado esperado
- El sistema no debe permitir guardar un gasto con cantidad igual a 0.
- Se debe mostrar un mensaje de error indicando que la cantidad no es válida.
- El gasto no debe registrarse ni afectar a los totales.

## Severidad
Media

## Prioridad
Alta
