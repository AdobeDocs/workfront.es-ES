---
source-git-commit: b3148e5706abd75f2dd260f32507dedf8e259f57
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 0%

---
# Solicitudes de extracción (PR)

Cuando redacte o revise un título o una descripción de solicitud de extracción (por ejemplo, en GitHub/GitLab o cuando se le pregunte en el chat del agente), siga estas convenciones.

## Derivación del problema Jira

- **Source de la verdad:** Derive el ID del problema Jira a partir del **nombre de la rama Git actual** (por ejemplo, un segmento que coincida con el patrón de clave de su proyecto, como `FFENT-8796`).
- **Si el nombre de la sucursal incluye un ID Jira:** Use ese ID en el título PR (ver abajo) y vincúlelo en `# Context` → `## Jira`.
- **Si el nombre de la sucursal no incluye un ID de Jira:** Trate el PR como no asociado a un ticket. **Omitir** la clave Jira del título PR (no inventar un ticket). Sigue incluyendo `# Context` → `## Jira`, con el contenido exactamente: `No ticket` (sin vínculo).

## Título de PR

**Cuando el nombre de la rama incluye un ID de problema de Jira**, incluya **ambos**:

1. **Id. de problema de Jira** (p. ej. `FFENT-8001`).
2. El **tipo de confirmación** (consulte la lista siguiente), con este patrón:

`{type}/{JIRA-ID}- {short task description}`

Ejemplo:

`feat/FFENT-8001- Add validation for numVariations in OCAPI request`

Utilice una descripción concisa de estilo imperativo después del ID. Haga coincidir el patrón de espaciado que se muestra: tipo, barra diagonal, tecla Jira con guión final, espacio y, a continuación, la descripción.

**Cuando el nombre de la sucursal no incluya un ID de problema de Jira**, omita el ticket del título y use:

`{type}- {short task description}`

Ejemplo:

`docs- Refresh Object Composite API changelog`

### Tipos de confirmación aceptables (utilice exactamente estas etiquetas antes de `/`)

- **feat** — agrega una nueva característica. Cuando se agrega un nuevo elemento del índice o el JIRA se conecta a otro Jira de `feat` etiquetado como.
- **corregir** — corrige un error
- **refactor** — reescribe/reestructura el código sin cambiar el comportamiento
- **perf** — mejora el rendimiento (refactor especial)
- **style**: solo formato/espacio en blanco; sin cambio de significado. Solo ediciones
- **prueba** — agrega o corrige pruebas
- **docs** — Nuevo contenido añadido. solo documentación
- **build**: herramientas de compilación, CI, dependencias, versión del proyecto, etc.
- **ops**: infraestructura, implementación, copia de seguridad, recuperación, etc.
- **tarea** — varias (p. ej. `.gitignore`)

## PR body — secciones requeridas

Use **exactamente estas secciones de nivel superior** (encabezados de Markdown):

### 1. `# Summary`

Breve descripción general de **lo que** cambió y **por qué** (intención técnica o de negocios).

### 2. `# Changes`

Organizar por **archivo**. Para cada archivo tocado, utilice un encabezado de nivel 2 con la ruta en acentos graves y luego puntos de viñeta que describan las ediciones.

Formato:

```markdown
# Changes

## `path/to/file.ext`
* Concise bullet describing the change in that file.

## `another/file.ts`
* Another bullet for that file.
```

### 3. `# Context`

Incluya siempre una subsección **Jira** en `# Context`.

**Cuando el nombre de la rama incluya un ID de Jira:** Use un vínculo al problema en el que se pueda hacer clic (derive la clave del nombre de la rama).

Formato:

```markdown
# Context

## Jira
[FFENT-8796](https://jira.corp.adobe.com/browse/FFENT-8796)
```

Reemplace la clave y la URL por el ticket real. Si se aplican varios tickets, enumere cada uno en su propia línea en la misma subsección.

**Cuando el nombre de la rama no incluye un identificador Jira:** Mantenga `## Jira` y use exactamente:

```markdown
# Context

## Jira
No ticket
```

## Ejemplo (descripción completa de PR)

```markdown
# Summary
Adds minimum and maximum constraints for numVariations in the Object Composite API v4 OpenAPI spec.

# Changes

## `static/object-composite-v4.json`
* numVariations in OCAPIRequest now includes minimum: 1 and maximum: 3 to align with the allowed range (number of variations to generate).

# Context

## Jira
[FFENT-8796](https://jira.corp.adobe.com/browse/FFENT-8796)
```

## Ejemplo (descripción PR completa, rama sin ID de Jira)

**Título:** `docs- Refresh Object Composite API changelog`

```markdown
# Summary
Refreshes the changelog for the Object Composite API.

# Changes

## `CHANGELOG.md`
* Documents the latest OCAPI v4 constraint updates.

# Context

## Jira
No ticket
```
