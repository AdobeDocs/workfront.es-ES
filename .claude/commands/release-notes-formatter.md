---
name: release-notes-formatter
description: Dé formato y valide a las notas de la versión de Workfront para mantener la coherencia, una estructura correcta y una vinculación adecuada. Se utiliza solo para archivos de notas de versiones en directorios de versiones de productos o cuando el usuario menciona notas de versiones, versiones de productos o versiones trimestrales. No lo aplique a artículos de procedimientos o documentación general.
source-git-commit: fa39320af72acf6d2ceaf201480baf78a07ae76e
workflow-type: tm+mt
source-wordcount: '1729'
ht-degree: 3%

---


# Formato de notas de versión

Aplica formato y valida las notas de la versión de Adobe Workfront en el directorio `help/quicksilver/product-announcements/product-releases/`.

## Tipos de página

Identifique el tipo de página a partir de la ruta y el contenido del archivo:

| Tipo de página | Patrón de archivos | Plantilla |
|-----------|-------------|----------|
| **Información general** | `{YY}-q{N}-release-overview.md` | Consulte .claude/commands/_release-notes-formatter-reference.md#overview-page-template |
| **Área de producto** | `{YY}-q{N}-{area}.md` | Consulte .claude/commands/_release-notes-formatter-reference.md#product-area-page-template |
| **Planificación** | `planning-release-activity-{YY}-q{N}.md` | Similar al área de producto |
| **Aspecto** | `look-and-feel-updates-{YY}-q{N}.md` | Consulte .claude/commands/_release-notes-formatter-reference.md#look-and-feel-page-template |

## Paso 0: Determine el trimestre (haga esto antes que cualquier otra cosa)

