---
title: Conectar registros
description: Después de crear conexiones entre tipos de registros, puede conectar registros individuales entre sí.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 17796cdc-6de8-4209-a5af-b255dc64d70a
source-git-commit: a74f9f8940a170d8e1347fd99ff2a6c816b12eca
workflow-type: tm+mt
source-wordcount: '2911'
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
>La información de este artículo hace referencia a Adobe Maestro, que es una nueva oferta de Adobe Workfront.
>
>En la actualidad, Adobe Maestro forma parte de un programa beta abierto a un número limitado de clientes. Debe ser cliente de Workfront para utilizar las funciones de Maestro.
>
>Póngase en contacto con su representante de cuentas para obtener más información acerca de cómo unirse al programa beta de Maestro.
>
>Para obtener más información, consulte [Introducción a Adobe Maestro](../maestro-overview.md).

Puede conectar los registros de Adobe Maestro entre sí o con objetos de otras aplicaciones.

Primero debe conectar dos tipos de registro o un tipo de registro a un tipo de objeto de otra aplicación y, a continuación, puede utilizar la vista Tabla del tipo de registro para conectar registros entre sí o registros a otros objetos.

Para obtener información sobre cómo conectar tipos de registros entre sí o con tipos de objetos de otras aplicaciones, vea [Conectar tipos de registros](../architecture/connect-record-types.md).

Para ver un ejemplo de tipos de registros de conexión, consulte [Ejemplo de conexión de tipos y registros](../architecture/example-connect-record-types-and-records.md).

Puede conectar lo siguiente:

* Registros operativos de Maestro
* Registros operativos de Maestro a registros de taxonomía
* Registros operativos y objetos de otras aplicaciones de Maestro.

  Puede conectar registros de Maestro a objetos de los tipos que se indican a continuación desde las siguientes aplicaciones:

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

<!--
After permssions - replace the table with: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

-->

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
* Para vincular registros de Maestro con objetos de Workfront, debe tener lo siguiente:

   * Objetos Workfront. Por ejemplo, primero debe crear proyectos, portafolios, programas, empresas o grupos en Workfront.
   * Espacios de trabajo de Maestro, tipos de registros y registros. Para obtener más información, consulte los siguientes artículos:

      * [Creación de espacios de trabajo](../architecture/create-workspaces.md)
      * [Creación de tipos de registros](../architecture/create-record-types.md)
      * [Creación de registros](../records/create-records.md)

   * Conexiones entre tipos de registro o entre tipos de registro y objetos de otras aplicaciones. Para obtener más información, consulte [Conectar tipos de registros](../architecture/connect-record-types.md)

### Conectar registros de Maestro

{{step1-to-maestro}}

El espacio de trabajo al que se accedió por última vez debe abrirse de forma predeterminada.

1. (Opcional) Expanda la flecha hacia abajo a la derecha del nombre de un área de trabajo existente y seleccione el área de trabajo desde la que desea conectar registros.
1. Haga clic en la tarjeta de un tipo de registro para abrir la página del tipo de registro.
1. Seleccione una **Tabla** vista desde el **Ver** menú desplegable en la esquina superior derecha de la página tipo de registro.
1. Agregar una conexión a otro tipo de registro u objeto desde el tipo de registro seleccionado. Para obtener más información, consulte [Conectar tipos de registros](../architecture/connect-record-types.md).

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

Después de crear una conexión entre un tipo de registro Maestro y un tipo de objeto Workfront, puede conectar registros individuales de Maestro a objetos de Workfront. Los campos de Workfront que ha conectado se rellenan automáticamente en los registros de Maestro desde los que está vinculando los objetos.

{{step1-to-maestro}}

El espacio de trabajo al que se accedió por última vez debe abrirse de forma predeterminada.

1. (Opcional) Expanda la flecha hacia abajo a la derecha del nombre de un área de trabajo existente y seleccione el área de trabajo desde la que desea conectar registros.
1. Haga clic en la tarjeta de un tipo de registro para abrir la página del tipo de registro.
1. Seleccione una **Tabla** vista desde el **Ver** menú desplegable en la esquina superior derecha de la página tipo de registro.

