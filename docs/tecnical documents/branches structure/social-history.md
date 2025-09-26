# Branch: feature/social-history

Este documento describe exclusivamente la lógica y acciones implementadas para el branch `feature/social-history`.

## Acciones disponibles

- **create**: Crea o actualiza datos de tabaquismo, alcohol, drogas, ejercicio y dieta.
- **get**: Recupera datos sociales existentes, permite filtrar por campo.
- **update**: Actualiza campos específicos de social history.
- **delete**: Elimina campos específicos o todo el documento.

## Funciones afectadas

Las acciones de Social History están implementadas y gestionadas principalmente en el archivo:
- `summary.js` (dentro de la lógica de `managePatientSummaryData`)
