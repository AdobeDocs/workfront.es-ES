---
title: Creación de tipos de registros
description: Los tipos de registro son los tipos de objetos de Adobe Workfront Planning. En Workfront Planning, puede crear tipos de registros personalizados que ilustren los elementos de trabajo necesarios en el ciclo de vida de su organización.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: f713e8fa72c98b6df2509e71acd7080d4df46a3a
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 1%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->
<!--this is linked to the UI in an empty workspace screen-->

# Creación de tipos de registros

{{planning-important-intro}}

Los tipos de registro son los tipos de objetos de Adobe Workfront Planning. En Workfront Planning, puede crear tipos de registros personalizados que ilustran los elementos relacionados con el trabajo necesarios en el ciclo de vida de su organización.

Para obtener más información acerca de los tipos de registros, vea [Información general sobre los tipos de registros](/help/quicksilver/planning/architecture/overview-of-record-types.md).

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
   <td role="rowheader"><p>Licencia de Adobe Workfront*</p></td>
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
   <td> <p>El administrador del grupo o de Workfront debe agregar el área de Planning a la plantilla de diseño. Para obtener más información, consulte <a href="/help/quicksilver/planning/access/access-overview.md">Resumen de acceso</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permisos</p></td>
   <td> <p>Administrar permisos en un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon
</td>
  </tr>
 </tbody>
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

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

        Para obtener más información, consulte [Crear espacios de trabajo](/help/quicksilver/planning/architecture/create-workspaces.md).

     <!--* When you import them using an Excel or CSV file. 

            >[!IMPORTANT]
            >
            >This functionality has been temporarily removed since March 21, 2024. It will be enabled at a later date.-->

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

Para obtener información acerca de cómo crear espacios de trabajo, vea [Crear espacios de trabajo](/help/quicksilver/planning/architecture/create-workspaces.md).

Para obtener información sobre los tipos de registros que se incluyen en cada plantilla, vea [Lista de plantillas de área de trabajo](/help/quicksilver/planning/architecture/workspace-templates.md).

## Crear un tipo de registro desde cero

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo donde desee crear un tipo de registro,

   O

   Desde un espacio de trabajo, expanda la flecha hacia abajo a la derecha del nombre de un espacio de trabajo existente, busque un espacio de trabajo y selecciónelo cuando se muestre en la lista.
1. (Opcional) Haga clic en **Agregar sección** para agregar una nueva sección al área de trabajo.
1. Haga clic en **Agregar tipo de registro**.

   Se abre el cuadro Agregar tipo de registro.
   <!--1. (Conditional) When creating record types by importing an Excel or CSV file is enabled, click **From scratch**. Otherwise, the **Add record type** box opens. -->

   ![](assets/add-record-type-box-with-appearance-options.png)

1. Actualice la siguiente información:

   * Sustituya &quot;Tipo de registro sin título&quot; por el nombre del tipo de registro futuro. <!--did they bring back the field label here and did they rename it to "Name"-->
   * **Descripción**: Agregue más información sobre el tipo de registro.
   * Seleccione un color y una forma para el icono asociado al tipo de registro. Haga lo siguiente:
      * Seleccione un color para identificar el nuevo tipo de registro. Es el color del icono de tipo de registro. Gris está seleccionado de forma predeterminada.
      * Seleccione un icono de la lista o empiece a escribir el nombre de un icono para describir lo que representa y, a continuación, selecciónelo cuando se muestre. Este es el icono del tipo de registro. De forma predeterminada, se selecciona un icono de archivo.

1. Haga clic en **Crear**.

   La tarjeta de tipo de registro se añade a la sección y al espacio de trabajo seleccionado.
La descripción del tipo de registro se muestra en la tarjeta.

   ![](assets/record-type-card-with-description.png)

1. (Opcional) Pase el ratón sobre la tarjeta de tipo de registro, haga clic en el icono **Más** ![](assets/more-menu.png) en la esquina superior derecha y, a continuación, haga clic en **Editar** para modificar la información sobre el tipo de registro.
1. (Opcional) Haga clic en la tarjeta de tipo de registro para abrir la página de tipo de registro.

   ![](assets/operational-record-type-blank.png)

   La página de tipo de registro se muestra en la vista de tabla de forma predeterminada. Las columnas de la tabla son campos asociados al nuevo tipo de registro. Cada fila es un registro único que debe agregar.

   <!--TIP: If you import a record type from an Excel or CSV file, records are also imported.-->

   De forma predeterminada, los campos siguientes se muestran en las columnas de la vista de tabla de un tipo de registro operativo:

   * Nombre
   * Descripción
   * Fecha de inicio
   * Fecha de finalización
   * Estado

