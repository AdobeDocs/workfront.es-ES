---
title: Creación de tipos de registros
description: Los tipos de registro son los tipos de objetos de Adobe Workfront Planning. En Workfront Planning, puede crear tipos de registros personalizados que ilustren los elementos de trabajo necesarios en el ciclo de vida de su organización.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: 160bcc8796666c9615ebe8ead18813b96be26a71
workflow-type: tm+mt
source-wordcount: '1258'
ht-degree: 1%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->
<!--this is linked to the UI in an empty workspace screen-->

# Creación de tipos de registros

{{planning-important-intro}}

Los tipos de registro son los tipos de objetos de Adobe Workfront Planning. En Workfront Planning, puede crear tipos de registros personalizados que ilustran los elementos relacionados con el trabajo necesarios en el ciclo de vida de su organización.

Para obtener más información sobre los tipos de registros, consulte [Resumen de tipos de registro](/help/quicksilver/planning/architecture/overview-of-record-types.md).

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
   <td> Adobe Workfront
   </td>
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
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td>
   <td>
   <p>Actual: plan</p>
   O
   <p>Nuevo: estándar </p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuraciones de nivel de acceso</p></td>
   <td> <p>No hay controles de nivel de acceso para Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>El administrador del grupo o de Workfront debe agregar el área de Planning a la plantilla de diseño. Para obtener más información, consulte <a href="/help/quicksilver/planning/access/access-overview.md">Acceso a información general</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permisos</p></td>
   <td> <p>Administración de permisos en un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Consideraciones sobre la creación de tipos de registros

* Puede crear tipos de registros en un espacio de trabajo de las siguientes maneras:

   * Automáticamente:
      * Cuando se crea un espacio de trabajo mediante una plantilla.

        Para obtener más información, consulte [Creación de espacios de trabajo](/help/quicksilver/planning/architecture/create-workspaces.md).

      * Cuando se importan mediante un archivo CSV o de Excel.

        >[!IMPORTANT]
        >
        >Esta funcionalidad se ha deshabilitado temporalmente desde el 21 de marzo de 2024. Se activará en una fecha posterior.

     <!--this should not ne known anymore: * When you add objects from another application to a linked record field of a record. This creates a read-only record type in Workfront Planning which is connected to object types from the original application. 
        For information about connecting record types with object types from another application, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).
        For information about connecting objects with records, see [Connect records](/help/quicksilver/planning/records/connect-records.md). -->
   * Manualmente:

      * Desde cero.

        Este artículo describe cómo crear tipos de registros desde cero.

* Puede mover tipos de registros dentro de una sección y de una sección de un espacio de trabajo a otra. No se pueden mover tipos de registros de un espacio de trabajo a otro.

## Creación de tipos de registros con una plantilla de Workspace

Puede crear tipos de registros automáticamente al crear un espacio de trabajo con una plantilla de Workfront Planning. Cada plantilla contiene tipos de registro de ejemplo.

Al crear un espacio de trabajo a partir de una plantilla, los tipos de registro se agrupan en las siguientes secciones:

* Tipos de registros operativos
* Taxonomías

Puede añadir manualmente tipos de registros en las secciones Tipos de registros operativos y Taxonomías.

Para obtener información sobre la creación de espacios de trabajo, consulte [Creación de espacios de trabajo](/help/quicksilver/planning/architecture/create-workspaces.md).

Para obtener información sobre los tipos de registros que se incluyen con cada plantilla, consulte [Lista de plantillas de Workspace](/help/quicksilver/planning/architecture/workspace-templates.md).

## Crear un tipo de registro desde cero

{{step1-to-planning}}

El espacio de trabajo al que se accedió por última vez debe abrirse de forma predeterminada.

