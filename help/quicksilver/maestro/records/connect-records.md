---
title: Conectar registros
description: Después de crear conexiones entre tipos de registros, puede conectar registros individuales entre sí.
hidefromtoc: true
hide: true
source-git-commit: 71ce412ead1590b8511ec4219d3ba72fbf32b98d
workflow-type: tm+mt
source-wordcount: '1804'
ht-degree: 0%

---


<!--when you make this live, update the metadata above to this: 
---
title: Connect records and objects
description: In addition to connecting Maestro records to one another, you can also connect Maestro records to objects from other applications.  
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->
<!--udpate the metadata with real information when making this available in TOC and in the left nav-->

<!--if you change steps here, also update steps in the "Connect records" article-->

# Conectar registros

>[!IMPORTANT]
>
>En la actualidad, Adobe Maestro forma parte de un programa beta cerrado que está abierto a un número limitado de clientes.
>
>Póngase en contacto con su representante de cuentas para obtener más información acerca de cómo unirse al programa beta de Maestro.
>
>Para obtener más información, consulte [Introducción a Adobe Maestro](../maestro-overview.md).

Puede conectar los registros de Adobe Maestro entre sí o con objetos de otras aplicaciones.

Primero debe conectar dos tipos de registro o un tipo de registro a un tipo de objeto de otra aplicación y, a continuación, puede utilizar la vista Tabla del tipo de registro para conectar registros entre sí o registros a otros objetos.

Para obtener información sobre cómo conectar tipos de registros entre sí o con tipos de objetos de otras aplicaciones, vea [Conectar tipos de registros](../architecture-and-fields/connect-record-types.md).

Para ver un ejemplo de tipos de registros de conexión, consulte [Ejemplo de conexión de tipos y registros](../architecture-and-fields/example-connect-record-types-and-records.md).

Puede conectar lo siguiente:

* Registros operativos de Maestro
* Registros operativos de Maestro a registros de taxonomía
* Registros operativos y objetos de otras aplicaciones de Maestro.

  Actualmente se admiten las siguientes aplicaciones y tipos de objetos:

   * Adobe Workfront

      * Proyectos
      * Portafolios
      * Programas
      * Compañía
      * Grupo

  <!--when you add more objects, fix the Access Requirements below which right now refer only to projects-->

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
   <td><p>Cualquiera, para crear registros de Maestro</p> 
<p>Trabaje o superior para ver proyectos en Workfront</p>
  <p>Para obtener más información, consulte <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">Resumen de licencias de Adobe Workfront</a>.</p> 
  </td>
  </tr>
  <tr>
   <td role="rowheader">Nivel de acceso</td>
   <td> <p>Cualquiera, para crear registros de Maestro</p>
<p>Acceso de visualización o superior a Proyectos, Portfolio y Programas</p> 
<p>Acceso adicional a Grupos y Compañías, cuando los usuarios de grupos o empresas de visualización no pertenecen a</p>   
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permisos de objeto</p></td>
   <td> <p>Ver o permisos superiores a los objetos que desea vincular con registros de Maestro  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>El administrador del sistema debe agregar el área de Maestro en la plantilla de diseño. Para obtener más información, consulte <a href="../access/grant-access.md">Conceder acceso a Adobe Maestro</a>. </p></td>
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

## Conectar registros

### Consideraciones sobre la conexión de registros

* Una vez establecida la conexión entre tipos de registro, los tipos de registro conectados se muestran como campos de registro vinculados en la tabla de los tipos de registro desde los que están vinculados.
* Puede examinar y agregar registros y objetos de los tipos de registro y objeto vinculados desde los campos de registro vinculados.
* Puede agregar campos de los tipos de registro vinculados a la tabla del tipo de registro desde el que está vinculando.
* No se pueden actualizar manualmente los valores de los campos vinculados en los registros desde los que se está vinculando.

  Los valores de los campos vinculados de los registros vinculados rellenan automáticamente el registro de Maestro desde el que está estableciendo el vínculo.

* Todas las personas con acceso a Maestro pueden ver las conexiones que establece entre los registros de Maestro o entre los registros de Maestro y los objetos de Workfront. Además, puede ver y editar las conexiones de todos los demás. <!--add that this is based on your permissions in both Maestro and Workfront (or, later, any other application)-->
* Puede conectar un registro Maestro a uno o varios objetos de otra aplicación.
* No se pueden conectar taxonomías a tipos de registros ni a objetos de otra aplicación. <!-- this is temporary; there will be certain objects (teams, etc) that will be linked to taxonomies, per Lilit-->
* Actualmente, sólo puede vincular registros de Maestro a objetos de Workfront. Para vincular registros de Maestro con objetos de Workfront, debe tener lo siguiente:

   * Objetos Workfront. Por ejemplo, primero debe crear proyectos, portafolios, programas, empresas o grupos en Workfront.
   * Espacios de trabajo de Maestro, tipos de registros y registros. Para obtener más información, consulte los siguientes artículos:

      * [Creación de espacios de trabajo](../architecture-and-fields/create-workspaces.md)
      * [Creación de tipos de registros](../architecture-and-fields/create-record-types.md)
      * [Creación de registros](../records/create-records.md)

   * Conexiones entre tipos de registro o entre tipos de registro y objetos de otras aplicaciones. Para obtener más información, consulte [Conectar tipos de registros](../architecture-and-fields/connect-record-types.md).

