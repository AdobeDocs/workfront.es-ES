---
mode: agent
description: 'Elimine los marcos de documentación solo de vista previa de Workfront para GA: previsualice fragmentos de plantillas, class="preview" de HTML y pasos o secciones paralelos en vista previa o en producción.'
source-git-commit: 59deddd679267d10059f19cfd2d86b164903500e
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 1%
---

# Quitar resaltado de vista previa

Ejecute este flujo de trabajo solo cuando pida &quot;eliminar el resaltado de vista previa&quot; (o claramente el
misma intención). Convierte procedimientos/referencias etiquetados previamente y creados por Courtney
Temas de en contenido compatible con GA.

## Ámbito

Se aplican solo cuando **all** son verdaderos:

1. He invocado este flujo de trabajo.
2. La ruta de acceso del archivo **no contiene** `product-announcements` (excluya todo el archivo
árbol: notas de la versión, beta, anuncios).
3. El archivo no aparece en la lista bajo **Rutas excluidas** a continuación.
4. La línea de asunto previo `author:` incluye **`Courtney`** (único o coautor).
5. El artículo contiene al menos uno de los siguientes elementos:
   - Previsualizar el lenguaje del entorno en prosa corporal o párrafos de fragmentos reales
     (&quot;información resaltada&quot;, &quot;Entorno de vista previa&quot;, &quot;aún no es habitual&quot;)
     disponibles&quot;, notas de la versión rápida) — **no** una coincidencia sólo del texto del vínculo en un
     TDC/página de índice;
   - Cualquier elemento HTML con `class="preview"` (`<span>`, `<div>`, `<p>`, `<li>`...);
   - Una variable de fragmento de vista previa, como `{{highlighted-preview}}` o
     `{{highlighted-preview-article-level}}`.

Si el ámbito no es claro, confirme antes de editar.

**páginas de índice/índice: omitir siempre** cuando la única redacción de vista previa está dentro de un
markdown link muestra texto que señala a otro artículo y el archivo no tiene
`class="preview"`, sin variables de fragmento y sin plantillas de vista previa en prosa
fuera de vínculos.

### Rutas excluidas

Nunca realizar el inventario ni editar estos elementos a menos que anule explícitamente:

- `help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/send-to-aem.md`
- `help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-manage-reports.md`

## Flujo de trabajo requerido (humano en bucle)

No realice ediciones masivas sin aprobación.

1. **Inventario**: genere una lista ordenada de rutas de acceso en el ámbito (busque `help/`). Omitir
   `product-announcements`, rutas excluidas y menciones solo de índice/índice.
2. **Inicio** — pregunte si desea comenzar con el primer artículo (o un nombre de ruta de acceso).
3. **Por artículo — mostrar primero, editar después de Aceptar** — leer el archivo, proponer ediciones como
antes o después de extractos o una comparación de diferencias enfocada; a continuación, espere a que se apruebe explícitamente.
4. **Después de cada archivo** — pregunte si desea pasar al siguiente (o detener/omitir).

## Reglas de contenido (la vista previa del contenido se convierte en el documento)

Objetivo: mantener el comportamiento documentado para la vista previa, dejar obsoleto &quot;en producción&quot;
ramas y, a continuación, eliminar etiquetas y contenedores de solo vista previa.

- **Pasos paralelos**: elimine el paso &quot;en producción&quot;; mantenga el paso &quot;en vista previa&quot;
es la sustancia del paso, pero vuelva a escribirlo para que no sea específico para la vista previa. Corrija la numeración. Si
no hay un paralelo claro, deténgase y pregunte qué bloque mantener.
- **Secciones paralelas**: quite la sección del entorno de producción; reemplácela
con el contenido de la sección previsualización, neutralice la redacción de la previsualización y elimine
  `class="preview"` contenedores.
- **Fragmentos y avisos sobre la parte superior del artículo**: quite las plantillas de solo vista previa y
frases cuyo único propósito es la disponibilidad de previsualización.
- **`class="preview"`**: quite las etiquetas de apertura y cierre, mantenga el contenido interno.
Conservar la estructura de listas/tablas; corregir listas rotas o espacios en blanco inactivos.
- **Secciones comentadas (`<!-- … -->`)**: no modificar a menos que se especifique explícitamente
Díganlo... Si el contenido de la vista previa solo aparece dentro de los comentarios, llame a él y pregunte.
Predeterminado: dejar los comentarios sin modificar.

## No hacer

- Ejecutar en `product-announcements` rutas o rutas excluidas.
- Editar automáticamente bloques comentados.
- Elimine &quot;Vista previa&quot; cuando sea un nombre de producto en un contexto no relacionado (por ejemplo, Vista previa
Entorno de zona protegida) — pregunte si no está seguro.
- Cambiar `author:` o frontmatter no relacionado.
- Omita el paso mostrar → aprobar.

## Comprobación de la calidad antes de presentar las ediciones

- No quedan `class="preview"` en el ámbito acordado.
- No hay encabezados duplicados huérfanos ni números de paso rotos.
- La introducción se lee correctamente para GA (no &quot;solo en vista previa&quot; para las funciones enviadas).
