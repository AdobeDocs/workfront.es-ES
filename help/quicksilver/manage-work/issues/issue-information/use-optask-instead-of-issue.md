---
product-area: projects
navigation-topic: issue-information
title: Utilice "opTask" y "issue" al hacer referencia a problemas
description: El nombre de un problema aparece como opTask en la base de datos de Adobe Workfront. Aunque hay ocasiones en que necesita utilizar el nombre del campo de problema para hacer referencia a problemas, la mayoría de las veces debe utilizar el nombre del campo opTask en lugar de problema al hacer referencia a problemas.
author: Alina
feature: Work Management
exl-id: 91107c04-616c-49b2-aa78-10e373d11f6b
source-git-commit: 813b97ee0979e29a90293d9ddaba12a33c99f64d
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---

# Utilice &quot;opTask&quot; y &quot;issue&quot; al hacer referencia a problemas

El nombre de un problema aparece como `opTask` en la base de datos de Adobe Workfront. Aunque hay ocasiones en las que necesita utilizar la variable `issue` nombre del campo para hacer referencia a problemas, la mayoría de las veces debe utilizar la variable `opTask` nombre de campo en lugar de `issue` al hacer referencia a problemas.

Para obtener más información sobre cómo aparecen los objetos en la base de datos de Workfront, consulte la [Explorador de API](https://developer.adobe.com/workfront/api-explorer/).

## `opTask` filename

Utilice el `opTask` nombre del campo al hacer referencia a problemas en los siguientes contextos:

* Cuando crea un informe personalizado en modo texto para problemas y desea hacer referencia a ellos en vistas, filtros, agrupaciones o peticiones de datos.

   Para obtener más información sobre el uso del modo de texto en un informe, consulte [Introducción al modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

<!--* When you pull information about issues using our API.  
  For more information about the Workfront API, see [Adobe Workfront API](../../../wf-api/workfront-api.md)-->

* Cuando se actualizan los campos de problema en una hoja del importador de datos de KickStart.

   Para obtener más información sobre cómo importar datos en Workfront mediante un KickStart, consulte [Importación de datos en Adobe Workfront mediante una plantilla de KickStart](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## `issue` nombre de campo

Utilice el `issue` nombre del campo para hacer referencia a problemas en los siguientes contextos:

* Cuando se hace referencia a problemas en una colección mediante el modo de texto en un informe.
* Cuando se hace referencia a una colección de problemas mediante la API de Workfront.

Para obtener información sobre los informes de colecciones, consulte [Colecciones de referencia en un informe](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

<!--
<note type="tip">
For information about how issues appear in a collection, see the
<a href="https://developer.adobe.com/workfront/api-explorer/" target="_blank">API Explorer</a> and select the API Unsupported option from the upper-right corner of the page.
<br>(NOTE: Drafted because this might not be needed.)
</note>
-->
