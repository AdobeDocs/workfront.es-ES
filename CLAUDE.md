---
source-git-commit: 44629631cd2d99eadbed5fd81cf33458b13702af
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---
# Busque artículos candidatos antes de crear nuevos artículos

Cuando Courtney trae nuevo contenido para incorporar: un documento de admisión, comentarios del cliente o del PM, una pegatina de Slack/transcripción, capturas de pantalla con notas y preguntas de soporte técnico, **no se propone crear un nuevo artículo primero.** Busque en el repositorio y busque los artículos existentes en los que pueda caber el contenido.

## Flujo de trabajo obligatorio

1. **Lea primero el nuevo contenido** para identificar el tema, la audiencia (administrador frente a usuario final) y los hechos o pasos específicos que agrega.
2. **Busque `help/` candidatos** usando grep y find. Busque artículos que ya cubran la misma función, área o flujo de trabajo.
3. **Devuelve una lista clasificada** de artículos candidatos (normalmente de 3 a 7), cada uno con:
   - La ruta del archivo (ruta de acento grave en la que se puede hacer clic).
   - Una razón de 1 línea es un candidato (en qué sección se ubicaría o por qué es la coincidencia tópica más cercana).
   - Cualquier advertencia (por ejemplo, &quot;Discrepancia de audiencia: se trata del usuario final, la entrada es de administración&quot;).
4. **Pregunta a Courtney dónde ponerlo** antes de redactar un borrador o editar. Escriba la pregunta de forma explícita, por ejemplo, &quot;¿En cuál de estas debería redactar?&quot; o &quot;¿Quieres que lo encaje en #2, o crees que necesita su propio artículo?&quot;
5. **Solo sugiere un nuevo artículo** si ningún artículo existente es razonable y explica por qué ninguno de los candidatos funciona.

Incluso si el contenido &quot;obviamente&quot; pertenece a un artículo conocido, aún aparecen 2-3 alternativas para que Courtney pueda confirmar la ubicación. Esto detecta cuasi duplicados y lugares donde el contenido ya estaba parcialmente cubierto.

---

# Proponer cambios antes de editar artículos de ayuda

Cuando esté a punto de editar cualquier artículo de ayuda de `.md` en `help/`, **no edite el archivo aún**. Primero, muestre lo que planea cambiar y espere una aprobación explícita.

Para cada archivo que desee tocar:

1. Asigne un nombre al archivo (ruta).
2. Muestre el cambio propuesto como una diferencia/fragmento delimitado (texto antiguo y texto nuevo) con suficiente contexto para ser inequívoco.
3. Exponga brevemente la razón (1 frase).
4. Finalice con una tarea explícita como, por ejemplo, &quot;¿Aplicar estos cambios?&quot; o &quot;¿Quiere que continúe?&quot;

Solo después de que Courtney diga que sí (o &quot;ir&quot;, &quot;aplicar&quot;, &quot;hacerlo&quot;, etc.) debería llamar a las herramientas de edición.

Esto se aplica a **cada** edición en un artículo de `.md` de ayuda: errores tipográficos, correcciones de vínculos, cambios de una sola palabra, limpiezas terminológicas, nuevas secciones y reescrituras. No hay excepciones a menos que Courtney diga explícitamente &quot;solo arreglalo&quot; o &quot;no preguntes, solo edita&quot; en el mismo turno.

Para cambios que abarcan varios artículos: agrupe las diferencias propuestas por archivo en una respuesta. Si el conjunto es grande, primero enumere los archivos afectados con un resumen de 1 línea cada uno y, a continuación, muestre las diferencias por lotes y confirme antes de cada lote.

Esto hace que **no** bloquee la búsqueda de solo lectura (grep, read) o el dibujo/exploración en el chat (sin escritura de archivos).

---

# Mensajes de confirmación de Git

Al redactar o generar un mensaje de confirmación de Git, siga este formato.

## Línea de asunto

- Alrededor de **50 caracteres o menos**.
- Resuma el cambio en **estado de ánimo imperativo** (por ejemplo, &quot;Agregar...&quot;, &quot;Corregir...&quot;, &quot;Refactorizar...&quot;).

## Cuerpo

- Deje una línea en blanco después del asunto antes del cuerpo.
- Ajustar líneas a **72 caracteres** aproximadamente.
- Utilice **líneas de viñetas** para la explicación. Cada viñeta debe comenzar exactamente con una de:
   - **📖** — usar cuando el cambio **agregue** algo nuevo: nuevos archivos, nuevas secciones, nuevas características, nuevos encabezados, nuevas líneas u otro contenido de tipo &quot;greenfield&quot;.
   - **✏️** — usar cuando el cambio **modifica** trabajo existente: edita las líneas existentes, actualiza las secciones existentes, refactoriza o cambia el contenido actual.

Ejemplo:

```
Add refresh token rotation to auth flow

- 📖 Add refresh_tokens table and Alembic migration for schema v3.
- ✏️ Update session middleware to rotate secrets and revoke old tokens.
```

---

# Solicitudes de extracción (PR)

## Derivación del problema Jira

- Derive el ID del problema Jira del **nombre de la rama Git actual** (por ejemplo, un segmento que coincida con `FFENT-8796`).
- **Si el nombre de la rama incluye un ID de Jira:** Use ese ID en el título de PR y vincúlelo en `# Context` → `## Jira`.
- **Si el nombre de la rama no incluye un identificador Jira:** Omita la clave Jira del título PR. Sigue incluyendo `## Jira` con exactamente: `No ticket`.

## Título de PR

**Con Id. Jira:** `{type}/{JIRA-ID}- {short task description}`
Ejemplo: `feat/FFENT-8001- Add validation for numVariations in OCAPI request`

**Sin ID. de Jira:** `{type}- {short task description}`
Ejemplo: `docs- Refresh Object Composite API changelog`

### Tipos de compromiso

- **feat** — agrega una nueva característica
- **corregir** — corrige un error
- **refactor** — reescribe/reestructura el código sin cambiar el comportamiento
- **perf** — mejora el rendimiento
- **style**: solo formato/espacio en blanco; sin cambio de significado
- **prueba** — agrega o corrige pruebas
- **documentos** — solo documentación, contenido nuevo agregado
- **versión**: herramientas de compilación, CI, dependencias, versión del proyecto
- **ops**: infraestructura, implementación, copia de seguridad, recuperación
- **tarea** — varias (p. ej. `.gitignore`)

## PR body — secciones requeridas

### `# Summary`
Breve descripción de lo que ha cambiado y por qué.

### `# Changes`
Organizado por archivo. Para cada archivo tocado, utilice un encabezado de nivel 2 con la ruta en acentos graves y luego puntos de viñeta.

```markdown
# Changes

## `path/to/file.ext`
* Concise bullet describing the change in that file.
```

### `# Context`
Incluya siempre una subsección `## Jira`.

```markdown
# Context

## Jira
[FFENT-8796](https://jira.corp.adobe.com/browse/FFENT-8796)
```

O si no hay ticket: `No ticket`
