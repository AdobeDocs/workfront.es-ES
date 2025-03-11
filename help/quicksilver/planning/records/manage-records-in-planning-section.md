---
title: Administrar registros en la sección de planificación de objetos de Adobe Workfront
description: Puede mostrar los registros de Workfront Planning conectados a objetos de Adobe Workfront en la sección Planning de un objeto de Workfront, en el panel izquierdo.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d86cf3f9-cacc-4457-acb3-a5122ae91be8
source-git-commit: fd8e5d3baf6af0dbdd1275494fad54b204abd1a5
workflow-type: tm+mt
source-wordcount: '1797'
ht-degree: 7%

---


<!--add also Group and Company when they are available-->

# Administrar conexiones de registro desde objetos de Workfront

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información acerca de las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

{{planning-important-intro}}

Puede mostrar registros de Workfront Planning en Workfront en las siguientes áreas de los objetos conectados a ellos:

* La sección Planning de un objeto Workfront: muestra todos los tipos de registros conectados a un objeto y sus registros conectados respectivos.
* Campo personalizado de conexión de Planning: muestra un tipo de registro, sus registros conectados respectivos, <span class="preview"> y hasta 7 campos de búsqueda de los registros conectados.</span>

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso.

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
   <td role="rowheader"><p>Plan de Adobe Workfront*</p></td>
   <td>
<p>Cualquiera de los siguientes planes de Workfront:</p>
<ul><li>Seleccionar</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning no está disponible para planes Workfront heredados</p>
   </td>

<tr>
   <td role="rowheader"><p>Paquete de planificación de Adobe Workfront*</p></td>
   <td>
<p>Cualquiera</p>
<p>Para obtener más información sobre qué se incluye en cada plan de Workfront Planning, póngase en contacto con su administrador de cuentas de Workfront. </p>
   </td>

<tr>
   <td role="rowheader"><p>plataforma de Adobe Workfront</p></td>
   <td>
<p>La instancia de Workfront de su organización debe incorporarse a Adobe Unified Experience para poder acceder a todas las funcionalidades de Workfront Planning.</p>
<p>Para obtener más información, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience para Workfront</a>. </p>
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
   <td role="rowheader"><p>Configuración de nivel de acceso</p></td>
   <td> <p>Acceso de visualización o superior a Proyectos, Programas y Portafolios</p>  
   <p>No hay ninguna configuración de nivel de acceso para Workfront Planning. </p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permisos de objeto</p></td>
   <td>
   <p>En Workfront, vea o supere los permisos de un proyecto, portafolio o programa</a> </p> 
   <p>En Workfront Planning:
   <ul><li>
   Ver los permisos de un área de trabajo <!--<span class="preview">and record type</span>--> para ver los registros conectados </li>
   o
   <li> Conceder permisos de contribución o superiores a un espacio de trabajo <!--<span class="preview">and record type</span>--> para conectar o desconectar registros</a></li></ul> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo de Workfront Planning, incluidos los que no crearon</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>Para ver el área de Planning o la sección de Planning de un objeto de Workfront, todos los usuarios, incluidos los administradores de Workfront, deben tener asignada una plantilla de diseño que incluya el área de Planning en el menú principal y el área de Planning para proyectos, portafolios y programas. </p> Para obtener más información, consulte <a href="/help/quicksilver/planning/access/access-overview.md">Información general sobre el acceso a Adobe Planning</a>. </p>  </p>  
</td>
  </tr>
 </tbody>
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Administrar registros en la sección Planificación

Puede utilizar la sección Planning de un objeto Workfront para ver todos los tipos de registros y sus registros respectivos conectados al objeto Workfront.
La sección Planificación está disponible para los siguientes objetos de Workfront:

* Proyecto
* Portafolio
* Programa
<!--* Group
* Company-->

### Consideraciones sobre la sección Planificación de objetos de Workfront

Tenga en cuenta lo siguiente cuando vea los registros de Workfront Planning desde la sección Planning de un objeto Workfront:

* Los tipos de registros de Workfront Planning deben conectarse primero a los tipos de objetos de Workfront.

  Para obtener más información, consulte los siguientes artículos:

   * [Conectar tipos de registro](/help/quicksilver/planning/architecture/connect-record-types.md)
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
   * Los registros se muestran bajo su respectivo espacio de trabajo y tipo de registro.

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
1. Haga clic en **Conectar** para conectar más registros para los tipos de registros conectados.

   Para obtener más información, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).
1. (Opcional) Si no encuentra un registro para conectarse y desea agregarlo, haga clic en **+ Agregar** para agregar un nuevo registro. Para obtener más información, vea la sección &quot;Crear registros a medida que los conecta desde otros registros&quot; en el artículo [Crear registros](/help/quicksilver/planning/records/create-records.md).

   Ocurren lo siguiente:

   * Los registros se conectan inmediatamente al objeto Workfront y se muestran en la sección Planificación.
   * El objeto Workfront se agrega al campo conectado del registro de Workfront Planning.
   * Los valores de los campos de búsqueda de Workfront conectados al registro de Planning se rellenan en Workfront Planning.

## Administrar registros en el tipo de campo de conexión de Planning

Puede utilizar un campo personalizado de conexión de Planning en un objeto Workfront para ver un tipo de registro y sus registros respectivos conectados al objeto Workfront.

Puede controlar qué tipos de registros de Planning se muestran para el objeto de Workfront al crear campos personalizados de conexión de Planning.

* El campo Conexión de Planning muestra registros de Planning después de establecer una conexión y cuando el campo está adjunto a formularios para los siguientes objetos de Workfront:

   * Proyecto
   * Portafolio
   * Programa
   * Grupo
   * Compañía

