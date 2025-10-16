---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Los botones de filtro no se muestran en los encabezados de página
description: Lea este artículo para solucionar problemas con los botones de filtro que no se muestran en los encabezados de página.
feature: Get Started with Workfront
author: Nolan and Alina
exl-id: 327564ed-60df-441a-a38b-a17a8c57adb0
source-git-commit: 85ccee879fd4ba5a80b6e885458839901f83d26e
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 97%

---

# Los botones de filtro no se muestran en los encabezados de página

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table>
  <tr>
   <td>paquete de Adobe Workfront
   </td>
   <td> <p>PRIME o ULTIMATE</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr>
  <tr>
   <td>Licencias de Adobe Workfront
   </td>
   <td><p>Estándar</p>
   <p>Plan</p>
   </td>
  </tr>
   <tr>
   <td>Configuraciones de nivel de acceso
   </td>
   <td>Debe ser administrador de [!DNL Workfront].
   </td>
  </tr>
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   <td> <p>[!UICONTROL Projects] </p> </td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects I'm On]</p> </li> 
     <li> <p>[!UICONTROL Projects I Own]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><span>[!UICONTROL Timesheets]</span> </td> 
   <td> 
    <ul> 
     <li> <p><span>[!UICONTROL My Timesheet Approvals]</span> </p> </li> 
     <li> <p><span>[!UICONTROL My Timesheets]</span> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Solución

Los botones de filtro del área [!UICONTROL Proyectos y plantillas de horas] no se muestran porque los filtros correspondientes no están incluidos en la plantilla de diseño aplicada al usuario. El administrador de [!DNL Workfront] debe asignar una plantilla de diseño que incluya los filtros. 

>[!NOTE]
>
>A veces, los filtros se eliminan del área [!UICONTROL Controles de lista] en [!UICONTROL Configuración]. El administrador de [!DNL Workfront] debe incluirlos en las listas de esta área para que estén disponibles en las plantillas de diseño.

1. Compruebe que la plantilla de diseño muestre los siguientes filtros:

   * [!UICONTROL Proyectos en los que participo] y [!UICONTROL Proyectos de mi propiedad] en el área de [!UICONTROL Proyectos]
   * [!UICONTROL Mis aprobaciones de plantillas de horas] y [!UICONTROL Mis plantillas de horas] en el área [!UICONTROL Plantilla de horas]

   Para ello:

   1. Acceda a la plantilla de diseño.
   1. Seleccione **[!UICONTROL Listas]** en **[!UICONTROL Personalizar lo que ven los usuarios]**.
   1. Seleccione **[!UICONTROL Proyectos]** o **[!UICONTROL Plantillas de horas]** en **[!UICONTROL Seleccionar una lista para personalizar]**.
   1. En la sección **[!UICONTROL Filtrar]**, verifique que estén seleccionados **[!UICONTROL Proyectos en los que participo]**, **[!UICONTROL Proyectos de mi propiedad]** (para proyectos) y **[!UICONTROL Mis aprobaciones de plantillas de horas]** y **[!UICONTROL Mis plantillas de horas]** (para plantillas de horas).
   1. Haga clic en **[!UICONTROL Guardar]**.

   Para obtener más información, consulte [Personalizar filtros, vistas y agrupaciones mediante una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. Asigne la plantilla de diseño a los usuarios, las funciones, los equipos o los grupos correctos. Para obtener más información, consulte [Asignar usuarios a una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).
