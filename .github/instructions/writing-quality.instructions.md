---
description: Estándares técnicos de escritura de Workfront para artículos de ayuda. Aplica la Guía de estilo de la documentación de Workfront y los principios de Desarrollo de información técnica de calidad (DQTI).
applyTo: "help/**/*.md"
source-git-commit: 59deddd679267d10059f19cfd2d86b164903500e
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 1%
---

# Calidad de escritura

Aplique estos estándares siempre que edite, revise o escriba un artículo de ayuda.
Conservar la intención y la precisión técnica del autor. Para la versión completa
puntuación, terminología, mayúsculas y referencia de procedimiento, lectura
[.cursor/skills/writing-quality/reference.md](../../.cursor/skills/writing-quality/reference.md).

**no** aplica estas reglas a las notas de la versión de
`help/quicksilver/product-announcements/product-releases/` — usar
en su lugar, instrucciones de release-notes-formatter.

## Voz y punto de vista

- Usar **segunda persona** (&quot;Puedes...&quot;) al dirigirse al lector.
- Usa contracciones para un tono conversacional (no lo hagas, no puedes, es, son).
- Utilice &quot;Recomendamos&quot; para prácticas recomendadas, no &quot;Se recomienda&quot; ni &quot;Debería&quot;.
- Al escribir para un grupo de usuarios, haga referencia a otras funciones en tercera persona.
- Nunca use pronombres de género — reestructura la oración o use &quot;ellos&quot;.
- Sin barra para las opciones: use &quot;o&quot; (&quot;él o ella&quot; no &quot;él/ella&quot;).

## Claridad (DQTI)

- Una idea por frase; mantenga frases por debajo de ~25 palabras siempre que sea posible.
- El posible cliente con la acción o el resultado, no con el contexto de fondo.
- Utilice la palabra más simple (&quot;usar&quot; no &quot;utilizar&quot;, &quot;iniciar&quot; no &quot;iniciar&quot;).
- Evite las nominalizaciones (&quot;crear&quot;, no &quot;la creación de&quot;).
- Utilice un lenguaje específico y concreto: evite términos vagos (&quot;varios&quot;, &quot;varios&quot;).
- Evite los negativos dobles.

## Concreción y orientación de tareas (DQTI)

- Utilice ejemplos específicos con valores realistas; asigne un nombre a los elementos y campos de la IU exacta.
- Céntrese en lo que el usuario *puede hacer*, no en lo que el sistema *es*.
- Procedimientos principales con verbos imperativos (&quot;Crear una tarea&quot;, &quot;Configurar notificaciones&quot;).
- Proporcione contexto suficiente para actuar, pero no más.
- Incluya un vínculo a la ayuda detallada (&quot;Para obtener más información, consulte [artículo].&quot;).

## Uso de mayúsculas

- **Encabezados**: siempre utilice mayúsculas y minúsculas (&quot;Crear una tarea&quot;, no &quot;Crear una tarea&quot;).
- **Términos de Workfront**: use mayúsculas únicamente cuando haga referencia directamente a un elemento de la interfaz de usuario.
  - Directo: &quot;Rellene el campo Fecha planificada de finalización&quot;.
  - Indirecto: &quot;Cada tarea debe tener una fecha planificada de finalización&quot;.
  - Sugerencia: si puede poner &quot;the&quot; o &quot;a&quot; delante del término, normalmente está en minúsculas.
- **Botones**: seguir el uso de mayúsculas en la interfaz de usuario; los botones en mayúsculas se convierten en mayúsculas y minúsculas.
- **Roles**: &quot;Administrador del sistema&quot; para el rol en la interfaz de usuario; &quot;Workfront
&quot;administrador&quot; de la persona.

## Encabezados

- Comando imperativo en caso de oración, basado en tareas (&quot;Configurar niveles de acceso&quot;).
- Los artículos de información general terminan con &quot;información general&quot; (&quot;Información general de proyectos&quot;).
- Divida las secciones largas en varios encabezados con subobjetivos claros.

## Referencias cruzadas y vínculos

| Situación | Formato |
|-----------|--------|
| Vínculo después de proporcionar información | &quot;Para obtener más información, consulte [Nombre del artículo].&quot; |
| Vínculo sin información previa | &quot;Para obtener más información, consulte [Nombre del artículo].&quot; |
| Vínculo a una sección de otro artículo | &quot;Para obtener más información, consulte [Nombre de sección] en [Nombre de artículo].&quot; |
| Vínculo a una sección del mismo artículo | &quot;Para obtener más información, consulte [Nombre de sección] en este artículo&quot;. |

- En un párrafo: en línea. En un paso de procedimiento: en una nueva línea después del paso.
- Varios vínculos: utilice una lista con viñetas.
- Utilice &quot;esquina superior derecha&quot; / &quot;esquina superior izquierda&quot; para las posiciones de la pantalla.