1. (Opcional) Agregue registros individuales al tipo de registro seleccionado agregando una nueva fila a la tabla. Para obtener más información, consulte [Creación de registros](../../maestro/records/create-records.md).
1. (Condicional) Si conectó el tipo de registro seleccionado con un objeto Workfront, vaya a la columna de objeto vinculado y pase el ratón sobre la celda correspondiente al registro que desea vincular con objetos de Workfront y, a continuación, haga clic en **+** icono.

   El **Conectar objetos** aparece el cuadro.

   ![](assets/connect-objects-box-to-select-projects.png)

   Para obtener más información sobre cómo conectar tipos de registros con objetos de una aplicación de terceros, consulte [Conectar tipos de registros](../architecture/connect-record-types.md).

1. Comience a escribir el nombre de un objeto de Workfront en el cuadro de búsqueda y, a continuación, selecciónelo cuando se muestre en la lista

   O

   Seleccione el nombre de uno o varios objetos en el cuadro y haga clic en **Conectar objetos** en la esquina superior derecha del cuadro Conectar objetos.

   Se añaden los elementos siguientes:

   * Los objetos Workfront seleccionados se agregan al campo de registro vinculado.
   * Se crea un nuevo campo vinculado (o un campo de búsqueda) para cada campo vinculado que seleccionó al agregar los campos al registro vinculado.
   * Se crea un nuevo tipo de registro denominado &quot;&lt; Name of the Workfront object type >&quot; en el mismo espacio de trabajo que el registro de Maestro desde el que está vinculando. El nombre del objeto forma parte del nombre de este tipo de registro. Por ejemplo, al vincular a proyectos de Workfront se crea el **Proyecto** tipo de registro en Maestro.

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
     >* No se crea un campo de registro vinculado a los registros vinculados de Maestro para los objetos de Workfront vinculados en Workfront.


1. (Opcional) Cierre la página de tipo de registro de Maestro y vaya al espacio de trabajo seleccionado.
1. Haga clic en la tarjeta del tipo de registro de objeto de Workfront. Por ejemplo, haga clic en **proyecto de Workfront** , si ha vinculado proyectos de Workfront. La tarjeta de tipo de registro Workfront de solo lectura se debe abrir en la vista Tabla.

   >[!NOTE]
   >
   >    * Los registros enumerados en la página de tipo de registro de Workfront son objetos Workfront de sólo lectura. Los campos vinculados del tipo de registro Workfront también se muestran como columnas de solo lectura y se rellenan automáticamente cuando se rellenan en Workfront.
   >    * Los campos de Workfront no se pueden actualizar manualmente en Maestro. Los campos de objeto de Workfront deben rellenarse en Workfront y los valores de los campos se mostrarán automáticamente en el registro de Workfront en Maestro.
   >

1. (Opcional) Para abrir la página Detalles del registro de objetos de Workfront en Maestro, siga uno de estos procedimientos:

   * Desde el tipo de registro vinculado, vaya al campo de registro Workfront object linked y haga clic en el nombre del objeto Workfront.
   * Desde el **Tabla** Para ver la página de tipo de registro de Workfront, haga clic en el nombre del objeto de Workfront

     O

     Haga clic en **Más** a la derecha del nombre del objeto de Workfront y, a continuación, haga clic en **Ver**.

     ![](assets/workfront-object-more-menu-in-table-with-go-to-source-link.png)

   Se abrirá la página Detalles de Maestro del objeto de Workfront vinculado. Esta es una página de solo lectura.

1. (Opcional) Para abrir el objeto Workfront vinculado en Workfront, realice una de las siguientes acciones:

   * Desde el **Tabla** Para ver la página de tipo de registro de Workfront, haga clic en el nombre del objeto Workfront.

   O

   Haga clic en **Más** a la derecha del nombre del objeto de Workfront y, a continuación, haga clic en **Ir al origen**.

   ![](assets/workfront-project-maestro-details-page-with-go-to-source-link.png)

   Se abrirá la página de objetos de Workfront. Puede editar información sobre el objeto Workfront si tiene permisos para hacerlo.

1. (Opcional) Haga clic en **Añadir campos** icono ![](assets/add-fields-icon.png) en la esquina superior derecha de la vista de tabla de la página tipo de registro de Workfront, para agregar o quitar campos de Workfront del tipo de registro de Workfront.

   >[!NOTE]
   >
   >  Los campos que agregue o quite en la página de tipo de registro de objeto de Workfront no se agregarán ni quitarán del tipo de registro de Maestro que vincula al tipo de objeto de Workfront. Los campos sólo están visibles en la página de sólo lectura de tipo de registro de Workfront, por lo que puede revisarlos en Maestro.

