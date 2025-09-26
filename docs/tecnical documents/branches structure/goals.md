# Branch: feature/goals

Este documento describe exclusivamente la lógica y acciones implementadas para el branch `feature/goals`.

## Acciones disponibles

- **create**: Crea metas clínicas para un paciente, agrupadas por fecha y numeradas.
- **get**: Recupera metas existentes, permite filtrar por fecha o campo.
- **update**: Actualiza metas específicas o campos.
- **delete**: Elimina metas por campo/fecha/número o todo el documento.

## Funciones afectadas

Las acciones de GOALS están implementadas y gestionadas principalmente en el archivo:
- `summary.js` (dentro de la lógica de `managePatientSummaryData`)
