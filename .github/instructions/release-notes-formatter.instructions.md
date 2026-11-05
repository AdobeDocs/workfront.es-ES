---
description: Reglas de formato y validación para las notas de la versión de Adobe Workfront (información general, área de producto, planificación y páginas de aspecto y presentación).
applyTo: "help/quicksilver/product-announcements/product-releases/**/*.md"
source-git-commit: 59deddd679267d10059f19cfd2d86b164903500e
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%
---

# Formador de notas de versión

Estos archivos son **notas de la versión**, no artículos explicativos. **no** aplica el
estándares generales de calidad de escritura aquí. Antes de editar, lea el origen completo de
true, que incluye las plantillas y el calendario de versiones:

- [.cursor/skills/release-notes-formatter/SKILL.md](../../.cursor/skills/release-notes-formatter/SKILL.md)
- [.cursor/skills/release-notes-formatter/reference.md](../../.cursor/skills/release-notes-formatter/reference.md)

## Regla crítica: determine primero el trimestre doc

&#x200B;> [!IMPORTANT]
> Nunca asigne una función a un trimestre doc usando matemáticas de trimestre calendario en su
> Vista previa o fecha de producción. El trimestre del documento se basa en el **lanzamiento mensual**
> la función se envía en, por la agrupación de calendario de versiones interna de Workfront, que
> se desvía del trimestre natural. Por ejemplo, una función con una variable Producción
> la fecha del 13 de agosto de 2026 pertenece al trimestre del documento `26-q4`, no a `26-q3`. Siempre
> compruebe la tabla Calendario de versiones 2026 en el archivo de referencia antes de que
> crear o editar cualquier archivo. Si una fecha de producción queda fuera de esa tabla,
> pida un calendario actualizado en lugar de adivinar.

## Reglas estructurales clave

- **Frontmatter**: `feature` debe ser exactamente `Product Announcements`;
  `recommendations` debe ser exactamente `noDisplay, noCatalog`. Nunca inventes un
  `exl-id` — incluirlo sólo si ya existe uno.
- **Las características más recientes primero**: la nota de la versión más reciente es la primera H2 después de
la introducción (páginas de área de producto) y la fila superior de cada tabla de funciones (descripción general)
páginas).
- **Vínculo de información general**: las páginas de área de producto deben vincularse a **su propio trimestre**
archivo de información general: un error común se está vinculando al trimestre anterior.
- **Llamada de fecha**: cada característica H2 va seguida de un bloque `>[!NOTE]` con
Previsualización / Producción versión rápida / Producción para todas las fechas, coincidiendo con el
fila de tabla de información general. Dar formato a las fechas como `Month Day, Year`; usar `TBD` si se desconoce.
- **Nombres de trimestres escritos** en H1s: &quot;Primer trimestre&quot;, &quot;Segundo trimestre&quot;, &quot;Tercero
Trimestre&quot;, Cuarto Trimestre&quot;.

## Actualizaciones complementarias necesarias al agregar páginas

- **Nueva página (cualquiera)**: agréguela a `help/quicksilver/TOC.md` con el mismo cambio
(descripción general en primer lugar, páginas de área de producto alfabéticamente y otras mejoras en último lugar).
- **Página de información general del nuevo trimestre**: también actualizar `help/quicksilver/home.md` —
actualice el vínculo de la pestaña &quot;Última versión&quot; y el vínculo de la actividad de planificación y añada
Seleccione la pestaña nuevas versiones del trimestre actual.

Consulte los archivos SKILL.md y reference.md anteriores para ver las plantillas completas,
convenciones de nomenclatura de archivos, formatos de vínculos y el calendario de versiones completo.
