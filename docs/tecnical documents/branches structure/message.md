# Branch: feature/message

Este documento describe exclusivamente la lógica y acciones implementadas para el branch `feature/message`.

## Acciones disponibles

- **create**: Crea mensajes clínicos, agrupados por fecha y numerados, con campo SIGNED.
- **get**: Recupera mensajes existentes, permite filtrar por fecha o campo.
- **update**: Actualiza mensajes específicos o campos.
- **delete**: Elimina mensajes por campo/fecha/número o todo el documento.

## Funciones afectadas

Las acciones de MESSAGE están implementadas y gestionadas principalmente en el archivo:
- `summary.js` (dentro de la lógica de `managePatientSummaryData`)
