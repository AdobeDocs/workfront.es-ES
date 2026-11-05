---
source-git-commit: 59deddd679267d10059f19cfd2d86b164903500e
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 1%
---
# Instrucciones de copiloto para workfront.en

Este repositorio contiene la documentación en inglés de Adobe Workfront. Las reglas
a continuación, se aplican a todas las solicitudes de esta área de trabajo. Los estándares específicos por temas se aplican en
`.github/instructions/*.instructions.md` y se cargarán automáticamente al editar
archivos coincidentes.

## Busque artículos candidatos antes de crear nuevos artículos

Cuando llega contenido nuevo: un documento de admisión, comentarios del cliente o del administrador de proyectos, un
Slack/transcripción, capturas de pantalla con notas o preguntas de soporte técnico: **no
propone crear primero un nuevo artículo.** Buscar el repositorio y el candidato de superficie
artículos existentes en los que el contenido pueda caber.

Flujo de trabajo requerido:

1. **Primero lea el nuevo contenido** para identificar el tema, la audiencia (administrador vs. fin)
usuario) y los hechos o pasos específicos que añade.
2. **Busque `help/` candidatos** usando grep y la búsqueda de archivos. Buscar:
artículos que ya cubren la misma función, área o flujo de trabajo.
3. **Devuelve una lista clasificada** de artículos candidatos (normalmente de 3 a 7), cada uno con:
   - La ruta del archivo (como vínculo en el que puede hacer clic).
   - Una razón de una línea es un candidato (en qué sección se ubicaría o por qué)
     es la coincidencia tópica más cercana).
   - Cualquier advertencia (por ejemplo, &quot;Discrepancia de audiencia&quot;, si se trata del usuario final, la admisión es
     de cara a la administración&quot;).
4. **Pregunte dónde colocarlo** antes de redactar el borrador o editar. Escriba la pregunta
explícitamente, por ejemplo &quot;¿En cuál de ellos debo reclutar?&quot; o &quot;Quiero que lo haga&quot;
encajarlo en #2, o crees que necesita su propio artículo?&quot;
5. **Solo sugerir un nuevo artículo** si ningún artículo existente es razonable, y
explique por qué ninguno de los candidatos trabaja.

Incluso si el contenido &quot;obviamente&quot; pertenece a un artículo conocido, sigue apareciendo 2-3
alternativas para confirmar la ubicación. Esto detecta cuasi duplicados y
lugares en los que el contenido ya estaba parcialmente cubierto.

## Proponer cambios antes de editar artículos de ayuda

Cuando esté a punto de editar un artículo de ayuda de `.md` en `help/`, **no edite el archivo
aún.** Primero, muestre lo que planea cambiar y espere una aprobación explícita.

Para cada archivo que desee tocar:

1. Asigne un nombre al archivo (ruta).
2. Mostrar el cambio propuesto como una diferencia o un fragmento delimitado (texto antiguo y texto nuevo)
con suficiente contexto para ser inequívoco.
3. Exponga brevemente la razón (una frase).
4. Finalice con una tarea explícita como, por ejemplo, &quot;¿Aplicar estos cambios?&quot; o &quot;Quiero que lo haga&quot;
¿continuar?&quot;

Solo después de una aprobación explícita (&quot;sí&quot;, &quot;ir&quot;, &quot;aplicar&quot;, &quot;hacerlo&quot;, etc.) ¿debería
llame a las herramientas de edición.

Esto se aplica a **cada** edición en un artículo de `.md` de ayuda: errores tipográficos, correcciones de vínculos,
cambios de una sola palabra, limpiezas terminológicas, nuevas secciones y reescrituras. No
excepciones a menos que el usuario indique explícitamente &quot;simplemente corríjalo&quot; o &quot;no preguntes, solo
editar&quot; en el mismo turno.

Para los cambios que abarcan varios artículos, agrupe las diferencias propuestas por archivo en
una respuesta. Si el conjunto es grande, enumere primero los archivos afectados con un resumen de una línea
a continuación, muestre las diferencias en los lotes y confirme antes de cada lote.

Esto **no** bloquea la investigación de solo lectura (grep, read) o el dibujo/exploración
en el chat (sin escritura de archivos).

## Rellenar los huecos de forma inteligente

Cuando la intención sea clara desde el contexto, confíe en la respuesta de prácticas recomendadas en lugar de
presentación de menús de opciones. Aplicar los estándares de escritura (consulte
`.github/instructions/writing-quality.instructions.md`) de forma proactiva: no esperar
que se le recuerde que debe seguirlos. Hacer coincidir el texto nuevo con el del artículo adyacente
encabezados, terminología y estructura. Solo pregunte cuando una ambigüedad genuina
cambiar el resultado.

## Mensajes de confirmación de Git

### Línea de asunto

- Alrededor de **50 caracteres o menos**.
- Resuma el cambio en **estado de ánimo imperativo** (&quot;Agregar...&quot;, &quot;Corregir...&quot;, &quot;Refactorizar...&quot;).

### Cuerpo

- Deje una línea en blanco después del asunto antes del cuerpo.
- Ajustar líneas a **72 caracteres** aproximadamente.
- Utilice **líneas de viñetas** para la explicación. Cada viñeta debe comenzar con exactamente
uno de:
  - **📖** — cuando el cambio **agrega** algo nuevo: nuevos archivos, nuevas secciones, nuevo
    funciones, encabezados nuevos, líneas nuevas u otro contenido sin formato.
  - **✏️** — cuando el cambio **modifica** trabajo existente: edita a líneas existentes,
    actualizaciones de secciones existentes, refactores o cambios en el contenido actual.

Ejemplo:

```
Add refresh token rotation to auth flow

- 📖 Add refresh_tokens table and Alembic migration for schema v3.
- ✏️ Update session middleware to rotate secrets and revoke old tokens.
```

## Solicitudes de extracción

### Derivación del problema Jira

- Derive el ID del problema Jira del **nombre actual de la rama Git** (por ejemplo, un
coincidencia de segmento `FFENT-8796`).
- **Si el nombre de la sucursal incluye un ID de Jira:**, use ese ID en el título y el vínculo de PR
lo cambió en `# Context` → `## Jira`.
- **Si el nombre de la rama no incluye un identificador Jira:**, omita la clave Jira de la PR
título. Sigue incluyendo `## Jira` con exactamente `No ticket`.

### Título de PR

- **Con Id. Jira:** `{type}/{JIRA-ID}- {short task description}`
  - Ejemplo: `feat/FFENT-8001- Add validation for numVariations in OCAPI request`
- **Sin ID de Jira:** `{type}- {short task description}`
  - Ejemplo: `docs- Refresh Object Composite API changelog`

Tipos de confirmación: **feat** (nueva característica), **corrección** (corrección de errores), **refactorización** (reestructuración)
sin cambio de comportamiento), **perf** (rendimiento), **style** (solo formato),
**prueba** (pruebas), **documentos** (solo documentación, contenido nuevo), **compilación** (compilación/CI/
dependencias), **ops** (infraestructura/implementación), **chore** (varios).

### PR body — secciones requeridas

- `# Summary`: breve descripción de qué ha cambiado y por qué.
- `# Changes` — organizado por archivo. Para cada archivo tocado, utilice un encabezado de nivel 2
con la trayectoria en acentos graves y, a continuación, puntos de viñeta.
- `# Context` — incluir siempre una subsección `## Jira` con el problema vinculado, o
  `No ticket`.

```markdown
# Changes

## `path/to/file.ext`
* Concise bullet describing the change in that file.

# Context

## Jira
[FFENT-8796](https://jira.corp.adobe.com/browse/FFENT-8796)
```
