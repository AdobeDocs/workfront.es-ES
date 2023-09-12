---
title: Creación de tipos de registros
description: Los tipos de registro son los tipos de objeto de Adobe Maestro. En Maestro, puede crear tipos de registros personalizados que ilustren los elementos de trabajo necesarios en el ciclo de vida de su organización.
hidefromtoc: true
hide: true
source-git-commit: 6e219089f68db651f5eb8369e3c6df83b6cd823b
workflow-type: tm+mt
source-wordcount: '1397'
ht-degree: 1%

---


<!--udpate the metadata with real information when making this available in TOC and in the left nav-->

# Creación de tipos de registros

>[!IMPORTANT]
>
>En la actualidad, Adobe Maestro forma parte de un programa beta cerrado que está abierto a un número limitado de clientes.
>
>Póngase en contacto con su representante de cuentas para obtener más información acerca de cómo unirse al programa beta de Maestro.
>
>Para obtener más información, consulte [Introducción a Adobe Maestro](../maestro-overview.md).

Los tipos de registro son los tipos de objeto de Adobe Maestro. En Maestro, puede crear tipos de registros personalizados que ilustran los elementos relacionados con el trabajo necesarios en el ciclo de vida de su organización.

Los tipos de registro pueden ser uno de los siguientes:

* **Tipos de registros operativos**
* **Taxonomías**

Para obtener más información acerca de los tipos de registros de Maestro, vea [Información general sobre los tipos de registros y las taxonomías](../architecture-and-fields/overview-of-record-types-and-taxonomies.md).

Crear tipos de registros operativos es similar a crear tipos de registros de taxonomía. Este artículo describe cómo crear tipos de registros operativos.

