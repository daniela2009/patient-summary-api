# Branch: feature/screenings

Este documento describe exclusivamente la lógica y acciones implementadas para el branch `feature/screenings`.

## Acciones disponibles

- **create**: Crea registros de pruebas clínicas agrupadas por fecha y numeradas.
- **get**: Recupera screenings existentes, permite filtrar por fecha o campo.
- **update**: Actualiza screenings específicos o campos.
- **delete**: Elimina screenings por campo/fecha/número o todo el documento.

## Funciones afectadas

Las acciones de Screenings están implementadas y gestionadas principalmente en el archivo:
- `summary.js` (dentro de la lógica de `managePatientSummaryData`)
