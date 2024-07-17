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
   <td role="rowheader"><strong>Licencia de Adobe [!DNL Workfront]</strong></td> 
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
     <li> <p><span>[!UICONTROL Mis aprobaciones de hoja de horas]</span> </p> </li> 
     <li> <p><span>[!UICONTROL Mis hojas de horas]</span> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Solución

Los botones de filtro del área [!UICONTROL Proyectos y hojas de horas] no se muestran porque los filtros correspondientes no están incluidos en la plantilla de diseño aplicada al usuario. El administrador de [!DNL Workfront] debe asignar una plantilla de diseño que incluya los filtros.

>[!NOTE]
>
>A veces, los filtros se eliminan del área [!UICONTROL Controles de lista] en [!UICONTROL Configuración]. El administrador de [!DNL Workfront] debe incluirlos en las listas de esta área para que estén disponibles en las plantillas de diseño.

1. Compruebe que la plantilla de diseño muestra los siguientes filtros:

   * [!UICONTROL Proyectos en los que participo] y [!UICONTROL Proyectos de mi propiedad] en el área de [!UICONTROL Proyectos]
   * [!UICONTROL Aprobaciones de mi hoja de horas] y [!UICONTROL Mis hojas de horas] en el área [!UICONTROL Hoja de horas]

   Para ello:

   1. Acceda a la plantilla de diseño.
   1. Seleccione **[!UICONTROL Listas]** en **[!UICONTROL Personalizar lo que ven los usuarios]**.
   1. Seleccione **[!UICONTROL Proyectos]** o **[!UICONTROL Plantillas de horas]** en **[!UICONTROL Seleccione una lista para personalizar]**.
   1. En la sección **[!UICONTROL Filtrar]**, verifique que **[!UICONTROL Proyectos en los que participo]**, **[!UICONTROL Proyectos de mi propiedad]** (para proyectos) y **[!UICONTROL Mis aprobaciones de hojas de horas]** y **[!UICONTROL Mis hojas de horas]** (para hojas de horas) estén seleccionadas.
   1. Haga clic en **[!UICONTROL Guardar]**.

   Para obtener más información, vea [Personalizar filtros, vistas y agrupaciones mediante una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. Asigne la plantilla de diseño a los usuarios, los roles, los equipos o los grupos correctos. Para obtener más información, consulte [Asignar usuarios a una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).
