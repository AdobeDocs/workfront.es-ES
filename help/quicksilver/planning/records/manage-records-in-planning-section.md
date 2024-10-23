---
title: Administrar registros en la sección de planificación de objetos de Adobe Workfront
description: Puede mostrar los registros de Workfront Planning conectados a objetos de Adobe Workfront en la sección Planning de un objeto de Workfront, en el panel izquierdo.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d86cf3f9-cacc-4457-acb3-a5122ae91be8
source-git-commit: ecafbd693237427d727b15dd22afd485b4e59c72
workflow-type: tm+mt
source-wordcount: '802'
ht-degree: 1%

---


<!--add also Group and Company when they are available-->

# Administrar conexiones de registro desde objetos de Workfront

{{planning-important-intro}}

Puede mostrar los registros de Workfront Planning conectados a objetos de Adobe Workfront en la sección Planning de un objeto de Workfront, en el panel izquierdo.

<!--replace above with this: 

You can display Workfront Planning records and their respective records connected to Adobe Workfront objects in the following areas in Workfront:

* The Planning section of a Workfront object: Displays all record types connected to an object and their respective connected records. 
* A Planning connection custom field: Displays one record type and its respective connected records .-->

La sección Planificación está disponible para los siguientes objetos de Workfront:

* Proyecto
* Portafolio
* Programar
<!--* Group
* Company-->

<!--move the above to a lower place below when releasing Planning connection custom field-->


## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso para Workfront Planning.

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
   <p> Productos</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Planificación de Adobe Workfront<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>plan Adobe Workfront*</p></td>
   <td>
<p>Cualquiera de los siguientes planes de Workfront:</p>
<ul><li>Seleccionar</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning no está disponible para planes Workfront heredados</p>
   </td>

<tr>
   <td role="rowheader"><p>Plan de planificación de Adobe Workfront*</p></td>
   <td>
<p>Cualquiera</p>
<p>Para obtener más información sobre qué se incluye en cada plan de Workfront Planning, póngase en contacto con su administrador de cuentas de Workfront. </p>
   </td>

<tr>
   <td role="rowheader"><p>plataforma de Adobe Workfront</p></td>
   <td>
<p>La instancia de Workfront de su organización debe incorporarse a la experiencia Adobe unificado para poder acceder a todas las funcionalidades de Workfront Planning.</p>
<p>Para obtener más información, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiencia unificada de Adobe para Workfront</a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Licencia de Adobe Workfront*</p></td>
   <td>
   <p>Estándar</p>
   <p>Workfront Planning no está disponible para licencias de Workfront heredadas</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Configuración del nivel de acceso</p></td>
   <td> <p>Acceso de visualización o superior a Proyectos, Programas y Portfolio</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permisos de objeto</p></td>
   <td>
   <p>En Workfront, vea o supere los permisos de un proyecto, portafolio o programa</a> </p> 
   <p>En Workfront Planning, Contribute o permisos superiores para un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo de Workfront Planning, incluidos los que no crearon</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>A todos los usuarios, incluidos los administradores de Workfront, se les debe asignar una plantilla de diseño que incluya el área de Planning en el menú principal y el área de Planning para proyectos, portafolios y programas. </p> Para obtener más información, vea <a href="/help/quicksilver/planning/access/access-overview.md">Información general sobre el acceso a Adobe Planning</a>. </p>  </p>  
</td>
  </tr>
 </tbody>
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Administrar registros en la sección Planificación

Puede utilizar la sección Planning de un objeto Workfront para ver todos los tipos de registros y sus registros respectivos conectados al objeto Workfront.

<!--move the section above starting with "The Planning section is available ..." here-->

### Consideraciones sobre la sección Planificación de objetos de Workfront

Tenga en cuenta lo siguiente cuando vea los registros de Workfront Planning desde la sección Planning de un objeto Workfront:

* Los tipos de registros de Workfront Planning deben conectarse primero a los tipos de objetos de Workfront.

  Para obtener más información, consulte los siguientes artículos:

   * [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md)
   * [Conectar registros](/help/quicksilver/planning/records/connect-records.md)
* Puede ver la sección de Planning desde un objeto de Workfront, incluso cuando no haya registros asociados al objeto de Workfront.

### Administrar conexiones de registro desde la sección de Planning

{{step1-to-planning}}

1. Haga clic en la tarjeta de un espacio de trabajo.

   El espacio de trabajo se abre y los tipos de registro se muestran como tarjetas.

1. Haga clic en la tarjeta de un tipo de registro conectado a un proyecto, portafolio o programa de Workfront.
1. Vaya a un campo de registro conectado que tenga una conexión con un objeto Workfront, ya sea en la vista de tabla o desde la página de detalles de un registro. Para obtener más información, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).
1. Haga clic en el nombre de un objeto Workfront en el campo de registro conectado.
La página del objeto se abre en Workfront.

   >[!NOTE]
   >
   >  Si conoce un objeto de Workfront que ya está conectado a un registro de Planning, puede desplazarse a la sección de Planning desde el objeto de Workfront.

