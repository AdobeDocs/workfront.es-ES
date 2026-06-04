---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ver: Informe de documento con vínculo a una prueba'
description: 'Vista: informe de documento con vínculo a una prueba'
author: Courtney
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/bRL7x0qjHQrwg-HfxtJcazG9GK0WifSsl13VL1K5hGs
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 306
ht-degree: 35%

---

# Vista: informe de documento con vínculo a una prueba

<!--Audited: 11/2024-->

En esta vista de documento, puede insertar un vínculo a una prueba de la versión actual del documento.

![Ver documento con vínculo de revisión](assets/view-document-with-proof-link-350x92.png)

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
   <p>Colaborador o solicitud para modificar un filtro </p>
   <p>Estándar o Plan para modificar un informe</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Informes, Paneles de control y Calendarios para modificar un informe</p> <p>Acceso de edición a filtros, vistas y agrupaciones para modificar un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración para un informe</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ver un informe de documento con un vínculo a una prueba

Para aplicar este vista:

1. Ir a una lista de documentos.
1. En el menú desplegable **Vista**, seleccione **Nueva vista**.
1. Haga clic en **Añadir columna**.
1. Haga clic en **Cambiar al modo de texto** y, a continuación, **Editar el modo de texto**.
1. Elimine el texto que encuentre en el cuadro **Editar modo de texto** y reemplácelo por el siguiente código:

   ```
   displayname=Proof Link
   shortview=true
   textmode=true
   valueexpression=CONCAT("https://Your domain.my.workfront.com/document/",{currentVersion}.{ID},"/proof/",{currentVersion}.{proofID},"/view")
   valueformat=HTML
   ```

   >[!TIP]
   >
   >Sustituya &quot;Su dominio&quot; por el dominio real de Workfront. Por ejemplo, si la dirección URL de Workfront de su compañía es *Company.my.workfront.com*, su dominio será &quot;Compañía&quot;.

1. Haga clic en **Listo** y luego en **Guardar vista**.
1. (Opcional) Actualice el nombre de la vista y, a continuación, haga clic en **Guardar vista**.
1. (Opcional) Para asegurarse de que solo se muestran los documentos con pruebas, agregue un filtro haciendo lo siguiente:

   1. Haga clic en el menú **Filtro** y seleccione **Nuevo filtro**.
   1. Haga clic en **Agregar una regla de filtro** y empiece a escribir &quot;Propietario de prueba&quot;, luego seleccione **Identificador de propietario de prueba** cuando se muestre en la lista.
   1. Seleccione **No está en blanco** para el modificador de filtro.
   1. Haga clic en **Guardar filtro**.
   1. (Opcional) Actualice el nombre del filtro y, a continuación, haga clic en **Guardar filtro**.

1. Haga clic en el vínculo de la columna Vínculo de prueba para acceder a la prueba de la última versión del documento.
