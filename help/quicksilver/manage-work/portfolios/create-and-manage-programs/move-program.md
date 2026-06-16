---
product-area: programs
navigation-topic: create and manage programs
title: Agregar un programa existente a un Portfolio
description: Puede añadir programas existentes a un portafolio. Como los programas no pueden existir en dos portafolios diferentes, al añadir un programa existente se mueve permanentemente de un portafolio a otro.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 73dbe277-12d2-4041-8a02-91ccf5f8b465
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/LkyWuPHqv0muTinWZT1PMKPGUNErWulIIxHmXVtPIVg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 397e5e36632872bb7be3f4e219b36e33b44136e9
workflow-type: tm+mt
source-wordcount: 289
ht-degree: 48%

---

# Añadir un programa existente a un portafolio

<!--Audited: 05/2026-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release. </span>   

<span class="preview">For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). </span>
-->

Puede añadir programas existentes a un portafolio. Como los programas no pueden existir en dos portafolios diferentes, al añadir un programa existente se mueve permanentemente de un portafolio a otro.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] paquete</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td> <p>[!UICONTROL Standard]</p><p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de [!UICONTROL Edit] a [!UICONTROL Portafolios] y [!UICONTROL Programas] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>[!UICONTROL Manage] permisos para el portafolio y el programa</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>New: [!UICONTROL Standard] </p><p>Or </p><p>Current: [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL Edit] access to Portfolios and Programs </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] permissions to the portfolio and the program</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## Añadir un programa existente a un portafolio

>[!NOTE]
>
>Cuando su organización utiliza el almacenamiento en la nube heredado de Workfront y Adobe para documentos, no puede agregar un programa de almacenamiento en la nube de Adobe a un portafolio de almacenamiento heredado ni un programa heredado a un portafolio de almacenamiento en la nube de Adobe.
>Es posible que la instancia de Workfront no tenga ambos tipos de almacenamiento de documentos.
>Para obtener más información, consulte [Resumen de administración de documentos para proyectos y objetos relacionados](/help/quicksilver/manage-work/projects/manage-projects/manage-documents-on-projects.md).
>

Para agregar un programa existente a otro portafolio:

1. Vaya a un portafolio y, a continuación, haga clic en **[!UICONTROL Programas]** en el panel izquierdo.
1. Haga clic en **[!UICONTROL Nuevo programa]**.
1. Haga clic en **[!UICONTROL Existing Program]**.

   Se abre el cuadro **Agregar programas**. <!--check screen shot - I logged changes for this casing-->

   ![Agregar cuadro de programa](assets/add-programs-box.png)

   >[!IMPORTANT]
   >
   >Añadir un programa existente implica llevar todos los proyectos asociados con ese programa al portafolio. Tenga cuidado de no mover proyectos de esta manera sin querer.

1. En el campo **[!UICONTROL Agregar programas a este portafolio]**, escriba el nombre de un programa y selecciónelo cuando se muestre en la lista. <!--see the name of this field, I suggested changes here-->

   Puede agregar varios programas.

1. (Opcional) Si decide no agregarlo al portafolio, haga clic en el icono **Eliminar** ![Eliminar icono](assets/delete-icon.png) que está junto al nombre de un programa.

1. Haga clic en **[!UICONTROL Agregar programas]**.

   El programa se muestra en la ficha **[!UICONTROL Programas]** del portafolio que seleccionó.

