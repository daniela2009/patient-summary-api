# Branch: feature/encounter

Este documento describe exclusivamente la lógica y acciones implementadas para el branch `feature/encounter`.

## Acciones disponibles

- **create**: Crea registros de encuentros clínicos y sus subdocumentos (EncounterDetails, Note, Overview, Vital signs, Medications, Superbill, Documents attached to encounter).
- **get**: Recupera datos de encuentros y subdocumentos.
- **update**: Actualiza datos de encuentros y subdocumentos.
- **delete**: Elimina datos de encuentros y subdocumentos.

## Funciones afectadas

Las acciones de Encounter están implementadas y gestionadas principalmente en el archivo:
- `summary.js` (dentro de la lógica de `managePatientSummaryData`)