### Conectar registros de Maestro

1. Haga clic en **Menú principal** icono ![](assets/main-menu-workfront.png) en la esquina superior derecha de Workfront, <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> luego haga clic en **Maestro** ![](assets/maestro-icon.png).

   El espacio de trabajo al que se accedió por última vez debe abrirse de forma predeterminada.

1. (Opcional) Expanda la flecha hacia abajo a la derecha del nombre de un área de trabajo existente y seleccione el área de trabajo desde la que desea conectar registros.
1. Haga clic en la tarjeta de un tipo de registro para abrir la página del tipo de registro.
1. Seleccione una Vista de tabla de la **Ver** menú desplegable en la esquina superior derecha de la página tipo de registro.
1. Agregar una conexión a otro tipo de registro u objeto desde el tipo de registro seleccionado. Para obtener más información, consulte [Conectar tipos de registros](../architecture-and-fields/connect-record-types.md).

Se agrega una nueva columna a la tabla para mostrar el tipo de registro vinculado.

1. Agregue registros al tipo de registro seleccionado agregando una nueva fila a la tabla. Para obtener más información, consulte [Creación de registros](../../maestro/records/create-records.md).
1. Desde un registro enumerado en la vista de tabla, vaya a la columna de registro vinculada, pase el ratón sobre la celda correspondiente al registro que desea vincular con otros registros de Maestro y, a continuación, haga clic en el botón **+** icono.

   El **Conectar objetos** aparece el cuadro.

   ![](assets/connected-objects-table-for-records.png)

1. Comience a escribir el nombre de un registro en el cuadro de búsqueda y, a continuación, selecciónelo cuando aparezca en la lista

   O

   Seleccione el nombre de uno o varios registros en el cuadro y haga clic en **Conectar objetos** en la esquina superior derecha del cuadro Conectar objetos.

   Se añaden los elementos siguientes:

   * Los registros vinculados se muestran en el campo de registro vinculado del registro seleccionado en el paso 3. Al actualizar los registros vinculados, se actualizan automáticamente los campos de registro vinculados de los registros desde los que está vinculando. <!--ensure the number of the step stays accurate-->
   * Los campos vinculados que pertenecen a los registros vinculados se rellenan automáticamente con la información de los registros vinculados originales. Los campos vinculados no se pueden editar manualmente.

     >[!TIP]
     >
     >* Utilizamos &quot;campos vinculados&quot; y &quot;campos de búsqueda&quot; indistintamente.
     >
     >* Si habilitó la opción Permitir varios registros al conectar los tipos de registro, los valores de los campos de los objetos seleccionados se mostrarán separados por comas o se agregarán según el agregador elegido.

1. (Opcional) Cierre la página de tipo de registro de Maestro y vaya al espacio de trabajo seleccionado.
1. Haga clic en la tarjeta del tipo de registro al que está vinculado.

   Por ejemplo, si conectó el registro de Campaign con el registro de producto, haga clic en **Product** Tarjeta de.

   La tarjeta de tipo de registro se debe abrir en la vista Tabla.

   Observe que el campo de registro Campaña vinculada muestra los nombres de las campañas vinculadas a los productos en la página Tipo de registro de producto. Al actualizar la información de Campaign, se actualiza automáticamente el campo de registro vinculado de Campaign para el tipo de registro de producto.

### Conectar registros de Maestro a objetos de Workfront

<!--when we will have more applications to link to from Maestro, change the title to soemthing like: Connect Maestro records to objects from other applications-->

Después de crear una conexión entre un tipo de registro Maestro y un tipo de objeto Workfront, puede conectar registros individuales de Maestro a objetos de Workfront. También puede conectar campos del objeto Workfront al tipo de registro Maestro.

1. Haga clic en **Menú principal** icono ![](assets/main-menu-workfront.png) en la esquina superior derecha de Workfront, <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> luego haga clic en **Maestro** ![](assets/maestro-icon.png).

   El espacio de trabajo al que se accedió por última vez debe abrirse de forma predeterminada.

1. (Opcional) Expanda la flecha hacia abajo a la derecha del nombre de un área de trabajo existente y seleccione el área de trabajo desde la que desea conectar registros.
1. Haga clic en la tarjeta de un tipo de registro para abrir la página del tipo de registro.
1. Seleccione una Vista de tabla de la **Ver** menú desplegable en la esquina superior derecha de la página tipo de registro.
1. Agregar una nueva conexión a un tipo de objeto desde Workfront con el tipo de registro seleccionado. Seleccione entre los siguientes objetos de la sección Workfront:

   * Proyecto
   * Portafolio
   * Programar
   * Compañía
   * Grupo

   Para obtener más información, consulte [Conectar tipos de registros](../architecture-and-fields/connect-record-types.md).

   Se agrega una nueva columna a la tabla para mostrar el tipo de objeto vinculado.

