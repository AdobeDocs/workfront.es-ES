---
product-area: projects
navigation-topic: issue-information
title: Usar "opTask" y "issue" al hacer referencia a problemas
description: El nombre de un problema aparece como opTask en la base de datos de Adobe Workfront. Aunque hay ocasiones en que necesita utilizar el nombre del campo del problema para hacer referencia a problemas, la mayoría de las veces debe utilizar el nombre del campo opTask en lugar del problema al hacer referencia a problemas.
author: Alina
feature: Work Management
exl-id: 91107c04-616c-49b2-aa78-10e373d11f6b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/jrNMdSfyMO3MgzcxxKSNtrgzuY3e4ZNJpJ-JdvylJN4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 257
ht-degree: 95%

---

# Utilice “opTask” y “issue” al hacer referencia a problemas

<!--Audited: 08/2025-->

El nombre de un problema aparece como `opTask` en la base de datos de Adobe Workfront. Aunque hay ocasiones en las que necesita usar el nombre de campo `issue` para hacer referencia a problemas, la mayoría de las veces debe usar el nombre de campo `opTask` en lugar de `issue` al hacer referencia a problemas.

Para obtener más información sobre cómo aparecen los objetos en la base de datos de Workfront, consulte el [Explorador de API](https://developer.adobe.com/workfront/api-explorer/).

## `opTask` nombre de campo

Utilice el nombre de campo `opTask` al hacer referencia a problemas en los siguientes contextos:

* Cuando crea un informe personalizado en modo texto para problemas y desea hacer referencia a ellos en vistas, filtros, agrupaciones o peticiones de datos.

  Para obtener más información acerca del uso del modo de texto en un informe, consulte [Información general sobre el modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

<!--
* When you pull information about issues using our API.  
  For more information about the Workfront API, see [Adobe Workfront API](../../../wf-api/workfront-api.md)
  -->

* Cuando se actualizan los campos del problema en una hoja del importador de datos de KickStart.

  Para obtener más información sobre cómo importar datos en Workfront mediante una plantilla de KickStart, consulte [Importar datos a Adobe Workfront mediante una plantilla de KickStart](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## `issue` nombre de campo

Utilice el nombre de campo `issue` para hacer referencia a problemas en los siguientes contextos:

* Cuando se hace referencia a problemas en una colección mediante el modo de texto en un informe.
* Cuando se hace referencia a una colección de problemas mediante la API de Workfront.

Para obtener información acerca de cómo informar sobre colecciones, consulte [Colecciones de referencia en un informe](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

<!--
<note type="tip">
For information about how issues appear in a collection, see the
<a href="https://developer.adobe.com/workfront/api-explorer/" target="_blank">API Explorer</a> and select the API Unsupported option from the upper-right corner of the page.
<br>(NOTE: Drafted because this might not be needed.)
</note>
-->
