---
title: Creación de registros
description: Al utilizar la planificación de Adobe Workfront, un registro es una instancia de un tipo de registro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: a0f12a016ae8ac73136f05bf3255f9882e2ce6d4
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Creación de registros

{{maestro-important-intro}}

En la planificación de Adobe Workfront, un registro es una instancia de un tipo de registro.

Para crear registros, siga uno de estos procedimientos:

* Crearlos manualmente para tipos de registros
* Crear registros copiando y pegando información de una lista externa.

Este artículo describe cómo crear registros. Para obtener información acerca de la administración de registros en las vistas de tabla o escala de tiempo, vea los siguientes artículos:

* [Administrar la vista de tabla](/help/quicksilver/maestro/views/manage-the-table-view.md)
* [Administrar la vista de cronología](/help/quicksilver/maestro/views/manage-the-timeline-view.md)

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
<p>Su organización debe estar inscrita en el programa beta de planificación de Adobe Workfront. Póngase en contacto con el representante de cuentas para obtener más información sobre esta nueva oferta. </p>
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
   <p>Cualquiera</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuraciones de nivel de acceso</p></td>
   <td> <p>No hay controles de acceso para la planificación de Adobe Workfront </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permisos</p></td>
   <td> <p>Permisos de contribución o superiores en un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>El administrador del grupo o de Workfront debe agregar el área de Planning a la plantilla de diseño. Para obtener más información, consulte <a href="../access/access-overview.md">Acceso a información general</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Crear registros agregándolos manualmente a un tipo de registro <!--in a record type table (I don't think you can create them elsewhere right now)-->

Puede crear registros en la vista de tabla de una página de tipo de registro.

Para obtener información sobre cómo editar la información de registro, consulte [Edición de registros](/help/quicksilver/maestro/records/edit-records.md).

{#step1-to-maestro}

El espacio de trabajo al que se accedió por última vez se abre de forma predeterminada. Para obtener información sobre la creación de espacios de trabajo, consulte [Creación de espacios de trabajo](../architecture/create-workspaces.md).

1. Haga clic en una tarjeta de tipo de registro. Para obtener información sobre cómo crear un tipo de registro, consulte [Creación de tipos de registros](../architecture/create-record-types.md).

   La página de tipo de registro se abre en la vista a la que se accedió por última vez. De forma predeterminada, se abre una página de tipo de registro en la vista de tabla.
Todos los registros del tipo seleccionado se muestran en la vista de tabla.

1. (Condicional) Si la página de tipo de registro no se abre en la vista de tabla, haga clic en la ficha de una vista de tabla o en **+ Ver** para crear una vista de tabla.

1. Para añadir nuevos registros, haga clic en **Nuevo registro** en la última fila de la tabla

   O

   Clic **Mayús + Intro** en el teclado desde cualquier columna o fila de la tabla. Esto añade una fila vacía.

   ![](assets/adding-a-new-campaign-in-table-row.png)

1. Empiece a escribir información en la nueva fila sobre el nuevo registro.

   >[!NOTE]
   >
   >  * No hay campos obligatorios para los registros. Sin embargo, se recomienda agregar un Nombre para el registro, ya que es útil identificar registros al vincularlos entre sí.
   >
   >  * Los campos que hacen referencia a otros tipos de registro o campos calculados son campos de sólo lectura.

1. Siga agregando información en cada fila y haga clic en **Entrar** en el teclado para guardar los cambios.

   O

   Haga clic en el nombre del nuevo registro o en el icono **Abrir detalles** icono ![](assets/open-details-icon-in-table-name-field.png) a la izquierda del nombre del registro. El **Detalles** se abre en la tabla.

   >[!TIP]
   >
   >Solo puede tener acceso al cuadro Detalles desde el campo de nombre del registro cuando el campo Nombre es un campo principal.

1. Comience a editar la información del registro en el cuadro Detalles. Workfront guarda automáticamente los cambios.
1. (Opcional) Haga clic en **Abrir en ficha nueva** icono ![](assets/open-details-in-a-new-tab-icon.png) en la esquina superior derecha del cuadro Detalles para abrir el **Detalles** en una nueva pestaña. Continúe editando el registro en la página Detalles.


1. (Opcional) Utilice los siguientes métodos abreviados del teclado para deshacer o rehacer la adición de nuevos registros:

   * CTRL + Z (⌘ + Z para Mac) para deshacer un cambio
   * CTRL + Mayús + Z (⌘ + Mayús + Z para Mac) para rehacer un cambio

<!-- this is not possible anymore: 

## Create records by connecting them from another application

You can import records from other applications by linking them to existing records. This creates a linked record for the other application's connected object. 

1. Create a record type, as described in the [Create record types](../architecture/create-record-types.md).

1. Create records for the record type you created in the previous step. For information, see the section [Create records by manually adding them to a record type](#create-records-by-manually-adding-them-to-a-record-type) in this article. 

1. Create a connection to an object type from another application for the record type you created. For information, see [Connect record types](../architecture/connect-record-types.md).

1. Add objects from another application to the records you created above using the linked record field you created in the previous step. For information, see [Connect records](../records/connect-records.md). 

    The following items are created in Maestro:

    * A read-only Maestro record type that refers to the other application's record type you linked to in the connected record field. 

      For example, if you connect a Maestro record type to Workfront project, a read-only record type named "Workfront project" is created in the same workspace. You can access the read-only Workfront record types from the table view of the Maestro records you're linking from. 
   
-->

## Crear registros copiando y pegando información de una lista externa

1. Comience a crear registros en la vista Tabla, tal como se describe en la sección [Crear registros agregándolos manualmente a un tipo de registro](#create-records-by-manually-adding-them-to-a-record-type) en este artículo.

   Asegúrese de que la vista de tabla tiene las columnas (o los campos) que desea rellenar con la información del nuevo registro.

1. Clic **Nuevo &lt; Nombre del tipo de registro >** en la última fila de la tabla para agregar a la tabla tantas filas nuevas como desee que estén los registros nuevos.

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

   Se ha importado la siguiente información en el área de planificación de Workfront:

   * Las filas contienen los registros nuevos
   * Las columnas rellenan la información de los campos de los registros.
