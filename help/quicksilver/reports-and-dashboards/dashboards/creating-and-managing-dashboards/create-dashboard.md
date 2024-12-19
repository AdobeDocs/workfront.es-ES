---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Creación de un panel
description: Puede crear paneles para acceder rápidamente a la información en Adobe Workfront. Se pueden añadir informes, calendarios y páginas externas a los paneles, los cuales puede compartir con otros para lograr una colaboración óptima.
author: Nolan
feature: Reports and Dashboards
exl-id: 6a284df4-f011-4b4c-b44c-2e20918f643f
source-git-commit: 51e8faf8cc91546ccc1af551f359f81c2174c19b
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 87%

---

# Creación de un panel

<!--Audited: 01/2024-->

Puede crear paneles para acceder rápidamente a la información en Adobe Workfront. Se pueden agregar hasta 25 informes, calendarios y páginas externas a los paneles que puede compartir con otros para lograr una colaboración óptima.

Para obtener más información sobre los paneles, consulte [Introducción a los paneles](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener lo siguiente:

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Plan de Adobe Workfront</strong></p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td> <p><strong>Licencia de Adobe Workfront*</strong></p> </td> 
   <td> <p>Actual: plan </p>
   O
   <p>Nuevo: estándar </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Configuraciones de nivel de acceso</strong> </td> 
   <td> <p>Editar el acceso a Informes, Paneles y Calendarios</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Permisos de objeto</strong> </p> </td> 
   <td> <p>Obtendrá permisos de administración en los paneles que cree</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront. Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Debe crear cualquiera de los siguientes objetos antes de añadirlos a un panel:

* **Informes**: para obtener información sobre cómo crear informes, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* **Calendarios**: para obtener información sobre cómo crear calendarios, consulte [Información general de informes de calendario](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

Puede añadir páginas externas existentes a un panel o crear una desde el nuevo panel. Para obtener información sobre cómo crear páginas externas, consulte [Incrustar una página web externa en un panel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

## Creación de un panel

{{step1-to-dashboards}}

1. Haga clic en **Nuevo panel**.\
   Se muestra el cuadro de diálogo Nuevo panel.

1. Especifique lo siguiente:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>Nombre</strong></td>
      <td><p>Este es el nombre del panel.</p><p>Si no especifica un nombre, el nombre del primer informe del panel se convierte en el nombre del panel de forma predeterminada.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Descripción (opcional)</strong></td>
      <td>Esta es una descripción del panel.</td>
     </tr>
    </tbody>
   </table>

1. Seleccione un diseño haciendo clic en el botón de opción correspondiente en la parte superior de la sección **Seleccionar diseño/ Añadir informes/ Añadir calendarios**. Diseño en el que se muestran los informes, calendarios o páginas externas en el panel.

   El diseño predeterminado es el de una sola columna.

   Para obtener información sobre el diseño de informes en los paneles, consulte [Comprender cómo se muestran los informes en un panel](../../../reports-and-dashboards/dashboards/understanding-dashboards/understand-how-reports-display-dashboard.md).

   <!--
   Consider adding the information from this article above here, at some point, instead of linking to it.)
   -->

1. En la sección **Informes y calendarios disponibles**, empiece a escribir el nombre de un informe, calendario o página externa en la barra de búsqueda y, a continuación, arrastre y suelte el informe, calendario o página externa en el panel de diseño situado a la derecha.

   >[!NOTE]
   >
   >Al buscar un elemento, la búsqueda devuelve cualquiera de los 2000 informes con fecha de creación más reciente. Los nombres de los informes que incluyen caracteres Unicode no se devuelven en los resultados de búsqueda. Como práctica recomendada, evite incluir caracteres Unicode al nombrar objetos en Workfront escribiendo nombres en lugar de copiar y pegar nombres de otra fuente.

   ![Búsqueda de informes](assets/unshimmed-dashboard-ui.png)

1. (Opcional) Haga clic en **Añadir página externa** para añadir una nueva página externa al panel.

   Para obtener más información sobre cómo crear páginas externas e incrustarlas en los paneles, consulte [Incrustar una página web externa en un panel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

1. Haga clic en **Guardar + Cerrar**.

   Una marca de tiempo se muestra en la esquina superior derecha del panel. La marca de tiempo incluye la fecha, la hora y el huso horario en que se actualizó el panel de control por última vez.
