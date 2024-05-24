---
title: Administrar registros en la sección Planificación de objetos de Adobe Workfront
description: Puede mostrar los registros conectados a objetos de Adobe Workfront en la sección Planning de un objeto de Workfront, en el panel izquierdo.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: c2659e0b3f571053c1c014703103bfcc7935ff3c
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 1%

---


<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--add also Group and Company when they are available-->

<!-- opening the Details preview and page is not possible yet - hid those steps, but add them when released-->


# Administrar registros en la sección Planificación de objetos de Adobe Workfront

{{maestro-important-intro}}

Puede mostrar los registros conectados a objetos de Adobe Workfront en la sección Planning de un objeto de Workfront, en el panel izquierdo.

La sección Planificación está disponible para los siguientes objetos de Workfront:

* Proyecto
* Portafolio
* Programar
<!--* Group
* Company-->

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

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
<p>Su organización debe estar inscrita en el programa beta de Adobe Workfront Planning. Póngase en contacto con el representante de cuentas para obtener más información sobre esta nueva oferta. </p>
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
   <td> <p>En Workfront, vea o aumente los permisos de un proyecto, portafolio o programa</a> </p> 
   <p>En Workfront Planning, vea los permisos o superiores de un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo de Workfront Planning, incluidos los que no crearon</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>El administrador de su Workfront o de su grupo debe añadir el área de Planning en el menú principal y la sección de Planning en el panel izquierdo a la plantilla de diseño. Para obtener más información, consulte <a href="../access/access-overview.md">Acceso a información general</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Consideraciones sobre la sección Planificación de objetos de Workfront

* En primer lugar, debe conectar los tipos de registros a los tipos de objetos de Workfront y los registros a los objetos de Workfront para verlos en Workfront.

  Para obtener más información, consulte los siguientes artículos:

   * [Conectar tipos de registros](/help/quicksilver/maestro/architecture/connect-record-types.md)
   * [Conectar registros](/help/quicksilver/maestro/records/connect-records.md)
* Puede ver la sección de Planning en un objeto de Workfront, incluso cuando no haya registros asociados al objeto de Workfront.
* Puede conectar registros de Planning con objetos de Workfront desde Workfront, en la sección de Planning cuando haya al menos un registro conectado al objeto de Workfront.
* Debe tener permisos de Contribute o superiores en un espacio de trabajo para conectar registros de los objetos de Workfront.

## Administrar registros en la sección Planificación

{{step1-to-maestro}}

El último espacio de trabajo al que se accede se abre de forma predeterminada.

1. Haga clic en la tarjeta de un tipo de registro conectado a un proyecto, portafolio o programa de Workfront.
1. Elija una vista de tabla de la **Ver** menú desplegable.
1. (Condicional) Vaya al campo de registro conectado de la tabla y agregue un objeto Workfront; a continuación, haga clic en el nombre del objeto Workfront en el campo. Para obtener más información, consulte [Conectar registros](/help/quicksilver/maestro/records/connect-records.md).
La página del objeto se abre en Workfront Planning.
1. Clic **Ir al origen**, en la esquina superior derecha de la pantalla.

   La página del objeto se abre en Workfront.
1. Clic **Planificación** en el panel izquierdo.

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
1. (Opcional) Haga clic en **Abrir en una pestaña nueva** icono ![](assets/open-details-in-a-new-tab-icon.png) en la esquina superior derecha del cuadro de vista previa para abrir la página de detalles del registro.
1. Pase el ratón sobre una tarjeta de registro y haga clic en el icono de desconexión de registro **-**, luego haga clic en **Desconectar**.
Ocurren lo siguiente:
   * El registro ya no está conectado al objeto Workfront.
   * El objeto Workfront también se quita del campo conectado del registro de Workfront Planning.
   * También se eliminan los valores de los campos de búsqueda de Workfront conectados al registro de Planning.
1. Clic **Connect** para conectar más registros.

   >[!NOTE]
   >
   >   El botón Conectar sólo se muestra para los espacios de trabajo en los que tiene permisos de Contribute.

1. Haga clic en los registros que desee conectar. Ocurren lo siguiente:

   * Los registros se conectan inmediatamente al objeto Workfront y se muestran en la sección Planificación.
   * El objeto Workfront se agrega al campo conectado del registro de Workfront Planning.
   * Los valores de los campos de búsqueda de Workfront conectados al registro de Planning se rellenan en Workfront Planning.

<!--add more steps here for what happens after clicking Connect-->


