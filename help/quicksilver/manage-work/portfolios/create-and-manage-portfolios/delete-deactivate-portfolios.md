---
product-area: portfolios
navigation-topic: create-and-manage-portfolios
title: Eliminar y desactivar portafolios
description: Los portafolios son colecciones de proyectos o programas de Adobe Workfront. Puede eliminar o desactivar un portafolio si descubre que es irrelevante para su sistema.
author: Alina
feature: Work Management, Strategic Planning
exl-id: f88669d2-e8e9-4905-a771-1427b1fd32b2
source-git-commit: 03c1f17504846fc4b8c4114ddc32df687281bc07
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 12%

---

# Eliminar y desactivar portafolios

<!--Audited: 2/2024-->

Los portafolios son colecciones de proyectos o programas de [!DNL Adobe Workfront]. Puede eliminar o desactivar un portafolio si descubre que es irrelevante para su sistema.

Se recomienda desactivar un portafolio que ya no necesite asociarse con proyectos futuros en lugar de eliminarlo, para mantener la información histórica de los proyectos que están asociados actualmente con el portafolio y sus programas.

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td> <p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso [!UICONTROL Edit] a proyectos y portafolio</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de [!UICONTROL Manage] en el portafolio </p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Información general sobre la eliminación y desactivación de portafolios

Tenga en cuenta lo siguiente a la hora de decidir si elimina o desactiva portafolios:

* Al eliminar un portafolio, se eliminan los programas asociados a él.

  >[!IMPORTANT]
  >
  >No es necesario tener permisos en los programas para poder eliminar el portafolio.

* Al eliminar un portafolio, no se eliminan los proyectos asociados a él.
* No puede recuperar los portafolios eliminados.
* La desactivación de un portafolio garantiza que el nombre del portafolio y sus programas ya no se puedan asignar a proyectos al crear un proyecto.
* Al desactivar un portafolio que ya está adjunto a un proyecto, no se elimina del proyecto. Si elimina un portafolio desactivado de un proyecto, debe reactivarlo para poder volver a adjuntarlo al proyecto.

## Eliminar un portafolio

{{step1-to-portfolios}}

1. Realice una de las siguientes acciones:

   * Seleccione el portafolio en la lista y luego haga clic en el icono **[!UICONTROL Eliminar]** ![Eliminar icono](assets/delete.png).
   * Haga clic en el portafolio para abrirlo y, a continuación, haga clic en el menú **Más** ![Menú más](assets/more-icon.png) a la derecha del nombre del portafolio y, a continuación, en **Eliminar Portfolio**.
1. Haga clic en **[!UICONTROL Sí, eliminarlo]** para confirmar.

   El portafolio se elimina y no se puede recuperar.

## Desactivar un portafolio

Cuando desactiva un portafolio, aún puede acceder a él desde el área de [!UICONTROL Portafolios], pero ya no se muestra en la lista de portafolios cuando los usuarios intentan agregarlo a un proyecto.

>[!NOTE]
>
>Según la forma en que el administrador de grupo o [!DNL Workfront] configure la plantilla de diseño, es posible que el área [!UICONTROL Portafolios] no se muestre en el [!UICONTROL Menú principal]. Para obtener más información, consulte [Personalizar el menú principal con una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

{{step1-click-main-menu}}

1. Haga clic en **[!UICONTROL Portafolios]** .
1. Haga clic en el nombre del portafolio.
1. Haga clic en el menú **Más** ![Menú más](assets/more-icon.png) que se encuentra a la derecha del nombre del portafolio y, a continuación, haga clic en **[!UICONTROL Desactivar Portfolio]**.
El portafolio se desactiva inmediatamente.
1. (Opcional) Haga clic en el menú **Más** ![Menú más](assets/more-icon.png) que se encuentra a la derecha del nombre del portafolio y, a continuación, haga clic en **[!UICONTROL Activar Portfolio]** para reactivarlo.


