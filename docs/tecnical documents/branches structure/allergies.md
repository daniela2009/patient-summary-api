# Branch: feature/allergies

Este documento describe exclusivamente la lógica y acciones implementadas para el branch `feature/allergies`.

## Acciones disponibles

- **create**: Permite crear nuevas alergias para un paciente, agrupadas por fecha y numeradas. Se pueden agregar múltiples alergias en una sola petición.
- **get**: Recupera las alergias existentes de un paciente, permitiendo filtrar por fecha o campo específico.
- **update**: Actualiza los datos de alergias existentes, ya sea modificando campos específicos o reemplazando la información de una fecha/número.
- **delete**: Elimina alergias específicas (por campo/fecha/número) o todo el documento de alergias de un paciente.

## Funciones afectadas

Las acciones de Allergies están implementadas y gestionadas principalmente en el archivo:
- `summary.js` (dentro de la lógica de `managePatientSummaryData`)

Cada acción corresponde a un bloque de código que maneja la petición HTTP y la interacción con Firestore para el type `Allergies`.