1. (Opcional y condicional) Si ha añadido al menos dos campos de fecha al objeto Workfront, haga clic en **Ver** menú desplegable en la página tipo de registro de objeto de Workfront y seleccione **Cronología** ver o **Crear vista** para crear una vista de cronología.  Para obtener más información, consulte [Administrar la vista de cronología](/help/quicksilver/maestro/views/manage-the-timeline-view.md).

   Los objetos vinculados de Workfront se muestran en la vista de cronología.


### Conectar registros de Maestro a objetos de Adobe Experience Manager

<!--when we will have more applications to link to from Maestro, change the title to soemthing like: Connect Maestro records to objects from other applications-->

Después de crear una conexión entre un tipo de registro de Maestro y Adobe Experience Manager Assets, puede conectar registros individuales de Maestro a recursos de Experience Manager. Los campos de recurso que conectó desde Experience Manager Assets al crear la conexión se rellenan automáticamente en el tipo de registro de Maestro desde el que vinculó.

{{step1-to-maestro}}

El espacio de trabajo al que se accedió por última vez debe abrirse de forma predeterminada.

1. (Opcional) Expanda la flecha hacia abajo a la derecha del nombre de un área de trabajo existente y seleccione el área de trabajo desde la que desea conectar registros.
1. Haga clic en la tarjeta de un tipo de registro para abrir la página del tipo de registro.
1. Seleccione una **Tabla** vista desde el **Ver** menú desplegable en la esquina superior derecha de la página tipo de registro.

1. (Opcional) Agregue registros individuales al tipo de registro seleccionado agregando una nueva fila a la tabla. Para obtener más información, consulte [Creación de registros](../../maestro/records/create-records.md).
1. (Condicional) Si ha conectado el tipo de registro seleccionado con Experience Manager Assets, vaya a la columna de objeto vinculado, pase el ratón sobre la celda correspondiente al registro que desea vincular con otros objetos desde Experience Manager y, a continuación, haga clic en **+** icono.

   El **Seleccionar recursos** aparece el cuadro. <!--update screen shot with actual assets-->

   ![](assets/select-assets-box-for-aem-record-connections.png)

   Para obtener más información sobre cómo conectar tipos de registros con objetos de una aplicación de terceros, consulte [Conectar tipos de registros](../architecture/connect-record-types.md).

1. Haga clic para seleccionar algunos de los siguientes tipos de recursos:

   * Imágenes
   * Colecciones
   * Carpetas

   Puede seleccionar varios recursos.

   >[!IMPORTANT]
   >
   > Solo puede conectar recursos a los que tenga acceso para verlos en Experience Manager.

1. Clic **Seleccionar**.

   Se añaden los elementos siguientes:

   * Los recursos del Experience Manager seleccionado se añaden al campo de registro vinculado.
   * Se crea un nuevo campo vinculado (o un campo de búsqueda) para cada campo vinculado que seleccionó al agregar los campos al registro vinculado.
   * Se crea un nuevo tipo de registro denominado &quot;Experience Manager Assets&quot; en el mismo área de trabajo que el registro de Maestro desde el que está estableciendo el vínculo.

     Es un tipo de registro de sólo lectura y muestra los objetos de Experience Manager seleccionados en el nuevo campo de objeto vinculado creado a partir del registro Maestro. Los campos vinculados del objeto vinculado también se muestran en los registros de Experience Manager vinculados de solo lectura.

     >[!IMPORTANT]
     >
     > El tipo de registro de sólo lectura de Experience Manager Assets se crea sólo cuando se agregan recursos individuales a los registros de Maestro. La simple creación de una conexión entre un tipo de registro de Maestro y Experience Manager Assets no crea el tipo de registro de Experience Manager Assets.

     Cualquier información existente de los campos de los recursos del Experience Manager se muestra en los campos vinculados o de búsqueda.

     >[!TIP]
     >
     >
     >* Si habilitó la configuración Permitir varios registros, los valores de los objetos múltiples se mostrarán separados por comas.
     >
     >* No se crea un campo de registro vinculado a los registros vinculados de Maestro para los recursos de Experience Manager vinculados en la aplicación de Experience Manager Assets.