1. (Opcional) Expanda la flecha hacia abajo a la derecha del nombre de un área de trabajo existente y seleccione el área de trabajo para la que desea crear tipos de registros.
1. (Opcional) Haga clic en **Agregar sección** para agregar una nueva sección al espacio de trabajo.
1. Clic **Añadir tipo de registro**.
1. (Condicional) Cuando esté habilitada la creación de tipos de registros mediante la importación de un archivo de Excel o CSV, haga clic en **Desde cero**. De lo contrario, la variable **Añadir tipo de registro** se abre el cuadro.

   ![](assets/add-record-type-box-with-appearance-options.png)

1. Actualice la siguiente información:

   * Sustituya &quot;Tipo de registro sin título&quot; por el nombre del tipo de registro futuro. <!--did they bring back the field label here and did they rename it to "Name"-->
   * **Descripción**: Añada más información sobre el tipo de registro.
   * Seleccione un color y una forma para el icono asociado al tipo de registro. Haga lo siguiente:
      * Seleccione un color para identificar el nuevo tipo de registro. Es el color del icono de tipo de registro. Gris está seleccionado de forma predeterminada.
      * Seleccione un icono de la lista o empiece a escribir el nombre de un icono para describir lo que representa y, a continuación, selecciónelo cuando se muestre. Este es el icono del tipo de registro. De forma predeterminada, se selecciona un icono de archivo.

1. Haga clic en **Crear**.

   La tarjeta de tipo de registro se añade a la sección y al espacio de trabajo seleccionado.
La descripción del tipo de registro se muestra en la tarjeta.

   ![](assets/record-type-card-with-description.png)

1. (Opcional) Pase el ratón sobre la tarjeta de tipo de registro y haga clic en **Más** icono ![](assets/more-menu.png) en la esquina superior derecha, haga clic en **Editar** para modificar información sobre el tipo de registro.
1. (Opcional) Haga clic en la tarjeta de tipo de registro para abrir la página de tipo de registro.

   ![](assets/operational-record-type-blank.png)

   La página de tipo de registro se muestra en la vista de tabla de forma predeterminada. Las columnas de la tabla son campos asociados al nuevo tipo de registro. Cada fila es un registro único que debe agregar.

   >[!TIP]
   >
   >    Si importa un tipo de registro desde un archivo de Excel o CSV, también se importan los registros.

   De forma predeterminada, los campos siguientes se muestran en las columnas de la vista de tabla de un tipo de registro operativo:

   * Nombre
   * Descripción
   * Fecha de inicio
   * Fecha de finalización
   * Estado

1. (Opcional) Actualice el nombre del tipo de registro en el encabezado de la página

   O

   Haga clic en **Más** icono ![](assets/more-menu.png) a la derecha del nombre del tipo de registro y haga clic en **Editar** para cambiarle el nombre o cambiar la información sobre él. Para obtener más información, consulte [Editar tipos de registros](/help/quicksilver/planning/architecture/edit-record-types.md).

1. (Opcional) Haga clic en **+ Nuevo registro** para agregar registros del tipo de registro seleccionado. Para obtener más información, consulte [Creación de registros](/help/quicksilver/planning/records/create-records.md).
1. (Opcional) Haga clic en **+** en la esquina superior derecha de la tabla para agregar más campos al tipo de registro.

   Para obtener más información sobre la creación de campos, consulte [Creación de campos](/help/quicksilver/planning/fields/create-fields.md).

1. (Opcional) Haga clic en la flecha que señala a la izquierda del nombre del tipo de registro, en el encabezado, para volver al espacio de trabajo seleccionado.

1. (Opcional) En el espacio de trabajo, haga clic y mantenga pulsada una tarjeta de tipo de registro para arrastrar y soltar el tipo de registro en un punto deseado o para moverlo a otra sección.

   Los cambios se guardan automáticamente.

   Para obtener información adicional sobre cómo agregar registros, eliminar o editar tipos de registros, o actualizar la vista en la página de tipo de registro, vea los siguientes artículos:

   * [Creación de registros](/help/quicksilver/planning/records/create-records.md)
   * [Eliminar tipos de registros](/help/quicksilver/planning/architecture/delete-record-types.md)
   * [Editar tipos de registros](/help/quicksilver/planning/architecture/edit-record-types.md)
   * [Administrar vistas de registros](/help/quicksilver/planning/views/manage-record-views.md)

