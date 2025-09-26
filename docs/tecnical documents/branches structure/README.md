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
