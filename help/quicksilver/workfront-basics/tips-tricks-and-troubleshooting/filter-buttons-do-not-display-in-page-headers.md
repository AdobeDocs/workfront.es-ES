---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Los botones de filtro no se muestran en los encabezados de página
description: Lea este artículo para solucionar problemas relacionados con los botones de filtro que no se muestran en los encabezados de página.
feature: Get Started with Workfront
author: Lisa and Alina
exl-id: 327564ed-60df-441a-a38b-a17a8c57adb0
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
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
   <td> <p>[!UICONTROL System administrator]</p> </td> 
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
   <td><strong>[!DNL Adobe Workfront] area</strong></td> 
   <td><strong>Botones Filtro</strong></td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Proyectos] </p> </td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Proyectos en los que estoy activado]</p> </li> 
     <li> <p>[!UICONTROL Proyectos que tengo]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><span>[!UICONTROL Hojas de horas]</span> </td> 
   <td> 
    <ul> 
     <li> <p><span>[!UICONTROL Mis aprobaciones de parte de horas]</span> </p> </li> 
     <li> <p><span>[!UICONTROL Mis HOJAS]</span> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Solución

Los botones de filtro de la sección [!UICONTROL Proyectos y hojas de tiempo] no se muestran porque los filtros correspondientes no se incluyen en la plantilla de diseño aplicada al usuario. La variable [!DNL Workfront] el administrador debe asignar una plantilla de diseño que incluya los filtros.

>[!NOTE]
>
>A veces, los filtros se eliminan del [!UICONTROL Controles de lista] área [!UICONTROL Configuración]. La variable [!DNL Workfront] El administrador debe incluirlos en las listas de esta área para que estén disponibles en las plantillas de diseño.

1. Compruebe que la plantilla de diseño muestra los filtros siguientes:

   * [!UICONTROL Proyectos en los que estoy] y [!UICONTROL Proyectos de los que soy propietario] en el [!UICONTROL Proyectos] area
   * [!UICONTROL Aprobaciones de Mi parte de horas] y [!UICONTROL Mis hojas de hora] en el [!UICONTROL Hoja de horas] area

   Para ello:

   1. Acceda a la plantilla de diseño.
   1. Select **[!UICONTROL Listas]** under **[!UICONTROL Personalización de lo que ven los usuarios]**.
   1. Select **[!UICONTROL Proyectos]** o **[!UICONTROL Hojas de tiempo]** under **[!UICONTROL Seleccione una lista para personalizar]**.
   1. En el **[!UICONTROL Filtro]** , compruebe que **[!UICONTROL Proyectos en los que estoy]**, **[!UICONTROL Proyectos de los que soy propietario]** (para proyectos) y **[!UICONTROL Aprobaciones de Mi parte de horas]** y **[!UICONTROL Mis hojas de hora]** (para hojas de horas).
   1. Haga clic en **[!UICONTROL Guardar]**.

   Para obtener más información, consulte [Personalización de filtros, vistas y grupos mediante una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. Asigne la plantilla de diseño a los usuarios, funciones de trabajo, equipos o grupos correctos. Para obtener más información, consulte [Asignar usuarios a una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).