Para obtener información sobre la creación de taxonomías, consulte [Crear tipos de registros de taxonomía](../architecture-and-fields/create-a-taxonomy.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> producto de Adobe</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>acuerdo con Adobe Workfront</p></td>
   <td>
<p>Su organización debe estar inscrita en el programa beta cerrado de Adobe Maestro. Póngase en contacto con el representante de cuentas para obtener más información sobre esta nueva oferta. </p>
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
   <td role="rowheader">Nivel de acceso</td>
   <td> <p>Cualquiera</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Plantilla de diseño</td>
   <td> <p>El administrador del sistema debe agregar el área de Maestro en la plantilla de diseño. Para obtener más información, consulte <a href="../access/grant-access.md">Conceder acceso a Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Consideraciones sobre la creación de tipos de registros

* Puede crear tipos de registros en un espacio de trabajo mediante uno de los procedimientos siguientes:

   * Automáticamente:
      * Cuando se crea un espacio de trabajo mediante una plantilla.

        Para obtener más información, consulte [Creación de espacios de trabajo](../architecture-and-fields/create-workspaces.md).
      * Cuando se importan mediante un archivo CSV o de Excel. Esto no está disponible para tipos de registros de taxonomía.
      * Cuando se crea una conexión a tipos de objeto desde otra aplicación, al agregar campos a un tipo de registro. Esto crea un tipo de registro de sólo lectura en Maestro que está conectado a los tipos de objeto de la aplicación original. Esto no está disponible para tipos de registros de taxonomía.

     Para obtener información acerca de cómo conectar tipos de objetos con registros Maestro, vea [Conectar registros](../records/connect-records.md).
   * Manualmente:

      * Desde cero.

## Creación de tipos de registros con una plantilla de Workspace

Puede crear tipos de registros automáticamente al crear un espacio de trabajo con una plantilla. Cada plantilla de Maestro contiene ejemplos de tipos de registros operativos y de taxonomía.

Para obtener información sobre la creación de espacios de trabajo, consulte [Creación de espacios de trabajo](../architecture-and-fields/create-workspaces.md).

Para obtener información sobre los tipos de registros que se incluyen con cada plantilla, consulte [Lista de plantillas de Workspace](../architecture-and-fields/workspace-templates.md).

## Crear un tipo de registro desde cero

Este artículo describe cómo crear tipos de registros operativos desde cero. Crear tipos de registros operativos desde cero es similar a crear taxonomías.

Para obtener más información sobre las taxonomías, consulte [Creación de una taxonomía](../architecture-and-fields/create-a-taxonomy.md).

1. Haga clic en **Menú principal** icono ![](assets/main-menu-workfront.png) en la esquina superior derecha de Workfront, <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> luego haga clic en **Maestro** ![](assets/maestro-icon.png).

   El espacio de trabajo al que se accedió por última vez debe abrirse de forma predeterminada.

1. (Opcional) Expanda la flecha hacia abajo a la derecha del nombre de un área de trabajo existente y seleccione el área de trabajo para la que desea crear tipos de registros.
1. Clic **Añadir tipo de registro**.
1. (Condicional) Si está creando un tipo de registro operativo, haga clic en **Desde cero**. Esta opción no está disponible al crear taxonomías.

   Se abre el cuadro Agregar tipo de registro.

   ![](assets/add-record-type-box-with-appearance-options.png)

1. Seleccione la siguiente información:

   * **Nombre de registro**: reemplace &quot;Tipo de registro operativo sin título&quot; por el nombre del tipo de registro futuro. <!--correct this - I asked Garik to change this field to "Record type name"-->
   * **Aspecto**: defina el color y la forma del icono asociado al tipo de registro. Haga lo siguiente:
      * Seleccione un color para identificar el nuevo tipo de registro. Es el color del icono de tipo de registro. Gris está seleccionado de forma predeterminada.
      * Seleccione un icono de la lista o empiece a escribir el nombre de un icono para describir lo que representa y, a continuación, selecciónelo cuando se muestre. Este es el icono del tipo de registro. De forma predeterminada, se selecciona un icono de archivo.

1. Haga clic fuera de **Añadir tipo de registro** para guardar el registro.

   La tarjeta de tipo de registro se añade al espacio de trabajo seleccionado.
El número de campos que contiene el tipo de registro se muestra en la tarjeta.
1. (Opcional) Haga clic en la tarjeta de tipo de registro para abrir la página de tipo de registro.

   ![](assets/operational-record-type-blank.png)

   La página de tipo de registro se muestra en la vista Tabla de forma predeterminada. Las columnas de la tabla son campos asociados al nuevo tipo de registro. Cada fila es un registro único que debe agregar.

   De forma predeterminada, los campos siguientes se muestran en las columnas de la vista de tabla de un tipo de registro operativo:

   * Nombre

     El campo Nombre es el único campo creado automáticamente para las taxonomías.
   * Descripción
   * Fecha de inicio
   * Fecha de finalización
   * Estado

1. (Opcional) Actualice el nombre del tipo de registro en el encabezado de la página

   O

   Haga clic en **Más** icono ![](assets/more-menu.png) a la derecha del nombre del tipo de registro y haga clic en **Cambiar nombre** para cambiarle el nombre.

1. (Opcional) Haga clic en **+ Nuevo &lt; nombre de tipo de registro >** para agregar registros del tipo de registro seleccionado. Para obtener más información, consulte [Creación de registros](../records/create-records.md).
1. (Opcional) Haga clic en **+** en la esquina superior derecha de la tabla para agregar más campos al tipo de registro. Para obtener más información, consulte [Creación de campos](../architecture-and-fields/create-fields.md).
1. (Opcional) Haga clic en la flecha que señala a la izquierda del nombre del tipo de registro para volver al espacio de trabajo seleccionado.

   La tarjeta de tipo de registro muestra el número de campos y conexiones que contiene el tipo de registro.

   ![](assets/campaign-card-with-fields-and-connections-highlighted.png)

   Para obtener información adicional sobre cómo agregar registros, eliminar o editar tipos de registros, o actualizar la vista en la página de tipo de registro, vea los siguientes artículos:

   * [Creación de registros](../records/create-records.md)
   * [Eliminar tipos de registros](../architecture-and-fields/delete-record-types.md)
   * [Editar tipos de registros](../architecture-and-fields/edit-record-types.md)
   * [Administrar vistas de registros en Adobe Maestro](../views/manage-record-views.md) <!--add information here about the sorting and grouping when available-->

## Creación de tipos de registros importando un archivo CSV o de Excel

Tenga en cuenta lo siguiente al importar tipos de registros mediante un archivo CSV o de Excel:

* Cada hoja del archivo de Excel se convierte en un tipo de registro en Maestro.
* Las columnas de cada hoja se convierten en los campos asociados a cada tipo de registro.
* Los campos son únicos para sus respectivos tipos de registros.
* Cada fila de cada hoja se convierte en un registro único asociado a su tipo de registro respectivo.
* Cada hoja del archivo de Excel no debe superar lo siguiente:
   * 10 000 filas
   * 500 columnas
* El archivo de Excel no debe tener más de 5 MB.
* No se admiten hojas vacías.

Para importar tipos de registros mediante un archivo de Excel:

1. Haga clic en **Menú principal** icono ![](assets/main-menu-workfront.png) en la esquina superior derecha de Workfront, <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> luego haga clic en **Maestro** ![](assets/maestro-icon.png).

   El espacio de trabajo al que se accedió por última vez debe abrirse de forma predeterminada.

1. (Opcional) Expanda la flecha hacia abajo a la derecha del nombre de un área de trabajo existente y seleccione el área de trabajo para la que desea crear tipos de registros.
1. Clic **Añadir tipo de registro**.
1. (Condicional) Si está creando un tipo de registro operativo, haga clic en **Excel/CSV**.

   >[!NOTE]
   >
   >    Esta opción no está disponible al crear tipos de registros de taxonomía.

1. Arrastre y suelte un archivo de Excel o CSV guardado anteriormente en el equipo, o haga clic en **Seleccione un archivo CSV o de Excel** para buscar uno.
1. Clic **Revisión de los datos**.

   El cuadro Vista previa y edición muestra la siguiente información:

   * Los nombres de las hojas o de los futuros tipos de registros se muestran en el panel izquierdo. Maestro selecciona de forma predeterminada un icono y un color para cada nuevo tipo de registro.
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

   La siguiente información se importa en Maestro:

   * Nuevos tipos de registros
   * Nuevos campos asociados a cada tipo de registro
   * Nuevos registros asociados a cada tipo de registro

   Puede empezar a administrar campos y registros en las páginas de tipos de registros.

   Todas las personas con acceso a Maestro ahora pueden ver y editar los tipos de registro importados y su información. <!--this will change with permissions-->

## Conectar tipos de registros con tipos de objetos de otra aplicación

Puede importar tipos de registro cuando cree una conexión entre un tipo de registro Maestro y un tipo de objeto de otra aplicación. Esto crea un tipo de registro de sólo lectura en Maestro que corresponde al tipo de objeto de la aplicación de terceros.

Por ejemplo, puede crear tipos de registros conectando los tipos de registros de Maestro con proyectos de Workfront. Como resultado, el tipo de objeto de proyecto de Workfront se importa en Maestro como un tipo de registro de sólo lectura. De forma predeterminada, el tipo de registro se denomina &quot;Proyecto de Workfront&quot;. <!--has this name changed? Lusine wanted to change it at some point-->

Se pueden importar los objetos siguientes desde las aplicaciones siguientes:

* Desde Workfront:

   * Proyectos
   * Portafolios
   * Programas

Para obtener más información, consulte [Conectar tipos de registros](../architecture-and-fields/connect-record-types.md).