1. (Opcional) Actualice el nombre del tipo de registro en el encabezado de la página

   O

   Haga clic en el icono **Más** ![](assets/more-menu.png) a la derecha del nombre del tipo de registro y haga clic en **Editar** para cambiarle el nombre o cambiar la información sobre él. Para obtener más información, vea [Editar tipos de registros](/help/quicksilver/planning/architecture/edit-record-types.md).

1. (Opcional) Haga clic en **+ Nuevo registro** para agregar registros del tipo de registro seleccionado. Para obtener más información, consulte [Crear registros](/help/quicksilver/planning/records/create-records.md).
1. (Opcional) Haga clic en el icono **+** en la esquina superior derecha de la tabla para agregar más campos al tipo de registro.

   Para obtener más información sobre cómo crear campos, vea [Crear campos](/help/quicksilver/planning/fields/create-fields.md).

1. (Opcional) Haga clic en la flecha que señala a la izquierda del nombre del tipo de registro, en el encabezado, para volver al espacio de trabajo seleccionado.

1. (Opcional) En el espacio de trabajo, haga clic y mantenga pulsada una tarjeta de tipo de registro para arrastrar y soltar el tipo de registro en un punto deseado o para moverlo a otra sección.

   Los cambios se guardan automáticamente.

   Para obtener información adicional sobre cómo agregar registros, eliminar o editar tipos de registros, o actualizar la vista en la página de tipo de registro, vea los siguientes artículos:

   * [Creación de registros](/help/quicksilver/planning/records/create-records.md)
   * [Eliminar tipos de registros](/help/quicksilver/planning/architecture/delete-record-types.md)
   * [Editar tipos de registros](/help/quicksilver/planning/architecture/edit-record-types.md)
   * [Administrar vistas de registros](/help/quicksilver/planning/views/manage-record-views.md)

<!--
## Create record types by importing an Excel or CSV file

>[!IMPORTANT]
>
>This functionality has been temporarily removed since March 21, 2024. It will be enabled at a later date.

Consider the following when importing record types using an Excel or CSV file: 

* Each sheet of the Excel file becomes a record type. 
* The columns of each sheet become the fields associated with each record type. 
* Fields are unique for their respective record types. 
* Each row in each sheet becomes a unique record associated with its respective record type. 
* Each sheet of the Excel file should not exceed the following: 
    * 50,000 rows
    * 500 columns
* The Excel file should not be larger than 5MB.
* Empty sheets are not supported. 

To import record types using an Excel file: 

{{step1-to-planning}}

1. Click the workspace where you want to create record types, 

    Or

    From a workspace, expand the downward-pointing arrow to the right of an existing workspace name, search for a workspace, then select it when it displays in the list.
1. Click **Add record type**. 
1. Click **Excel/CSV**.
1. Drag and drop an Excel or CSV file previously saved on your computer, or click **Select a CSV or Excel file** to browse for one. 
1. Click **Review your data**.
    
    The Preview and edit box displays with the following information: 

    * The names of the sheets or of the future record types display in the left panel. Workfront Planning selects an icon and a color for each new record type by default.
    * The first sheet or record type is selected and the names of the fields associated with it display as the column headers. The type of each field is selected by default. 
    * Each row represents a new record. Only the first 10 records display in the Preview and edit box. 

    ![](assets/preview-and-edit-box.png)

1. (Optional) Click the name of each sheet in the left panel to review the information it contains. 

    >[!NOTE]
    >
    >    Sheets that are empty are not supported and are dimmed. 


1. (Optional) Click the **Select sheets to import** drop-down menu and deselect the sheets that you don't want to import. 

    ![](assets/select-sheets-to-import-drop-down-with-unselected.png)

    Sheets you deselected display with a gray background. 

1. Click **Import** when you are ready to import your file. 

    The following information imports in to Workfront Planning:

    * New record types
    * New fields associated with each record type
    * New records associated with each record type

    You can start managing fields and records on the record types pages. 
    
    Everyone with access to Workfront Planning can now view and edit the imported record types and their information.-->

