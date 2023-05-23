---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Los botones de filtro no se muestran en los encabezados de página
description: Lea este artículo para solucionar problemas con los botones de filtro que no se muestran en los encabezados de página.
feature: Get Started with Workfront
author: Nolan and Alina
exl-id: 327564ed-60df-441a-a38b-a17a8c57adb0
source-git-commit: 114d306d99ae9ba0a18abd63a6137ad0568ab202
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 1%

---

# Los botones de filtro no se muestran en los encabezados de página

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] licencia</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso</strong></td> 
   <td> <p>[!UICONTROL Administrador del sistema]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Problema

Los siguientes botones de filtro no se muestran en sus áreas respectivas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>[!DNL Adobe Workfront] área</strong></td> 
   <td><strong>Botones de filtro</strong></td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Proyectos] </p> </td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Proyectos en los que participo]</p> </li> 
     <li> <p>[!UICONTROL Proyectos de mi propiedad]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><span>[!UICONTROL Plantillas de horas]</span> </td> 
   <td> 
    <ul> 
     <li> <p><span>[!UICONTROL Mis aprobaciones de hojas de horas]</span> </p> </li> 
     <li> <p><span>[!UICONTROL Mis hojas de horas]</span> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Solución

Los botones de filtro del [!UICONTROL Proyectos y hojas de horas] no se muestran porque los filtros correspondientes no están incluidos en la plantilla de diseño aplicada al usuario. El [!DNL Workfront] El administrador debe asignar una plantilla de diseño que incluya los filtros.

>[!NOTE]
>
>A veces, los filtros se eliminan del [!UICONTROL Controles de lista] área en [!UICONTROL Configurar]. El [!DNL Workfront] El administrador de debe incluirlos en las listas de esta área para que estén disponibles en las plantillas de diseño.

1. Compruebe que la plantilla de diseño muestra los siguientes filtros:

   * [!UICONTROL Proyectos en los que trabajo] y [!UICONTROL Proyectos de mi propiedad] en el [!UICONTROL Proyectos] área
   * [!UICONTROL Mis aprobaciones de hojas de horas] y [!UICONTROL Mis hojas de horas] en el [!UICONTROL Hoja de horas] área

   Para ello:

   1. Acceda a la plantilla de diseño.
   1. Seleccionar **[!UICONTROL Listas]** bajo **[!UICONTROL Personalizar lo que ven los usuarios]**.
   1. Seleccionar **[!UICONTROL Proyectos]** o **[!UICONTROL Plantillas de horas]** bajo **[!UICONTROL Seleccione una lista para personalizar]**.
   1. En el **[!UICONTROL Filtrar]** , compruebe que **[!UICONTROL Proyectos en los que trabajo]**, **[!UICONTROL Proyectos de mi propiedad]** (para proyectos) y **[!UICONTROL Mis aprobaciones de hojas de horas]** y **[!UICONTROL Mis hojas de horas]** (en el caso de las plantillas de horas).
   1. Haga clic en **[!UICONTROL Guardar]**.

   Para obtener más información, consulte [Personalización de filtros, vistas y agrupaciones mediante una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. Asigne la plantilla de diseño a los usuarios, los roles, los equipos o los grupos correctos. Para obtener más información, consulte [Asignar usuarios a una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).
