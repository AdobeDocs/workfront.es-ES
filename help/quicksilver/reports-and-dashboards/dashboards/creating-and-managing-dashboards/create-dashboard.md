---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Creación de un panel de control
description: Puede crear paneles de control para acceder rápidamente a la información en Adobe Workfront. Se pueden añadir informes, calendarios y páginas externas a los paneles de control, los cuales puede compartir con otros para lograr una colaboración óptima.
author: Nolan
feature: Reports and Dashboards
exl-id: 6a284df4-f011-4b4c-b44c-2e20918f643f
source-git-commit: c8b7ad473b0c2120ef5ea52374b3501ad6f553f1
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 83%

---

# Creación de un panel de control

<!--Audited: 01/2025-->

Puede crear paneles de control para acceder rápidamente a la información en Adobe Workfront. Se pueden agregar hasta 25 informes, calendarios y páginas externas a los paneles que puede compartir con otros para lograr una colaboración óptima.

Para obtener más información sobre los paneles de control, consulte [Introducción a los paneles de control](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
      <p>Estándar</p>
      <p>Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Informes, Paneles de control y Calendarios</p></td> 
  </tr>  
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Obtendrá permisos de administración en los paneles de control que cree</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Debe crear cualquiera de los siguientes objetos antes de añadirlos a un panel de control:

* **Informes**: para obtener información sobre cómo crear informes, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* **Calendarios**: para obtener información sobre cómo crear calendarios, consulte [Información general de informes de calendario](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

Puede añadir páginas externas existentes a un panel de control o crear una desde el nuevo panel de control. Para obtener información sobre cómo crear páginas externas, consulte [Incrustar una página web externa en un panel de control](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

## Creación de un panel de control

{{step1-to-dashboards}}

1. Haga clic en **Nuevo panel de control**.\
   Se muestra el cuadro de diálogo Nuevo panel de control.

1. Especifique lo siguiente:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>Nombre</strong></td>
      <td><p>Este es el nombre del tablero. Se recomienda utilizar solo caracteres UTF-8 para evitar problemas de compatibilidad.</p><p>Si no especifica un nombre, el nombre del primer informe del panel de control se convierte en el nombre del panel de control de forma predeterminada.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Descripción (opcional)</strong></td>
      <td>Esta es una descripción del panel de control.</td>
     </tr>
    </tbody>
   </table>

1. Seleccione un diseño haciendo clic en el botón de opción correspondiente en la parte superior de la sección **Seleccionar diseño/ Añadir informes/ Añadir calendarios**. Diseño en el que se muestran los informes, calendarios o páginas externas en el panel de control.

   El diseño predeterminado es el de una sola columna.

   Para obtener información sobre el diseño de informes en los paneles de control, consulte [Comprender cómo se muestran los informes en un panel de control](../../../reports-and-dashboards/dashboards/understanding-dashboards/understand-how-reports-display-dashboard.md).

   <!--
   Consider adding the information from this article above here, at some point, instead of linking to it.)
   -->

1. En la sección **Informes y calendarios disponibles**, empiece a escribir el nombre de un informe, calendario o página externa en la barra de búsqueda y, a continuación, arrastre y suelte el informe, calendario o página externa en el panel de diseño situado a la derecha.

   >[!NOTE]
   >
   >Al buscar un elemento, la búsqueda devuelve cualquiera de los 2000 informes con fecha de creación más reciente. Los nombres de los informes que incluyen caracteres Unicode no se devuelven en los resultados de búsqueda. Como práctica recomendada, evite incluir caracteres Unicode al nombrar objetos en Workfront escribiendo nombres en lugar de copiar y pegar nombres de otra fuente.

   ![Búsqueda de informes](assets/unshimmed-dashboard-ui.png)

1. (Opcional) Haga clic en **Añadir página externa** para añadir una nueva página externa al panel de control.

   Para obtener más información sobre cómo crear páginas externas e incrustarlas en los paneles de control, consulte [Incrustar una página web externa en un panel de control](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

1. Haga clic en **Guardar + Cerrar**.

   Una marca de tiempo se muestra en la esquina superior derecha del panel de control. La marca de tiempo incluye la fecha, la hora y el huso horario en que se actualizó el panel de control por última vez.
