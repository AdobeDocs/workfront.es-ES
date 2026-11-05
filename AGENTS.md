---
source-git-commit: 59deddd679267d10059f19cfd2d86b164903500e
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%
---
# AGENTS.md

Directrices del agente para el repositorio **workfront.en** (Adobe Workfront español)
documentación). Este archivo apunta a las instrucciones canónicas para que cualquier agente —
independientemente del archivo de convención que lea, sigue las mismas reglas.

## Archivos de instrucciones canónicas

- **Reglas de todo el repositorio**: [.github/copilot-instructions.md](.github/copilot-instructions.md)
— formatos de búsqueda de candidatos a artículos, propuesta antes de edición, mensaje de compromiso y PR,
y &quot;rellenar los huecos de forma inteligente&quot;.
- **Estándares de escritura** (se aplica automáticamente a `help/**/*.md`):
  [.github/instructions/writing-quality.instructions.md](.github/instructions/writing-quality.instructions.md),
con todos los detalles en
  [.cursor/skills/writing-quality/reference.md](.cursor/skills/writing-quality/reference.md).
- **Notas de la versión** (se aplica automáticamente a `product-announcements/product-releases/**`):
  [.github/instructions/release-notes-formatter.instructions.md](.github/instructions/release-notes-formatter.instructions.md).
- **Limpieza con resaltado previo** (flujo de trabajo bajo demanda):
  [.github/prompts/remove-preview-highlighting.prompt.md](.github/prompts/remove-preview-highlighting.prompt.md).

## Comportamientos no negociables

1. **Busque artículos candidatos antes de crear otros nuevos.** Cuando llega nuevo contenido
en, busque `help/` y vea una lista clasificada de los artículos existentes que le pueden interesar,
a continuación, pregunte a dónde pertenece antes de redactar el borrador.
2. **Proponer cambios antes de editar cualquier artículo de ayuda `.md`.** Mostrar los proyectos propuestos
diff y esperar aprobación explícita. La única excepción es cuando digo &quot;sólo arregla
it&quot; o &quot;don&#39;t ask, just edit&quot; en el mismo turno. Investigación de solo lectura y chat
los borradores siempre están bien.
3. **Rellene los huecos de forma inteligente.** Cuando la intención sea clara, comprometerse con el
las prácticas recomendadas responden y coinciden con los encabezados del artículo circundante,
terminología y estructura en lugar de presentar menús de opciones.
4. **Aplicar los estándares de escritura de forma proactiva** en cada edición de `help/`; no espere
para que se le recuerde.

## Convenciones de compromiso y PR

Consulte [.github/copilot-instructions.md](.github/copilot-instructions.md) para obtener la información completa
formato de mensaje de confirmación (asunto obligatorio ≤ ~50 caracteres; 📖 para adiciones, ✏️ para
modificaciones) y estructura PR (ID de Jira a partir del nombre de la rama; `# Summary`,
`# Changes` por archivo, `# Context` → `## Jira`).