1. Haga clic en **Planificación** en el panel izquierdo.

   >[!NOTE]
   >
   >   El administrador de Workfront o de grupo debe agregar la sección de planificación a la plantilla de diseño para que se muestre para un proyecto, portafolio o programa de Workfront.

   La sección Planificación se muestra con la siguiente información:

   * Los registros conectados se muestran en tarjetas individuales que contienen la siguiente información:
      * Nombre del registro
      * La miniatura del registro
      * Nombre del campo de registro conectado tal como se muestra en Workfront Planning.
   * Los registros se muestran en su espacio de trabajo respectivo.

   ![](assets/planning-section-on-project.png)

1. (Opcional) Haga clic en **Mostrar todas las conexiones** para mostrar todos los tipos de registros conectados, incluidos los que no tienen registros conectados. De forma predeterminada, no se muestran los tipos de registros sin registros conectados.
1. Haga clic en una tarjeta de registro para mostrar más información sobre el registro. Se muestra el cuadro de vista previa de registros.
1. (Opcional) Comience a modificar los campos en el cuadro de vista previa del registro. Los cambios se guardarán automáticamente.
1. (Opcional) Haga clic en el icono **Abrir en una nueva ficha** ![](assets/open-details-in-a-new-tab-icon.png) en la esquina superior derecha del cuadro de vista previa para abrir la página de detalles del registro. Se abre la página de detalles del registro en Workfront Planning.
1. (Opcional) Pase el ratón sobre una tarjeta de registro, haga clic en el icono de registro de desconexión **-** y, a continuación, haga clic en **Desconectar**.
Ocurren lo siguiente:
   * El registro ya no está conectado al objeto Workfront.
   * El objeto Workfront también se quita del campo conectado del registro de Workfront Planning.
   * También se eliminan los valores de los campos de búsqueda de Workfront conectados al registro de Planning.
1. Haga clic en **Conectar** para conectar más registros para los tipos de registros conectados. Para obtener más información, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

   Ocurren lo siguiente:

   * Los registros se conectan inmediatamente al objeto Workfront y se muestran en la sección Planificación.
   * El objeto Workfront se agrega al campo conectado del registro de Workfront Planning.
   * Los valores de los campos de búsqueda de Workfront conectados al registro de Planning se rellenan en Workfront Planning.

<!--

## Manage records in the Planning connection field type

You can use a Planning connection custom field on a Workfront object to view one record type and its respective records connected to the Workfront object. 

You can control which Planning records display for the Workfront object when you create Planning connection custom fields. 

* The Planning connection field can be populated with Planning records when it is attached to forms for the following Workfront objects:

   * Project
   * Portfolio
   * Program
   * Group
   * Company

For more information, see [Create a form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md). 

### Considerations about the Planning connection field type

Consider the following when you view Workfront Planning records from a Planning connection field of a Workfront object: 

* You can associate only one record type with one Planning connection field.
* Your Workfront or group administrator must add a Planning connection field on a Workfront custom form.
* You must attach the custom form to a Workfront object that can be connected from Workfront Planning, if you have the correct access.
* Workfront Planning record types must first be connected to Workfront object types. For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md). 
* You can connect or disconnect records from the Planning connection field of a Workfront object only for objects that can have Workfront Planning connections.
* You must have Contribute permissions for a workspace in Workfront Planning to be able to connect or disconnect records from the Planning connection field of a Workfront object.
* You can view a Planning connection field for a Workfront object, even when there are no records connected to the object yet. 
* You cannot edit a Planning connection field when editing Workfront objects in bulk. 

### Manage record connections from the Planning connection field type

1. Go to one of the following object types that has been connected with a Workfront Planning record type: 

   * Project
   * Portfolio
   * Program
   * Company
   * Group

1. Click **< Object > Details** in the left panel.
1. (Conditional) Add a custom form with at least one Planning connection field for the object you selected, if one is not present. 

   >[!NOTE]
   >
   >Your Workfront or group administrator must first create the form and add a Planning connection field on it before you can add it to an object. 


1. Click inside the field to add connected records.
1. Click the downward-pointing arrow inside the field, to select records from the list. 

   ![](assets/planning-connection-field-on-project-with-record-list-open.png)

   >[!TIP]
   >
   >   You cannot add records to Planning connection fields that are associated with Workfront objects other than the object you selected. 
   >
   >For example, you cannot add records to a Planning connection field created for a Portfolio connection from a Project's custom form. 
   >
   >There is an indication that the object of the field and the object you selected don't match.  
   >
   >![](assets/warning-unsupported-object-planning-connection-field-on-form.png)

1. Click outside the list to close it. 

   The following things occur:

   * The records are immediately connected to the Workfront object and they display in the Planning connection field as well as the Planning section of the Workfront object. 
   * The Workfront object is added to the Workfront Planning record's connected field. 
   * The values for the Workfront lookup fields connected to the Planning record are populated in Workfront Planning. 
1. (Optional) Click the name of a record in the Planning connection field to open it in Workfront Planning. 
   The record details tab opens in Workfront Planning. 
   You can review information about the record, or navigate to the record type page. 

1. (Optional) From the custom form in Workfront, click the **Remove** icon ![](assets/remove-icon.png) on a record to remove it from the Planning connection field and disconnect it from the Workfront object. 
   The Workfront object is disconnected from the Planning record, and any lookup information from Workfront is removed from the record. 

-->