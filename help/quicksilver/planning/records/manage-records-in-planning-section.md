---
title: Administrar registros en la sección Planificación de objetos de Adobe Workfront
description: Puede mostrar los registros conectados a objetos de Adobe Workfront en la sección Planning de un objeto de Workfront, en el panel izquierdo.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: d86cf3f9-cacc-4457-acb3-a5122ae91be8
source-git-commit: 5c7b60ac5b78bd065ffc270588ec72ab3eb2f41d
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 1%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--add also Group and Company when they are available-->

<!-- opening the Details preview and page is not possible yet - hid those steps, but add them when released-->


# Administrar registros en la sección Planificación de objetos de Adobe Workfront

{{planning-important-intro}}

Puede mostrar los registros conectados a objetos de Adobe Workfront en la sección Planning de un objeto de Workfront, en el panel izquierdo.

La sección Planificación está disponible para los siguientes objetos de Workfront:

* Proyecto
* Portafolio
* Programar
<!--* Group
* Company-->

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso para Workfront Planning.

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>acuerdo con Adobe Workfront</p></td>
   <td>
<p>Su organización debe estar inscrita en la fase de acceso anticipado para Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>plan de Adobe Workfront</p></td>
   <td>
<p>Cualquiera</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licencia de Adobe Workfront*</p></td>
   <td>
   <p>Nuevo: estándar</p>
   O
   <p>Actual: plan</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuraciones de nivel de acceso</p></td>
   <td> <p>Acceso de visualización o superior a Proyectos, Programas y Portfolio</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permisos</p></td>
   <td> <p>En Workfront, vea o supere los permisos de un proyecto, portafolio o programa</a> </p> 
   <p>En Workfront Planning, Contribute o permisos superiores para un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo de Workfront Planning, incluidos los que no crearon</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>El administrador de su Workfront o de su grupo debe añadir el área de Planning en el menú principal y la sección de Planning en el panel izquierdo a la plantilla de diseño. Para obtener más información, consulte <a href="/help/quicksilver/planning/access/access-overview.md">Resumen de acceso</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones sobre la sección Planificación de objetos de Workfront

* En primer lugar, debe conectar los tipos de registros a los tipos de objetos de Workfront y los registros a los objetos de Workfront para verlos en Workfront.

  Para obtener más información, consulte los siguientes artículos:

   * [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md)
   * [Conectar registros](/help/quicksilver/planning/records/connect-records.md)
* Puede ver la sección de Planning en un objeto de Workfront, incluso cuando no haya registros asociados al objeto de Workfront.
* Puede conectar registros de Planning con objetos de Workfront desde Workfront, en la sección de Planning cuando haya al menos un registro conectado al objeto de Workfront.

## Administrar registros en la sección Planificación

{{step1-to-planning}}

1. Haga clic en la tarjeta de un espacio de trabajo.

   El espacio de trabajo se abre y los tipos de registro se muestran como tarjetas.

1. Haga clic en la tarjeta de un tipo de registro conectado a un proyecto, portafolio o programa de Workfront.
1. Vaya a un campo de registro conectado que tenga una conexión con un objeto Workfront, ya sea en la vista de tabla o desde la página de detalles de un registro. Para obtener más información, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).
1. Haga clic en el nombre de un objeto Workfront en el campo de registro conectado.
La página del objeto se abre en Workfront.

1. Haga clic en **Planificación** en el panel izquierdo.

   >[!NOTE]
   >
   >   El administrador de Workfront o del grupo debe agregar la sección de Planificación a la plantilla de diseño para que se muestre para un proyecto, portafolio o programa de Workfront.

   La sección Planificación se muestra con la siguiente información:

   * Los registros conectados se muestran en tarjetas individuales que contienen la siguiente información:
      * Nombre del registro
      * La miniatura del registro
      * Nombre del campo de registro conectado tal como se muestra en Workfront Planning.
   * Los registros se muestran en su espacio de trabajo respectivo.

   ![](assets/planning-section-on-project.png)

1. Haga clic en una tarjeta de registro para mostrar más información sobre el registro. Se muestra el cuadro de vista previa de registros.
1. (Opcional) Comience a modificar los campos en el cuadro de vista previa del registro. Los cambios se guardarán automáticamente.
1. (Opcional) Haga clic en el icono **Abrir en una nueva ficha** ![](assets/open-details-in-a-new-tab-icon.png) en la esquina superior derecha del cuadro de vista previa para abrir la página de detalles del registro. Se abre la página de detalles del registro en Workfront Planning.
1. Pase el ratón sobre una tarjeta de registro, haga clic en el icono de registro de desconexión **-** y, a continuación, haga clic en **Desconectar**.
Ocurren lo siguiente:
   * El registro ya no está conectado al objeto Workfront.
   * El objeto Workfront también se quita del campo conectado del registro de Workfront Planning.
   * También se eliminan los valores de los campos de búsqueda de Workfront conectados al registro de Planning.
1. Haga clic en **Conectar** para conectar más registros.

   >[!NOTE]
   >
   >   El botón Conectar solo se muestra en los espacios de trabajo en los que tiene permisos de Contribute. <!--they might replace this with one button at the top of the page. Rephrase-->

1. Haga clic en los registros que desee conectar. Ocurren lo siguiente:

   * Los registros se conectan inmediatamente al objeto Workfront y se muestran en la sección Planificación.
   * El objeto Workfront se agrega al campo conectado del registro de Workfront Planning.
   * Los valores de los campos de búsqueda de Workfront conectados al registro de Planning se rellenan en Workfront Planning.

<!--add more steps here for what happens after clicking Connect-->