## Creación de tipos de registros importando un archivo CSV o de Excel

>[!IMPORTANT]
>
>Esta funcionalidad se ha deshabilitado temporalmente desde el 21 de marzo de 2024. Se activará en una fecha posterior.

Tenga en cuenta lo siguiente al importar tipos de registros mediante un archivo CSV o de Excel:

* Cada hoja del archivo de Excel se convierte en un tipo de registro.
* Las columnas de cada hoja se convierten en los campos asociados a cada tipo de registro.
* Los campos son únicos para sus respectivos tipos de registros.
* Cada fila de cada hoja se convierte en un registro único asociado a su tipo de registro respectivo.
* Cada hoja del archivo de Excel no debe superar lo siguiente:
   * 50 000 filas
   * 500 columnas
* El archivo de Excel no debe tener más de 5 MB.
* No se admiten hojas vacías.

Para importar tipos de registros mediante un archivo de Excel:

{{step1-to-planning}}

El espacio de trabajo al que se accedió por última vez debe abrirse de forma predeterminada.

1. (Opcional) Expanda la flecha hacia abajo a la derecha del nombre de un área de trabajo existente y seleccione el área de trabajo para la que desea crear tipos de registros.
1. Clic **Añadir tipo de registro**.
1. Clic **Excel/CSV**.
1. Arrastre y suelte un archivo de Excel o CSV guardado anteriormente en el equipo, o haga clic en **Seleccione un archivo CSV o de Excel** para buscar uno.
1. Clic **Revisión de los datos**.

   El cuadro Vista previa y edición muestra la siguiente información:

   * Los nombres de las hojas o de los futuros tipos de registros se muestran en el panel izquierdo. De forma predeterminada, Workfront Planning selecciona un icono y un color para cada nuevo tipo de registro.
   * Se selecciona el primer tipo de hoja o registro y los nombres de los campos asociados a él se muestran como encabezados de columna. El tipo de cada campo está seleccionado de forma predeterminada.
   * Cada fila representa un nuevo registro. Solo se muestran los 10 primeros registros en el cuadro Vista previa y edición.

   ![](assets/preview-and-edit-box.png)

1. (Opcional) Haga clic en el nombre de cada hoja en el panel izquierdo para revisar la información que contiene.

   >[!NOTE]
   >
   >    Las hojas vacías no son compatibles y aparecen atenuadas.


1. (Opcional) Haga clic en **Seleccionar hojas para importar** menú desplegable y deseleccione las hojas que no desee importar.

   ![](assets/select-sheets-to-import-drop-down-with-unselected.png)

   Las hojas que no haya seleccionado se muestran con un fondo gris.

1. Clic **Importar** cuando esté listo para importar el archivo.

   La siguiente información se importa en Workfront Planning:

   * Nuevos tipos de registros
   * Nuevos campos asociados a cada tipo de registro
   * Nuevos registros asociados a cada tipo de registro

   Puede empezar a administrar campos y registros en las páginas de tipos de registros.

   Todas las personas con acceso a Workfront Planning ahora pueden ver y editar los tipos de registro importados y su información. <!--this will change with permissions-->

<!--## Connect record types with object types from another application

You can connect a record type and an object type from another application. This creates a read-only record type in Workfront Planning that corresponds to the object type in the other application. 

For example, you can create record types by connecting Workfront Planning record types with Workfront projects. As a result, the Workfront project object type is imported into Workfront Planning as a read-only record type. By default, the record type is named "Workfront Project." (********************)has this name changed? Lusine wanted to change it at some point***********)
    
You can import the following objects from the following applications: 

* From Workfront:

    * Projects
    * Portfolios
    * Programs
    * Company
    * Group

For more information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md). 
-->