1. (Opcional) Cierre la página de tipo de registro de Maestro y vaya al espacio de trabajo seleccionado.
1. Haga clic en la tarjeta del tipo de registro Experience Manager Assets. La tarjeta de tipo de registro Experience Manager Assets de solo lectura se debe abrir en la vista Tabla.

   >[!NOTE]
   >
   >    * Los registros enumerados en la página de tipo de registro de Experience Manager Assets son recursos de solo lectura. Los campos vinculados del tipo de registro Experience Manager Assets también se muestran como columnas de solo lectura y se rellenan automáticamente cuando se rellenan en Experience Manager.
   >    * No puede actualizar manualmente los campos de Experience Manager en Maestro. Los campos de recursos del Experience Manager deben rellenarse en Experience Manager y los valores de los campos se mostrarán automáticamente en el registro de Experience Manager Assets en Maestro.
   >

1. (Opcional) Vaya al tipo de registro desde el que vinculó a Experience Manager Assets y haga clic en el nombre de un recurso en el campo de registro vinculado. Los detalles del Experience Manager del recurso se muestran en una ventana emergente. <!--update screen shot with hi-rez picture-->

   ![](assets/asset-pop-up-window-with-aem-details-and-thumbnail.png)

   Se muestran los campos siguientes para un archivo de imagen:

   * Una miniatura de la imagen
   * El nombre del archivo de imagen
   * Dimension
   * Tamaño
   * Descripción
   * Ruta del archivo en el Experience Manager
   * El tipo de recurso
   * Fecha de creación
   * Fecha de modificación

1. (Opcional) Para abrir la página Detalles del registro de Experience Manager Assets en Maestro, haga lo siguiente:

   1. Vaya a la **Experience Manager Assets** Tarjeta de tipo de registro Maestro en el mismo espacio de trabajo que seleccionó originalmente y haga clic para abrir la página de tipo de registro.
La página de tipo de registro de Experience Manager Assets Maestro es de sólo lectura.
   1. En la vista de tabla, haga clic en el nombre de un recurso

      O

      Pase el ratón sobre el nombre de un recurso y haga clic en **Más** menú ![](assets/more-menu.png) a la derecha del nombre del recurso y haga clic en **Ver**.\
      Se abre el Maestro del recurso **Detalles** página. Esta es una página de solo lectura.
1. (Opcional) Para abrir la página Detalles del registro de recursos del Experience Manager en Experience Manager, realice una de las siguientes acciones:

   * Vaya a la página de tipo de registro de Maestro del registro desde el que está vinculando, haga clic en el nombre de un recurso en el campo de registro vinculado para abrir la ventana emergente y, a continuación, haga clic en **Abrir** icono ![](assets/open-asset-icon.png) para abrir el recurso.
   * Vaya a la **Experience Manager Assets** Tarjeta de tipo de registro Maestro en el mismo área de trabajo que seleccionó originalmente y haga clic para abrir la página de tipo de registro, haga clic en el nombre de un recurso para abrir Maestro **Detalles** y haga clic en **Ir al origen** en la esquina superior derecha de la pantalla.

     ![](assets/go-to-source-asset-maestro-details-page.png)
   * Vaya a la **Experience Manager Assets** Tarjeta de tipo de registro Maestro en el mismo espacio de trabajo que seleccionó originalmente y haga clic en la tarjeta para abrir la página de tipo de registro de Experience Manager Assets, pase el ratón sobre el nombre de un recurso y haga clic en **Más** y haga clic en **Ir al origen**.

     ![](assets/go-to-source-option-on-table-view.png)

   El recurso se abre en Experience Manager Assets.

1. (Opcional) Haga clic en **Añadir campos** icono ![](assets/add-fields-icon.png) en la esquina superior derecha de la vista de tabla de la página tipo de registro de Experience Manager Assets, para agregar o quitar campos de Experience Manager.

   >[!NOTE]
   >
   >  Los campos que agregue o quite en la página de tipo de registro de Experience Manager Assets no se agregarán ni quitarán del tipo de registro de Maestro que vincula al recurso de Experience Manager. Los campos sólo están visibles en la página de sólo lectura de tipo de registro de Experience Manager Assets, por lo que puede revisarlos en Maestro.

1. (Opcional y condicional) Si ha añadido al menos dos campos de fecha al recurso vinculado de Experience Manager, haga clic en **Ver** menú desplegable en la página de tipo de registro de Experience Manager Assets y seleccione **Cronología** ver o **Crear vista** para crear una vista de cronología.  Para obtener más información, consulte [Administrar la vista de cronología](/help/quicksilver/maestro/views/manage-the-timeline-view.md).
Los recursos vinculados de Experience Manager Assets se muestran en la vista de cronología.