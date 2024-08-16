---
title: Creación de registros
description: Al utilizar Adobe Workfront Planning, un registro es una instancia de un tipo de registro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: 57e0fe65180cec3fab5cb10b3afbc0ac0a1dbb55
workflow-type: tm+mt
source-wordcount: '930'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Creación de registros

{{planning-important-intro}}

En Adobe Workfront Planning, un registro es una instancia de un tipo de registro.

Para crear registros, siga uno de estos procedimientos:

* Añádalos desde la página de tipo de registro
* Copiar y pegar una lista de registros de una lista externa
* Duplicarlos
  <!--* Add them as you connect them from other records-->

Este artículo describe cómo crear registros. Para obtener información acerca de la administración de registros en las vistas de tabla o escala de tiempo, vea los siguientes artículos:

* [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md)
* [Administrar la vista de cronología](/help/quicksilver/planning/views/manage-the-timeline-view.md)

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
   <p>Actual: plan</p>  
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuraciones de nivel de acceso</p></td>
   <td> <p>No hay controles de acceso para Adobe Workfront Planning </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permisos</p></td>
   <td> <p>Permisos de Contribute o superiores para un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>El administrador del grupo o de Workfront debe agregar el área de Planning a la plantilla de diseño. Para obtener más información, consulte <a href="/help/quicksilver/planning/access/access-overview.md">Resumen de acceso</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Para obtener más información, consulte [Requisitos de acceso para la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/planning/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Crear registros agregándolos a un tipo de registro <!--in a record type table (I don't think you can create them elsewhere right now)-->

Puede crear registros en la vista de tabla de una página de tipo de registro.

Para obtener información acerca de cómo editar información de registro, vea [Editar registros](/help/quicksilver/planning/records/edit-records.md).

{{step1-to-planning}}

1. Haga clic en el área de trabajo donde desee agregar registros.

   El espacio de trabajo se abre y los tipos de registro se muestran como tarjetas.

1. Haga clic en una tarjeta de tipo de registro. Para obtener información acerca de cómo crear un tipo de registro, vea [Crear tipos de registros](/help/quicksilver/planning/architecture/create-record-types.md).

   La página de tipo de registro se abre en la vista a la que se accedió por última vez. De forma predeterminada, se abre una página de tipo de registro en la vista de tabla.
Todos los registros del tipo seleccionado se muestran en la vista.

1. (Condicional) Según la vista que muestre, siga uno de estos procedimientos:

   * Desde la vista de tabla:

      * Haga clic en **Nuevo registro** en la última fila de la tabla

      * Haz clic en **Mayús + Intro** en el teclado desde cualquier columna o fila de la tabla. Esto agrega una fila vacía debajo del registro desde el que comienza.
      * Pase el ratón sobre el campo principal de un registro, haga clic en el menú **Más** ![](assets/more-menu.png) que se encuentra a la derecha del campo y, a continuación, haga clic en **Insertar registro arriba** o **Insertar registro abajo**.

     ![](assets/adding-a-new-campaign-in-table-row.png)

   * Desde cualquier vista:

      * Haga clic en **Nuevo registro** en la esquina superior derecha de la página. Se abre el cuadro de vista previa de registros.

     Workfront carga automáticamente una miniatura y una imagen de portada en cada nuevo registro. Puede modificar estas imágenes más adelante. Para obtener más información, consulte los siguientes artículos:

      * [Agregar una imagen de portada a un registro](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md)
      * [Añadir una miniatura en un registro](/help/quicksilver/planning/records/add-thumbnails-to-records.md)

1. Empiece a escribir información sobre el nuevo registro en los campos que ve en el cuadro de vista previa.

   >[!NOTE]
   >
   >  * No hay campos obligatorios para los registros. Sin embargo, se recomienda agregar información para el campo principal de un registro, ya que es útil identificar registros al vincular registros entre sí. Para obtener más información acerca de los campos principales, vea [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md) y [Información general del campo principal](/help/quicksilver/planning/fields/primary-field-overview.md).
   >
   >  * Los campos que hacen referencia a otros tipos de registro o campos calculados son campos de sólo lectura.

1. (Condicional) Cuando agregue registros a la tabla, siga agregando información en cada fila y, a continuación, haga clic en **Escribir** en el teclado para guardar los cambios.

   O

   Haga clic en el nombre del nuevo registro o en el icono **Abrir detalles** ![](assets/open-details-icon-in-table-name-field.png) que aparece a la izquierda del nombre del registro. Se abrirá en la tabla una vista previa con la información detallada del registro.

   >[!TIP]
   >
   >Solo puede obtener acceso al icono **Abrir detalles** desde el campo de nombre del registro cuando el campo Nombre es un campo principal.

1. Comience a editar la información del registro en la vista previa del registro. Workfront guarda automáticamente los cambios.
1. (Opcional) Haga clic en el icono **Abrir en ficha nueva** ![](assets/open-details-in-a-new-tab-icon.png) en la esquina superior derecha de la vista previa del registro para abrir la página del registro en una ficha nueva. Continúe editando el registro en la página de registros. Para obtener más información, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

1. (Opcional) Utilice los siguientes métodos abreviados del teclado para deshacer o rehacer la adición de nuevos registros o su información al agregarlos en la vista de tabla:

   * CTRL + Z (⌘ + Z para Mac) para deshacer un cambio
   * CTRL + Mayús + Z (⌘ + Mayús + Z para Mac) para rehacer un cambio

<!-- this is not possible anymore: 

## Create records by connecting them from another application

You can import records from other applications by linking them to existing records. This creates a linked record for the other application's connected object. 

1. Create a record type, as described in the [Create record types](/help/quicksilver/planning/architecture/create-record-types.md).

1. Create records for the record type you created in the previous step. For information, see the section [Create records by manually adding them to a record type](#create-records-by-manually-adding-them-to-a-record-type) in this article. 

1. Create a connection to an object type from another application for the record type you created. For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).

1. Add objects from another application to the records you created above using the linked record field you created in the previous step. For information, see [Connect records](/help/quicksilver/planning/records/connect-records.md). 

    The following items are created in Workfront Planning:

    * A read-only record type that refers to the other application's record type you linked to in the connected record field. 

      For example, if you connect a Planning record type to Workfront project, a read-only record type named "Workfront project" is created in the same workspace. You can access the read-only Workfront record types from the table view of the Planning records you're linking from. 
   
-->

## Crear registros copiándolos y pegándolos desde una lista externa

1. Comience a crear registros en la vista Tabla, tal como se describe en la sección [Crear registros agregándolos manualmente a un tipo de registro](#create-records-by-manually-adding-them-to-a-record-type) en este artículo.

   Asegúrese de que la vista de tabla tiene las columnas (o los campos) que desea rellenar con la información del nuevo registro.

1. Haga clic en **Nuevo &lt; Nombre de tipo de registro >** en la última fila de la tabla para agregar tantas filas nuevas a la tabla como desee que sean los registros nuevos.

   Por ejemplo, agregue 10 filas a la vista de tabla si desea pegar la información de 10 registros nuevos de otra aplicación.

1. En otra aplicación, cree una lista de registros que desee importar.

   Por ejemplo, puede utilizar una hoja de cálculo de Excel para crear la lista.

   La lista debe contener información en formato tabular.

   >[!TIP]
   >
   > Las columnas de la lista deben contener información sobre los campos existentes que tiene en Workfront.
   >
   > Asegúrese de que ya ha creado los campos deseados en Workfront y de que la información de la hoja se muestra en el formato correcto que coincide con el de cada campo en Workfront.

1. Desde otra aplicación, seleccione varias filas y columnas y pegue la información en la vista de tabla de tipo de registro, empezando por el primer registro nuevo.

   Se ha importado la siguiente información en el área de Workfront Planning:

   * Las filas contienen los registros nuevos
   * Las columnas rellenan la información de los campos de los registros.

## Creación de registros duplicándolos

Para obtener información sobre la duplicación de registros, vea [Registros duplicados](/help/quicksilver/planning/records/copy-or-duplicate-records.md).

<!--check the steps with the release of in-context record types epic: 

## Create records as you connect them

You can create records as you connect them from other records. 

You must have the following before you can add new records by connecting them from existing records:

* Connected record types. For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).
* Connected records. For information, see [Connect records](/help/quicksilver/planning/records/connect-records.md).

To create records as you are connecting them from other records: 

1. Start connecting Workfront Planning records, as described in the article [Connect records](/help/quicksilver/planning/records/connect-records.md). 
1. (Conditional) If you cannot find a record when trying to add it from the connected record field of another record, search for a record, then click **+ Add**. The **+ Add** button is followed by the name of the record type you are connecting from. 

    ![](assets/add-button-to-create-records-in-context-highlighted.png)

    The record is created and added to the connected record field. 
1. (Optional) Go to the table view of the record type whose record you created. A new record displays in the last row of the view. 
1. (Optional) Start adding information for the new record in the table view, or click its name to open the details page and add information there. 

-->