>[!IMPORTANT]
>
>Nunca asigne una función a un trimestre doc usando matemáticas de trimestre calendario en su fecha de Previsualización o Producción. El trimestre del documento se basa en la **versión mensual** en la que se envía la característica, según la agrupación del calendario de versiones interno de Workfront, que se desvía del trimestre natural; consulte la tabla [Calendario de versiones de 2026](#2026-release-calendar) cerca del final de este archivo. Por ejemplo, una característica con una fecha de producción del 13 de agosto de 2026 pertenece al trimestre doc `26-q4`, no a `26-q3`, porque la versión mensual de agosto se asigna a `26-q4`.
>
>La tabla &quot;Asignación de trimestres&quot; más abajo (Formulario escrito/meses) es para escribir nombres de trimestres en títulos (por ejemplo, &quot;Tercer trimestre&quot; para el tercer trimestre); **no** es suficiente por sí sola para decidir a qué archivos de trimestre pertenece una característica. Compruebe siempre con la tabla Calendario de versiones antes de crear o editar cualquier archivo.
>
>Si la fecha de producción de una función no aparece en la tabla Calendario de lanzamiento (por ejemplo, está fuera del intervalo de fechas de la tabla), pida al usuario un calendario actualizado en lugar de adivinar.

## Flujo de trabajo de formato

### Paso 1: Validar Frontmatter

Campos obligatorios para todas las páginas de notas de la versión:

```yaml
---
title: <descriptive title>
description: <matches or summarizes the title>
author: <author name>
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: <existing UUID — never generate or change>
---
```

Reglas:
- `feature` debe ser exactamente `Product Announcements`
- `recommendations` debe ser exactamente `noDisplay, noCatalog`
- No inventar nunca un(a) `exl-id`: incluir solo si ya existe uno
- No agregue `draft: Probably` a páginas reales (solo plantillas)

### Paso 2: Validar la estructura por tipo de página

#### Páginas de área de producto

1. **H1**: `{Written Quarter} {Area} enhancements`
   - Ejemplo: `# Second Quarter 2026 Administrator enhancements`
   - El trimestre debe escribirse: &quot;Primer trimestre&quot;, &quot;Segundo trimestre&quot;, &quot;Tercer trimestre&quot;, &quot;Cuarto trimestre&quot;

2. **Párrafo introductorio**: Describe el área y los vínculos a la descripción general
   - Debe vincularse al archivo de información general **del trimestre correcto**
   - Error común: se está vinculando con el trimestre anterior (por ejemplo, `26-q1` en lugar de `26-q2`)

3. **H2 por característica**: título de característica como encabezado
   - **Las características más recientes primero**: la nota de la versión más reciente debe aparecer como el primer H2 después del párrafo de introducción
   - Las funciones antiguas se siguen en orden cronológico inverso

4. **Bloque de llamada de fecha** después de cada H2:

```markdown
>[!NOTE]
>
>Preview: {Month Day, Year}
>Production fast release: {Month Day, Year}
>Production for everyone: {Month Day, Year}
```

&#x200B;5. **Cuerpo**: Descripción de la función y después vínculo a la documentación de ayuda

#### Páginas de información general

1. **H1**: `{Written Quarter} release overview`

2. **Párrafo de introducción** con mes de lanzamiento programado

3. **`>[!IMPORTANT]`bloque** con tabla de programación de versiones

4. **H2`Adobe Workfront enhancements`** con lista con viñetas de vínculos de anclaje:

```markdown
* [Administrator enhancements](#administrator-enhancements)
* [Document enhancements](#document-enhancements)
```

&#x200B;5. **H3 por área de producto** con tabla de características de HTML (consulte .claude/commands/_release-notes-formatter-reference.md#overview-feature-table)
   - Dentro de cada tabla, **las características más recientes primero**, la fila más reciente aparece en la parte superior de la tabla (después de la fila de encabezado)

&#x200B;6. **Secciones finales** (H2): Notas de la versión para otras áreas, Actualizaciones del visor de revisión de escritorio, Anuncios, Versión de API, Actualizaciones de mantenimiento, Actualizaciones de formación

### Paso 3: Validación de vínculos

- **Vínculo de información general en las páginas de área de productos**: Debe señalar al mismo trimestre
  - Correcto: `26-q2-release-activity/26-q2-release-overview.md`
  - Incorrecto: `26-q1-release-activity/26-q1-release-overview.md`
- **Vínculos de anclaje en la descripción general**: Debe coincidir con los ID de H3 (en minúsculas, guiones)
- **Vínculos de características en tablas de información general**: Debe usar `class="MCXref xref" xrefformat="{para}"`
- **Vínculos del documento de ayuda**: Debe comenzar con `/help/quicksilver/`

### Paso 4: Validar las fechas

- Formato: `{Month} {Day}, {Year}` (por ejemplo, &quot;12 de marzo de 2026&quot;)
- Usar `TBD` para fechas desconocidas
- Las fechas del bloque de la página `>[!NOTE]` del área de productos deben coincidir con la fila de la tabla de resumen correspondiente
- Las fechas de vista previa deben preceder a las de producción

### Paso 5: Correcciones comunes

Aplique estas correcciones al dar formato:

| Problema | Corregir |
|-------|-----|
| Trimestre de vínculo de información general incorrecto | Actualizar para que coincida con el trimestre del propio archivo |
| Falta el bloque de fecha `>[!NOTE]` | Añadir bloque después del encabezado de la función H2 |
| Formato de fecha incoherente | Estandarizar a `Month Day, Year` |
| Falta una línea en blanco antes de `>[!NOTE]` | Añadir línea en blanco |
| Espacios adicionales en las líneas de llamada | Recortar espacio final |
| HTML en páginas de área de producto | Mantener como marcador (HTML solo sirve para tablas de información general) |
| Falta `exl-id` | Déjelo fuera, no genere uno |

### Paso 6: Actualizar el índice

Siempre que cree una **nueva** página de nota de versión (información general o área de producto), agréguela a `help/quicksilver/TOC.md` con el mismo cambio. Las páginas que no estén en el índice no aparecerán en la navegación publicada, aunque los vínculos de la tabla de resumen apunten a ellas.

Dónde se agrega:

- La TDC tiene una sección por trimestre bajo un encabezado como `* 2026 Q3 Release {#release-26-q3}`. Si el encabezado del trimestre aún no existe (primera página de un nuevo trimestre), agréguelo por encima del trimestre anterior para que el trimestre más reciente aparezca en la parte superior.
- Bajo ese encabezado de trimestre, enumere las páginas en este orden:
  1. **Información general** primero (`Third Quarter 2026 release overview`).
  2. **Páginas de área de producto** alfabéticamente por nombre de área (Administrador, Documentos, Operaciones de empresa, Proyectos, Informes, Solicitud).
  3. **Otras mejoras** duran (siempre después de las áreas de producto alfabéticas).

Cada entrada del índice es un vínculo de markdown que utiliza el título de página y la ruta absoluta del repositorio:

```markdown
      * [Third Quarter 2026 Documents enhancements](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-documents.md)
```

Hacer coincidir la sangría (seis espacios) con las entradas adyacentes. Use la página H1 literalmente como texto del vínculo, por ejemplo `Documents enhancements`, `Requesting enhancements` (no `Requests`), de modo que las etiquetas de tabla de contenido coincidan con trimestres anteriores.

Errores comunes que se deben evitar:

- Creación de una página de área de producto sin agregarla al índice.
- Vínculo a una descripción general de trimestre diferente desde la nueva página de área de producto (paso 3).
- Inserción de páginas de un nuevo trimestre bajo el encabezado del trimestre anterior.

### Paso 7: Actualizar la página de inicio

Siempre que cree una **página de información general del trimestre nuevo** (es decir, esta es la primera página de un trimestre nuevo, no solo una página de área de producto nueva agregada a un trimestre existente), actualice `help/quicksilver/home.md` con el mismo cambio:

- En la sección `>[!TAB Latest release]`, reemplace el vínculo de información general de la versión con el vínculo de información general del nuevo trimestre.
- También en esa sección, actualice el vínculo de actividad de la versión de Adobe Workfront Planning para que indique el archivo de planificación del nuevo trimestre (`planning-release-activity-{YY}-q{N}.md`), si existe.
- En la ficha `>[!TAB {YYYY} releases]` del año actual, agregue el vínculo de información general del nuevo trimestre en la parte superior de la lista, encima de la entrada del trimestre anterior.

No toque `home.md` al agregar solamente una página de área de producto a un trimestre que ya tiene una página de información general en la lista.

Errores comunes que se deben evitar:

- Crear una página de información general de un trimestre nuevo sin actualizar la ficha &quot;Última versión&quot; de `home.md` (seguirá apuntando al trimestre anterior).
- Olvidando agregar también el nuevo trimestre a la lista de pestañas del año actual.

## Convenciones de nomenclatura de archivos

| Tipo | Patrón | Ejemplo |
|------|---------|---------|
| Información general | `{YY}-q{N}-release-overview.md` | `26-q2-release-overview.md` |
| Área de producto | `{YY}-q{N}-{area-slug}.md` | `26-q2-admin-and-setup.md` |
| Directorio | `{YY}-q{N}-release-activity/` | `26-q2-release-activity/` |

slugs de área estándar: `admin-and-setup`, `documents`, `projects`, `reports`, `requests`, `other`

## Asignación de trimestre

>[!NOTE]
>
>Esta tabla es para escribir nombres de trimestres (por ejemplo, en un H1 o título). NO determina a qué archivos de trimestre pertenece una característica: use la tabla [Calendario de versiones de 2026](#2026-release-calendar) que aparece a continuación para eso, ya que doc-quarter está desplazado de calendar-quarter.

| Trimestre | Formulario escrito | Meses |
|---------|-------------|--------|
| Primer trimestre | Primer trimestre | Ene-Mar |
| Segundo trimestre | Segundo trimestre | Abr-Jun |
| Tercer trimestre | Tercer trimestre | Jul-Sep |
| Cuarto trimestre | Cuarto trimestre | Oct-Dic |

**Importante: el trimestre doc usado en los nombres de archivo (`26-q3`, `26-q4`, etc.) se desplaza en un mes con respecto a esta asignación de calendario.** En su lugar, sigue la agrupación del calendario de versiones interno de Workfront, donde cada trimestre doc = las dos versiones mensuales anteriores + el mes de lanzamiento trimestral. Por ejemplo, el trimestre doc `26-q3` cubre las versiones mensuales de mayo, junio y julio de 2026 (versión trimestral `2026.07`) y el trimestre doc `26-q4` cubre las versiones mensuales de agosto, septiembre y octubre de 2026 (versión trimestral `2026.10`). Compruebe siempre el calendario de versiones que aparece a continuación (o pida uno actualizado) antes de asumir el trimestre de un archivo según la tabla de trimestres del calendario que se muestra arriba.

## Calendario de versiones 2026

Source: &quot;Calendario de versiones mensuales de 2026&quot; (wiki de Adobe corp, espacio AWF — `wiki.corp.adobe.com`, clave de espacio AWF, título &quot;Calendario de versiones mensuales de 2026&quot;). WebFetch no puede llegar a esta página (requiere Adobe SSO); pida al usuario que pegue un PDF/tabla actualizado cuando se necesiten fechas más allá de lo que se captura aquí.

| Mes de lanzamiento | Previsualización final | Producción | Versión mensual | Versión trimestral | Doc Trimestre |
|---|---|---|---|---|---|
| Noviembre de 2025 | 30 de octubre de 2025 | 13 de noviembre de 2025 | 2025.11 | 2026.01 | 26-q1 |
| Diciembre de 2025 | 27 de noviembre de 2025 | 11-dic-2025 | 2025.12 | 2026.01 | 26-q1 |
| Enero de 2026 | 23 de diciembre de 2025 | 15 de enero de 2026 | 2026.01 | 2026.01 | 26-q1 |
| Febrero de 2026 | 29 de enero de 2026 | 12 de febrero de 2026 | 2026.02 | 2026.04 | 26-q2 |
| Marzo de 2026 | 26 de febrero de 2026 | 12 de marzo de 2026 | 2026.03 | 2026.04 | 26-q2 |
| Abril de 2026 | 2 de abril de 2026 | 16 de abril de 2026 | 2026.04 | 2026.04 | 26-q2 |
| Mayo de 2026 | 30 de abril de 2026 | 14 de mayo de 2026 | 2026.05 | 2026.07 | 26-q3 |
| Junio de 2026 | 28 de mayo de 2026 | 11 de junio de 2026 | 2026.06 | 2026.07 | 26-q3 |
| Julio de 2026 | 7 de julio de 2026 | 16 de julio de 2026 | 2026.07 | 2026.07 | 26-q3 |
| Ago de 2026 | 30 de julio de 2026 | 13 de agosto de 2026 | 2026.08 | 2026.10 | 26-q4 |
| Septiembre de 2026 | 3 de septiembre de 2026 | 17 de septiembre de 2026 | 2026.09 | 2026.10 | 26-q4 |
| Octubre de 2026 | 1-oct-2026 | 15 de octubre de 2026 | 2026.10 | 2026.10 | 26-q4 |
| Noviembre de 2026 | 29 de octubre de 2026 | 12 de noviembre de 2026 | 2026.11 | 2027.01 | 27-q1 |
| Diciembre de 2026 | 26 de noviembre de 2026 | 10-dic-2026 | 2026.12 | 2027.01 | 27-q1 |
| Enero de 2027 | 5 de enero de 2027 | 14 de enero de 2027 | 2027.01 | 2027.01 | 27-q1 |

Notas sobre el uso de esta tabla

- **Vista previa final** son las últimas funciones de fecha que pueden aparecer en Vista previa para esa versión mensual. Utilícelo para la viñeta de la página de información general &quot;Última fecha en la que las funciones pueden aparecer en el entorno de vista previa&quot; (solo mes de fin de trimestre).
- **Producción** es la fecha oficial de Producción para todos para esa versión mensual.
- Para el mes de fin de trimestre (el que coincide con la columna Versión trimestral), la tabla de programación de la página de información general enumera la versión de ese mes **dos veces**: una vez en la columna &quot;Versión mensual&quot; con fecha de **un día antes** de la fecha de producción (la fecha de lanzamiento rápido) y una vez en la columna &quot;Versión trimestral&quot; con fecha de la fecha real de producción. Los meses no finales de un trimestre utilizan la misma fecha de producción tanto en la lista mensual como en cualquier referencia de &quot;lanzamiento rápido&quot;, no se necesita ningún ajuste.
- Esta tabla solo se extiende hasta enero de 2027. Cuando se necesitan fechas posteriores, pídale al usuario un calendario actualizado en lugar de adivinar.

La versión de producción trimestral aterriza generalmente el jueves de la segunda semana completa del último mes del trimestre.

## Lista de comprobación de validación

Cuando revise un archivo de notas de la versión, compruebe:

- [ ] Frontmatter tiene todos los campos obligatorios con los valores correctos
- [ ] H1 coincide con el formato de tipo de página
- [ ] El vínculo de información general apunta al trimestre correcto
- [ ] Cada característica tiene un bloque de fecha `>[!NOTE]` (páginas de área de producto)
- [ ] El formato de fecha es coherente (`Month Day, Year`)
- [ ] Las filas de la tabla de características de la descripción general coinciden con el contenido de página del área de producto
- [ ] No hay vínculos internos rotos
- [ ] vínculos de anclaje en la descripción general coinciden con los ID de sección H3
- [ Las características de ] se ordenan más recientes (tanto páginas de área de productos como tablas de información general)
- [ ] Las nuevas páginas de notas de la versión se enumeran en `help/quicksilver/TOC.md` en el trimestre correcto, con la descripción general en primer lugar y las áreas de producto en orden alfabético (el otro en último lugar)
- [ ] Si se creó la página de información general de un nuevo trimestre, `help/quicksilver/home.md` pestaña &quot;Última versión&quot; y la pestaña del año actual apuntan a ella

## Recursos adicionales

- Para ver plantillas y ejemplos completos de HTML, consulte .claude/commands/_release-notes-formatter-reference.md
