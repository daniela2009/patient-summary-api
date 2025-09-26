# Estructura de Branches

Cada branch en este repositorio corresponde a una sección específica del endpoint `managePatientSummaryData`. Esto permite desarrollar, mantener y documentar cada funcionalidad de manera independiente y ordenada.

## Branches principales y su propósito

- **main**: Rama principal y estable. Contiene la versión de producción del código.

- **feature/encounter**: Implementa y mantiene la lógica relacionada con la sección Encounter (detalles, notas, overview, vital signs, medications, superbill, documentos adjuntos).

- **feature/allergies**: Gestiona la funcionalidad para la sección Allergies (creación, consulta, actualización y eliminación de alergias por paciente y fecha).

- **feature/goals**: Desarrolla la lógica para la sección GOALS (gestión de metas clínicas por paciente y fecha).

- **feature/message**: Implementa la sección MESSAGE (mensajes clínicos, firma y gestión por fecha).

- **feature/social-history**: Mantiene la funcionalidad de Social History (tabaquismo, alcohol, drogas, ejercicio, dieta).

- **feature/screenings**: Gestiona la sección Screenings (pruebas y procedimientos clínicos por paciente y fecha).

## Ventajas de esta estructura
- Permite trabajo colaborativo y paralelo en diferentes secciones.
- Facilita la revisión y el control de cambios por área funcional.
- Mejora la trazabilidad y documentación de cada parte del endpoint `managePatientSummaryData`.

Cada branch debe contener únicamente los cambios y mejoras relacionados con su sección correspondiente.
---

## Allergies

Esta sección gestiona toda la lógica relacionada con las alergias de los pacientes. Las acciones implementadas para el type `Allergies` en el código principal son:

### Acciones disponibles

- **create**: Permite crear nuevas alergias para un paciente, agrupadas por fecha y numeradas. Se pueden agregar múltiples alergias en una sola petición.
- **get**: Recupera las alergias existentes de un paciente, permitiendo filtrar por fecha o campo específico.
- **update**: Actualiza los datos de alergias existentes, ya sea modificando campos específicos o reemplazando la información de una fecha/número.
- **delete**: Elimina alergias específicas (por campo/fecha/número) o todo el documento de alergias de un paciente.

### Funciones afectadas

Las acciones de Allergies están implementadas y gestionadas principalmente en el archivo:

- `summary.js` (dentro de la lógica de `managePatientSummaryData`)

Cada acción corresponde a un bloque de código que maneja la petición HTTP y la interacción con Firestore para el type `Allergies`.

---

## GOALS

Acciones para el type `GOALS`:

- **create**: Crea metas clínicas para un paciente, agrupadas por fecha y numeradas.
- **get**: Recupera metas existentes, permite filtrar por fecha o campo.
- **update**: Actualiza metas específicas o campos.
- **delete**: Elimina metas por campo/fecha/número o todo el documento.

**Funciones afectadas:**
- `summary.js` (gestión en `managePatientSummaryData`)

---

## MESSAGE

Acciones para el type `MESSAGE`:

- **create**: Crea mensajes clínicos, agrupados por fecha y numerados, con campo SIGNED.
- **get**: Recupera mensajes existentes, permite filtrar por fecha o campo.
- **update**: Actualiza mensajes específicos o campos.
- **delete**: Elimina mensajes por campo/fecha/número o todo el documento.

**Funciones afectadas:**
- `summary.js` (gestión en `managePatientSummaryData`)

---

## Screenings

Acciones para el type `Screenings`:

- **create**: Crea registros de pruebas clínicas agrupadas por fecha y numeradas.
- **get**: Recupera screenings existentes, permite filtrar por fecha o campo.
- **update**: Actualiza screenings específicos o campos.
- **delete**: Elimina screenings por campo/fecha/número o todo el documento.

**Funciones afectadas:**
- `summary.js` (gestión en `managePatientSummaryData`)

---

## Health Concerns

Acciones para el type `Health Concerns`:

- **create**: Crea preocupaciones clínicas agrupadas por fecha y numeradas.
- **get**: Recupera health concerns existentes, permite filtrar por fecha o campo.
- **update**: Actualiza health concerns específicos o campos.
- **delete**: Elimina health concerns por campo/fecha/número o todo el documento.

**Funciones afectadas:**
- `summary.js` (gestión en `managePatientSummaryData`)

---

## Social History

Acciones para el type `Social History`:

- **create**: Crea o actualiza datos de tabaquismo, alcohol, drogas, ejercicio y dieta.
- **get**: Recupera datos sociales existentes, permite filtrar por campo.
- **update**: Actualiza campos específicos de social history.
- **delete**: Elimina campos específicos o todo el documento.

**Funciones afectadas:**
- `summary.js` (gestión en `managePatientSummaryData`)

---

## Encounter

Acciones para el type `Encounter` y sus subtypes (EncounterDetails, Note, Overview, Vital signs, Medications, Superbill, Documents attached to encounter):

- **create**: Crea registros de encuentros clínicos y sus subdocumentos.
- **get**: Recupera datos de encuentros y subdocumentos.
- **update**: Actualiza datos de encuentros y subdocumentos.
- **delete**: Elimina datos de encuentros y subdocumentos.

**Funciones afectadas:**
- `summary.js` (gestión en `managePatientSummaryData`)