## Negrita y cursiva

- **Negrita** acciones en las que se puede hacer clic y elementos de la interfaz de usuario **solo en pasos del procedimiento**.
- No aplique negrita a los elementos de la interfaz de usuario, nombres de cuadros de diálogo, nombres de páginas, nombres de iconos ni menús
nombres fuera de los pasos del procedimiento.
- Utilice *cursiva* para el texto que el usuario debe escribir (&quot;Escriba *my.workfront.com*...&quot;).
- Nunca use cursiva para enfatizar; en su lugar, reestructura la oración.

## Notas, sugerencias y advertencias

Usar con moderación: el uso excesivo los hace invisibles.

- Máximo de una nota/sugerencia/advertencia por sección; no apilarlas nunca.
- Combine notas relacionadas en una nota con una lista con viñetas.
- No use las notas para anunciar nuevas funciones; en su lugar, vuelva a redactar el texto del artículo.

| Tipo | Objetivo |
|------|---------|
| `>[!NOTE]` | Información que no se ajusta al párrafo; versiones/compatibilidad |
| `>[!TIP]` | Sugerencias agradables de tener que facilitan la vida del usuario |
| `>[!IMPORTANT]` | Información vital para el paso o procedimiento |
| `>[!WARNING]` | Alertar al usuario sobre la posible pérdida de datos |

## Procedimientos

- Utilice encabezados de comando imperativos; introducciones solo cuando sea necesario.
- Formato de introducción preferido: frase infinitiva + dos puntos (&quot;Para crear una
contraseña:&quot;).
- Los procedimientos de un solo paso siguen utilizando una lista numerada.
- Use &quot;type&quot; o &quot;select&quot; — evite palabras vagas como &quot;set&quot; o &quot;specified&quot;.
- Pasos condicionales: &quot;(Condicional) Si es miembro de más de un equipo,
seleccione...&quot;. Pasos opcionales: &quot;(Opcional) Para añadir un emoji, haga clic en...&quot;.
- Describa la respuesta del sistema antes o inmediatamente después de que se produzca.
- Varios métodos: primero documente la forma más directa y luego utilice &quot;Or&quot;.
- Navegación por menús/pestañas: &quot;Haga clic en **Correo electrónico** > **Notificaciones**&quot; (ponga en negrita los nombres, no
los paréntesis; espacios entre paréntesis). No utilizar corchetes en el menú principal
navegación: utilice el fragmento de menú principal.

## Referencia rápida de puntuación

| Regla | Ejemplo |
|------|---------|
| Coma de Oxford siempre | &quot;motivo, medios y oportunidad&quot; |
| Coma antes de &quot;then&quot; en los procedimientos | &quot;Haga clic en Configuración y luego en Interfaz.&quot; |
| Coma tras año en una fecha a mitad de la frase | &quot;La edición del 2 de enero de 2016 de...&quot; |
| Sin comas solo mes-año | &quot;Enero de 2016&quot; |
| Dos puntos antes de una lista, en minúsculas después de | &quot;Seleccione una de las siguientes opciones: opción A&quot; |
| No hay dos puntos después de encabezados de procedimiento | &quot;Crear una tarea&quot; |
| Guiones elásticos con moderación | Reestructurar la oración si es posible |
| Períodos en las extensiones de archivo | &quot;Cargar un archivo .pdf&quot; |

## Organización (DQTI)

- Estructura lógica con revelación progresiva (descripción general → detalles → referencia).
- Un tema por sección; utilice listas para más de 3 elementos paralelos.
- Mantenga los elementos de la lista y su posible cliente en paralelo gramaticalmente.
- Utilice tablas para realizar comparaciones estructuradas o descripciones de campos.
- Evite los párrafos de pared de texto: divida en fragmentos digeribles.

## Lista de comprobación de validación

- [ ] Segunda persona durante todo el tratamiento, contracciones utilizadas.
- [ ] caso de oración en todos los encabezados.
- [ ] términos de Workfront se capitalizaron correctamente (referencia directa e indirecta).
- [ ] Solo en negrita en acciones en las que se puede hacer clic dentro de los pasos del procedimiento.
- [ ]: las referencias cruzadas utilizan el formato estándar.
- [ ] notas/sugerencias/advertencias no apiladas, máximo una por sección.
- [ ] coma de Oxford usada de manera consistente.
- [ ] Los pasos del procedimiento utilizan verbos específicos (escriba, seleccione, haga clic).
- [ ] pasos condicionales/opcionales etiquetados correctamente.
- [ ] No hay pronombres de género.
- [ ] frases claras, concretas y orientadas a tareas; la estructura paralela se mantiene.