1. Agregue registros individuales al tipo de registro seleccionado agregando una nueva fila a la tabla. Para obtener más información, consulte [Creación de registros](../../maestro/records/create-records.md).
1. Desde un registro enumerado en la vista de tabla, vaya a la columna de objeto vinculado, pase el ratón sobre la celda correspondiente al registro que desea vincular con otros objetos de Workfront y, a continuación, haga clic en **+** icono. <!--change Workfront to other applications, when this will be possible-->

   El **Conectar objetos** aparece el cuadro.

   ![](assets/connect-objects-box-to-select-projects.png)

1. Comience a escribir el nombre de un objeto de Workfront en el cuadro de búsqueda y, a continuación, selecciónelo cuando se muestre en la lista

   O

   Seleccione el nombre de uno o varios objetos en el cuadro y haga clic en **Conectar objetos** en la esquina superior derecha del cuadro Conectar objetos.

   Se agregarán los siguientes elementos a Maestro:

   * Los objetos Workfront seleccionados se agregan al campo de registro vinculado.
   * Se crea un nuevo campo vinculado (o un campo de búsqueda) para cada campo vinculado que seleccionó al agregar los campos al registro vinculado.
   * Se crea un nuevo tipo de registro denominado &quot;objeto Workfront&quot; en el mismo área de trabajo que el registro de Maestro desde el que está estableciendo el vínculo. El nombre del objeto forma parte del nombre de este tipo de registro. Por ejemplo, al vincular a proyectos de Workfront se crea el tipo de registro de proyecto de Workfront en Maestro.

     Es un tipo de registro de sólo lectura y muestra los objetos de Workfront seleccionados en el nuevo campo de objeto vinculado creado a partir del registro Maestro. Los campos vinculados del objeto vinculado también se muestran en los registros de Workfront vinculados de solo lectura.

     >[!IMPORTANT]
     >
     > El tipo de registro de objeto de Workfront de sólo lectura sólo se crea cuando se agregan proyectos individuales a registros de Maestro. La simple creación de una conexión entre un tipo de registro Maestro y un tipo de objeto Workfront no crea el tipo de registro Workfront.

     Cualquier información existente de los campos de los objetos de Workfront se muestra en los campos vinculados o de búsqueda.

     >[!TIP]
     >
     >
     >* Si habilitó la configuración Permitir varios registros, los valores de los objetos múltiples se mostrarán separados por comas o se agregarán según el agregador elegido.
     >
     >* No se crea un campo de registro vinculado a los registros vinculados de Maestro para los objetos vinculados de Workfront.


1. (Opcional) Cierre la página de tipo de registro de Maestro y vaya al espacio de trabajo seleccionado.
1. Haga clic en la tarjeta del tipo de registro de objeto de Workfront. Por ejemplo, haga clic en **proyecto de Workfront** , si ha vinculado proyectos de Workfront. La tarjeta de tipo de registro Workfront de solo lectura se debe abrir en la vista Tabla.

   >[!NOTE]
   >
   >    * Los registros enumerados en la página de tipo de registro de Workfront son objetos Workfront de sólo lectura. Los campos vinculados del tipo de registro Workfront también se muestran como columnas de solo lectura y se rellenan automáticamente cuando se rellenan en Workfront.
   >    * Los campos de Workfront no se pueden actualizar manualmente en Maestro. Los campos de objeto de Workfront deben rellenarse en Workfront y los valores de los campos se mostrarán automáticamente en el registro de Workfront en Maestro.
   >
   >    * Para mostrar el tipo de registro de objeto de Workfront en la vista Línea de tiempo, debe haber al menos dos campos de fecha en la vista Tabla de la página de tipo de registro de Workfront de sólo lectura.

1. (Opcional) Haga clic en **Más** menú ![](assets/more-menu.png) junto al nombre del tipo de registro de objeto de Workfront en el encabezado de la página, haga clic en **Cambiar nombre** para editar el nombre del registro.

   >[!NOTE]
   >
   >    No se puede eliminar un tipo de registro de Workfront vinculado ni ningún objeto de la página de tipo de registro de Workfront.

1. (Opcional) Haga clic en **Añadir campos** icono ![](assets/add-fields-icon.png) en la esquina superior derecha de la vista de tabla de la página tipo de registro de Workfront, para agregar o quitar campos de Workfront del tipo de registro de Workfront.

   >[!NOTE]
   >
   >  Los campos que agregue o quite en la página de tipo de registro de objeto de Workfront no se agregarán ni quitarán del tipo de registro de Maestro que vincula al tipo de objeto de Workfront. Los campos sólo están visibles en la página de sólo lectura de tipo de registro de Workfront, por lo que puede revisarlos en Maestro.

1. (Opcional) En el menú desplegable Vista de la página de tipo de registro de objeto de Workfront, elija la vista Cronología para mostrar los objetos vinculados de Workfront en la vista Cronología.