Para obtener más información, consulte [Crear un formulario](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Consideraciones acerca del tipo de campo de conexión de Planning

Tenga en cuenta lo siguiente cuando vea los registros de Workfront Planning desde un campo de conexión de Planning de un objeto de Workfront:

* Un campo de conexión de Planning se muestra de las siguientes maneras en el formulario personalizado de un objeto de Workfront, después de que los registros de Planning estén conectados al objeto de Workfront:

   * Si sólo se selecciona el campo principal del registro conectado, el campo de conexión de Planning se muestra como un campo con varios valores, si la conexión permite vincular varios registros. Para obtener más información, consulte [Información general sobre los tipos de registros de Connect](/help/quicksilver/planning/architecture/connect-record-types-overview.md).
   * <span class="preview">Si el administrador del grupo o de Workfront agregó campos de búsqueda adicionales desde el registro conectado en el formulario personalizado, el campo de conexión de Planning se mostrará como una tabla. Se pueden seleccionar hasta 7 campos para el campo Planning connection. La vista de tabla es de solo lectura.  </span>

* Sólo puede asociar un tipo de registro con un campo de conexión de Planning. No hay límite en cuanto a la cantidad de campos de conexión de Planning que tiene en un formulario.
* Debe tener el acceso y los permisos correctos para el objeto, el registro y Workfront Planning para adjuntar un formulario personalizado con un campo personalizado de conexión de Planning a un objeto de Workfront.
* Debe tener permisos de contribución para un espacio de trabajo en Workfront Planning para poder conectar o desconectar registros del campo de conexión de Planning de un objeto de Workfront.
* Los tipos de registros de Workfront Planning deben conectarse primero a los tipos de objetos de Workfront. Para obtener más información, consulte [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md). Esto hace que los registros de Workfront Planning sean accesibles desde Workfront.
* Puede conectar o desconectar registros del campo de conexión de Planning de un objeto de Workfront sólo para objetos que puedan tener conexiones de Workfront Planning.

  Por ejemplo, puede adjuntar un formulario personalizado con un campo de conexión de Planning a las tareas, pero no puede conectar objetos de Workfront Planning a las tareas.
* No se puede editar un campo de conexión de Planning al editar objetos de Workfront de forma masiva.

### Administrar conexiones de registro desde el tipo de campo Conexión de Planning

1. Vaya a uno de los siguientes tipos de objetos que se han conectado con un tipo de registro de Workfront Planning:

   * Proyecto
   * Portafolio
   * Programa
   * Compañía
   * Grupo

1. Haga clic en **&lt; Objeto > Detalles** en el panel izquierdo.
1. (Condicional) Agregue un formulario personalizado con al menos un campo de conexión de Planning para el objeto seleccionado, si no hay ninguno presente.

   >[!NOTE]
   >
   >El administrador de Workfront o de grupo debe crear primero el formulario y agregarle un campo de conexión de Planning para poder agregarlo a un objeto.


1. Haga clic dentro del campo para agregar registros conectados y, a continuación, haga clic en la flecha hacia abajo dentro del campo para seleccionar registros de la lista.

   ![](assets/planning-connection-field-on-project-with-record-list-open.png)

   >[!TIP]
   >
   >No se pueden agregar registros a los campos de conexión de Planning asociados a objetos de Workfront que no sean el objeto seleccionado cuando se configuró el campo.
   >
   >Por ejemplo, no se pueden agregar registros a un campo de conexión de Planning creado para una conexión de Portfolio desde el formulario personalizado de un proyecto.
   >
   >Hay una indicación de que el objeto del campo y el objeto seleccionado no coinciden.
   >
   >![](assets/warning-unsupported-object-planning-connection-field-on-form.png)

1. Haga clic fuera de la lista para cerrarla.

   Ocurren lo siguiente:

   * Los registros se conectan inmediatamente al objeto Workfront y se muestran en el campo Planning connection y en la sección Planning del objeto Workfront.
   * El objeto Workfront se agrega al campo conectado del registro de Workfront Planning.
   * Los valores de los campos de búsqueda de Workfront conectados al registro de Planning se rellenan en Workfront Planning.
   * <span class="preview">Si el administrador de grupo o Workfront agregó campos de búsqueda de registros al crear el formulario personalizado, los campos de búsqueda del registro se rellenarán automáticamente en una vista de tabla. La vista de tabla del campo de conexión de Planning es de solo lectura </span>

     ![](assets/planning-connection-field-with-table-on-project-details-custom-form.png)

1. (Opcional) Haga clic en el nombre de un registro <span class="preview">o coloque el puntero sobre el nombre del registro de la tabla y, a continuación, haga clic en el icono **Abrir registro** ![Icono Abrir registro en el formulario personalizado de conexión de Planning](assets/open-record-icon-on-planning-connection-custom-form.png)</span> en el campo Conexión de Planning para abrirlo en Workfront Planning.
Se abre el cuadro de vista previa de detalles del registro de Workfront Planning.
1. Revise o edite la información sobre el registro o haga clic en el icono **Abrir en una ficha nueva** ![Abrir registro en una ficha nueva](assets/open-details-in-a-new-tab-icon.png) para abrir la página de detalles del registro.

1. (Opcional) En el formulario personalizado de Workfront, haga clic en el icono **Quitar** ![](assets/remove-icon.png) de un registro para quitarlo del campo de conexión de Planning y desconectarlo del objeto de Workfront.
El objeto Workfront se desconecta del registro de Planning y cualquier información de búsqueda de Workfront se quita del registro.

1. Haga clic en **Guardar cambios** para guardar el formulario personalizado y cualquier otro cambio que haya realizado en el objeto de Workfront.