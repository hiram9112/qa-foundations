# Caso de prueba: Crear gasto válido

## ID
TC-EXP-001

## Funcionalidad
Creación de un gasto

## Descripción
Verificar que el sistema permite crear un gasto con datos válidos y lo registra correctamente.

## Precondiciones
- El usuario está autenticado en la aplicación.
- El usuario se encuentra en la pantalla de creación de gastos.

## Pasos
1. Introducir una cantidad válida (por ejemplo, 50.00).
2. Seleccionar una categoría existente.
3. Introducir una fecha válida.
4. Introducir una descripción opcional.
5. Pulsar el botón de guardar.

## Resultado esperado
- El gasto se guarda correctamente.
- El gasto aparece en el listado de gastos.
- Los totales o resúmenes se actualizan correctamente.
- El sistema muestra un mensaje de confirmación o no muestra errores.

---

# Caso de prueba: Crear gasto con cantidad 0

## ID
TC-EXP-002

## Funcionalidad
Creación de un gasto

## Descripción
Verificar que el sistema no permite crear un gasto con una cantidad igual a 0.

## Precondiciones
- El usuario está autenticado en la aplicación.
- El usuario se encuentra en la pantalla de creación de gastos.

## Pasos
1. Introducir una cantidad igual a 0.
2. Seleccionar una categoría existente.
3. Introducir una fecha válida.
4. Introducir una descripción opcional.
5. Pulsar el botón de guardar.

## Resultado esperado
- El sistema no permite guardar el gasto.
- Se muestra un mensaje de error indicando que la cantidad no es válida.
- El gasto no aparece en el listado de gastos.
- Los totales o resúmenes no se modifican.

---

# Caso de prueba: Crear gasto sin cantidad

## ID
TC-EXP-003

## Funcionalidad
Creación de un gasto

## Descripción
Verificar que el sistema no permite crear un gasto cuando la cantidad está vacía.

## Precondiciones
- El usuario está autenticado en la aplicación.
- El usuario se encuentra en la pantalla de creación de gastos.

## Pasos
1. Dejar el campo cantidad vacío.
2. Seleccionar una categoría existente.
3. Introducir una fecha válida.
4. Introducir una descripción opcional.
5. Pulsar el botón de guardar.

## Resultado esperado
- El sistema no permite guardar el gasto.
- Se muestra un mensaje de error indicando que la cantidad es obligatoria.
- El gasto no aparece en el listado de gastos.
- Los totales o resúmenes no se modifican.
