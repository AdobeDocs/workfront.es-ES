---
title: Conectar registros
description: Después de crear conexiones entre tipos de registros, puede conectar registros individuales entre sí.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 17796cdc-6de8-4209-a5af-b255dc64d70a
source-git-commit: 66e6c96ca51a159f6e9a16178f06dd016217c7d8
workflow-type: tm+mt
source-wordcount: '2396'
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
<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--if you change steps here, also update steps in the "Connect records" article-->

# Conectar registros

{{maestro-important-intro}}

Puede conectar los registros de Adobe Maestro entre sí o con objetos de otras aplicaciones.

Primero debe conectar dos tipos de registro entre sí o un tipo de registro a un tipo de objeto de otra aplicación. Esto crea campos de registro vinculados. A continuación, puede conectar registros entre sí o registros a otros objetos desde otra aplicación mediante los campos de registro vinculados.

Para obtener información sobre cómo conectar tipos de registros entre sí o con tipos de objetos de otras aplicaciones, vea [Conectar tipos de registros](../architecture/connect-record-types.md).

Para ver un ejemplo de tipos de registros de conexión, consulte [Ejemplo de conexión de tipos y registros](../architecture/example-connect-record-types-and-records.md).

Puede conectar lo siguiente:

* Registros operativos de Maestro
* Registros operativos de Maestro con registros de taxonomía
* taxonomías de Maestro
* Registros operativos de Maestro o taxonomías con objetos de otras aplicaciones.

  Puede conectar registros de Maestro a objetos de los tipos que se indican a continuación desde las siguientes aplicaciones:

   * Adobe Workfront

      * Proyectos
      * Portafolios
      * Programas
      * Compañía
      * Grupo

   * Adobe Experience Manager Assets

      * Archivos de imagen
      * Carpetas

  <!--when you add more objects, fix the Access Requirements below which right now refer only to projects-->

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
<td>Product</p> </td>
   <td>
   <p> Adobe Workfront</p> 
   <p>Para conectar registros de Maestro con Experience Manager Assets, debe tener una licencia de Adobe Experience Manager Assets y la instancia de Workfront de su organización debe estar integrada en Adobe Business Platform o en Adobe Admin Console.</p>
   </td>
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
   <td role="rowheader"><p>Configuración del nivel de acceso</p></td>
   <td> <p>No hay controles de nivel de acceso para Maestro</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permisos</p></td>
   <td> <p>Administración de permisos en un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>El administrador de Workfront o de grupo debe agregar el área de Maestro en la plantilla de diseño. Para obtener más información, consulte <a href="../access/access-overview.md">Acceso a información general</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Conectar registros

### Consideraciones sobre la conexión de registros

* Después de conectar los tipos de registro, los tipos de registro conectados se muestran como campos de registro vinculados en la tabla de los tipos de registro desde los que están vinculados y en la página Detalles de los registros desde los que están vinculados.
* Puede examinar y agregar registros y objetos de los tipos de registro y objeto vinculados desde los campos de registro vinculados.
* Puede agregar campos de los tipos de registro vinculados a la tabla del tipo de registro desde el que está vinculando.
* No se pueden actualizar manualmente los valores de los campos vinculados en los registros desde los que se está vinculando.

  Los valores de los campos vinculados de los registros vinculados rellenan el registro de Maestro desde el que está estableciendo el vínculo automáticamente desde el área de trabajo de Maestro que ha configurado o desde la aplicación de terceros.

* Todas las personas que tengan acceso a Maestro y Vista o permisos superiores en el área de trabajo podrán ver las conexiones que se establecen entre los registros de Maestro o entre los registros de Maestro y los objetos de otras aplicaciones. Pueden ver los registros y objetos conectados independientemente de sus permisos en las aplicaciones de terceros a las que se conecte.
* Puede ver y editar las conexiones de todos los demás, si tiene permisos de Administración en el espacio de trabajo donde se encuentran los registros conectados.
* Puede conectar un registro Maestro a uno o varios objetos de otra aplicación.
* Para vincular registros de Maestro con otros registros u objetos, debe tener lo siguiente:

   * Al menos un área de trabajo de Maestro, tipo de registro y registro.

     Para obtener más información, consulte los siguientes artículos:

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
1. (Opcional) Agregue registros al tipo de registro seleccionado agregando una nueva fila a la tabla. Para obtener más información, consulte [Creación de registros](../../maestro/records/create-records.md).
1. Desde un registro enumerado en la vista de tabla, vaya a la columna de registro vinculada, haga clic dentro del campo de registro vinculado y, a continuación, haga clic en **+** icono.

   ![](assets/connected-objects-table-for-records.png)

   >[!TIP]
   >
   >    Puede abrir la página de detalles de un registro, buscar el campo de registro vinculado y hacer clic en **+** en el campo para añadir registros del tipo de objeto o registro conectado.

   El **Conectar objetos** aparece el cuadro.

1. Comience a escribir el nombre de un registro en el cuadro de búsqueda y, a continuación, selecciónelo cuando aparezca en la lista

   O

   Seleccione el nombre de uno o varios registros en el cuadro y haga clic en **Conectar objetos** en la esquina superior derecha del cuadro Conectar objetos.

   Se añaden los elementos siguientes:

   * Los registros vinculados se muestran en el campo de registro vinculado del registro seleccionado en el paso 6. <!--accurate?--> Al actualizar los registros vinculados, se actualizan automáticamente los campos vinculados de los registros que está vinculando. Los campos vinculados no se pueden editar manualmente.

     >[!TIP]
     >
     >* Utilizamos &quot;campos vinculados&quot; y &quot;campos de búsqueda&quot; indistintamente.
     >
     >* Si habilitó la variable **Permitir varios registros** configuración al conectar los tipos de registro, los valores de los campos de varios objetos seleccionados se muestran separados por comas o se agregan según el agregador elegido.

1. (Opcional) Cierre la página de tipo de registro de Maestro y vaya al área de trabajo seleccionada.
1. Haga clic en la tarjeta del tipo de registro al que está vinculado.

   Por ejemplo, si conectó el **Campaign** registro con el Registro de producto, haga clic en el botón **Product** Tarjeta de.

   La tarjeta de tipo de registro se debe abrir en la vista Tabla. Si no es así, seleccione una vista de tabla.

   Observe que la variable **Campaign** El campo de registro vinculado muestra los nombres de las campañas que vinculó a los productos en la página Tipo de registro de producto. Al actualizar la información de Campaign, se actualiza automáticamente el campo de registro vinculado de Campaign para el tipo de registro de producto.

### Conectar registros de Maestro a objetos de Workfront

<!--when we will have more applications to link to from Maestro, change the title to soemthing like: Connect Maestro records to objects from other applications-->

Después de crear una conexión entre un tipo de registro Maestro y un tipo de objeto Workfront, puede conectar registros individuales de Maestro a objetos de Workfront. Los campos de Workfront que ha conectado se rellenan automáticamente en los registros de Maestro desde los que está vinculando los objetos.

>[!NOTE]
>
>No puede conectar objetos de Workfront con registros de Maestro desde Workfront.


{{step1-to-maestro}}

El espacio de trabajo al que se accedió por última vez debe abrirse de forma predeterminada.

1. (Opcional) Expanda la flecha hacia abajo a la derecha del nombre de un área de trabajo existente y seleccione el área de trabajo desde la que desea conectar registros.
1. Haga clic en la tarjeta de un tipo de registro para abrir la página del tipo de registro.
1. Seleccione una **Tabla** vista desde el **Ver** menú desplegable.

1. Agregue registros individuales al tipo de registro seleccionado agregando una nueva fila a la tabla. Para obtener más información, consulte [Creación de registros](../../maestro/records/create-records.md).
1. (Condicional) Si conectó el tipo de registro seleccionado con un objeto Workfront, vaya a la columna de objeto vinculado y pase el ratón sobre la celda correspondiente al registro que desea vincular con objetos de Workfront y, a continuación, haga clic en **+** icono.

   El **Conectar objetos** aparece el cuadro.

   ![](assets/connect-objects-box-to-select-projects.png)

   >[!TIP]
   >
   >    Puede abrir la página de detalles de un registro, buscar el campo de registro vinculado y hacer clic en **+** en el campo para añadir objetos del tipo de objeto conectado.

   Para obtener más información sobre cómo conectar tipos de registros con objetos de una aplicación de terceros, consulte [Conectar tipos de registros](../architecture/connect-record-types.md).

1. Comience a escribir el nombre de un objeto de Workfront en el cuadro de búsqueda y, a continuación, selecciónelo cuando se muestre en la lista

   O

   Seleccione el nombre de uno o varios objetos en el cuadro y haga clic en **Conectar objetos** en la esquina superior derecha del cuadro Conectar objetos.

   >[!IMPORTANT]
   >
   >* Solo puede agregar objetos Workfront para los que tenga acceso de visualización.
   >
   >* Una vez agregados los objetos de Workfront, todas las personas con permisos de Vista o superiores al espacio de trabajo pueden ver los objetos de Workfront y su información de campo, independientemente de sus permisos o acceso en Workfront.

   Se añaden los elementos siguientes:

   * Los objetos Workfront seleccionados se agregan al campo de registro vinculado.
   * Si los agregó al conectar el tipo de registro con Workfront, los campos vinculados (o los campos de búsqueda) de los objetos de Workfront se rellenan automáticamente con información de Workfront.
   * Página de detalles de sólo lectura en Maestro para el objeto de Workfront conectado. Puede tener acceso a esta página haciendo clic en el nombre de un proyecto desde el campo vinculado de un registro de Maestro. Continúe con el paso 8. <!--accurate?-->

     Por ejemplo, al vincularse a proyectos de Workfront se crean las páginas de detalles de esos proyectos en Maestro.

     >[!IMPORTANT]
     >
     > La página Detalles de objetos de Workfront de sólo lectura sólo se crea cuando se agregan proyectos individuales a registros de Maestro. La simple creación de una conexión entre un tipo de registro de Maestro y un tipo de objeto de Workfront no crea el tipo de registro de Workfront en Maestro.

1. (Opcional) Haga clic en el nombre de un objeto de Workfront conectado a un registro Maestro en el campo vinculado de una vista de tabla o desde el **Detalles** página del registro de Maestro.

   Se abrirá el Maestro de sólo lectura **Detalles** para el objeto de Workfront vinculado. Los campos seleccionados como campos de búsqueda al conectar el tipo de registro con el objeto Workfront se muestran en la página Detalles.

   >[!TIP]
   >
   >* Si habilitó la configuración Permitir varios registros, los valores de los objetos múltiples se mostrarán separados por comas o se agregarán según el agregador elegido.
   >
   >* No se crea un campo de registro vinculado para los objetos de Workfront vinculados en Workfront.

1. (Opcional) Para abrir el objeto Workfront vinculado en Workfront, haga clic en **Ir al origen** en la esquina superior derecha de la página Detalles del objeto de Workfront.

   ![](assets/workfront-project-maestro-details-page-with-go-to-source-link.png)

   Esto abre la página de objetos de Workfront si tiene al menos permisos de visualización para ver el objeto. Puede editar información sobre el objeto Workfront si tiene permisos para hacerlo.

1. (Opcional) En la vista de tabla del tipo de registro de Maestro, pase el ratón sobre el encabezado de columna del objeto de Workfront vinculado, haga clic en el menú desplegable y, a continuación, haga clic en **Editar campos de búsqueda**.

1. Agregue campos de objeto de Workfront desde el **Campos no seleccionados** área

   O

   Quite los campos del objeto Workfront de **Campos seleccionados** área.

   Esto agrega o quita campos vinculados de los registros de Maestro. La información asociada con los campos eliminados permanece en Workfront.


### Conectar registros de Maestro a objetos de Adobe Experience Manager

<!--when we will have more applications to link to from Maestro, change the title to soemthing like: Connect Maestro records to objects from other applications-->

>[!IMPORTANT]
>
>Debe tener una licencia de Adobe Experience Manager Assets y la instancia de Workfront de su organización debe estar integrada en Adobe Business Platform o Adobe Admin Console para poder conectar los registros de Maestro a Adobe Experience Manager Assets.
>
>Si tiene alguna pregunta acerca de la incorporación a Adobe Admin Console, consulte la [Preguntas frecuentes sobre Adobe Unified Experience](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

Después de crear una conexión entre un tipo de registro de Maestro y Adobe Experience Manager Assets, puede conectar registros individuales de Maestro a recursos de Experience Manager. Los campos de recurso que conectó desde Experience Manager Assets al crear la conexión se rellenan automáticamente en el tipo de registro de Maestro desde el que vinculó.

{{step1-to-maestro}}

El espacio de trabajo al que se accedió por última vez debe abrirse de forma predeterminada.

1. (Opcional) Expanda la flecha hacia abajo a la derecha del nombre de un área de trabajo existente y seleccione el área de trabajo desde la que desea conectar registros.
1. Haga clic en la tarjeta de un tipo de registro para abrir la página del tipo de registro.
1. Seleccione una **Tabla** vista desde el **Ver** menú desplegable en la esquina superior derecha de la página tipo de registro.

1. (Opcional) Haga clic en **Nuevo registro** para agregar nuevos registros al tipo de registro seleccionado. Para obtener más información, consulte [Creación de registros](../../maestro/records/create-records.md).
1. (Condicional) Si ha conectado el tipo de registro seleccionado con Experience Manager Assets, vaya a la columna de objeto vinculado, pase el ratón sobre la celda correspondiente al registro que desea vincular con otros objetos desde Experience Manager y, a continuación, haga clic en **+** icono.

   >[!TIP]
   >
   >  Puede añadir y hacer clic en **+** en el campo de objeto vinculado de la página Detalles del registro de Maestro para conectar los recursos al registro.

   El **Seleccionar recursos** aparece el cuadro. <!--update screen shot with actual assets-->

   ![](assets/select-assets-box-for-aem-record-connections.png)

   Para obtener más información sobre cómo conectar tipos de registros con tipos de objetos de una aplicación de terceros, consulte [Conectar tipos de registros](../architecture/connect-record-types.md).

1. Haga clic para seleccionar algunos de los siguientes tipos de recursos:

   * Imágenes
   * Carpetas

   Puede seleccionar varios recursos.

   >[!IMPORTANT]
   >
   > Solo puede conectar recursos a los que tenga acceso para verlos en Experience Manager. Una vez conectado, todos los usuarios de Maestro podrán ver los recursos en Maestro, independientemente de su acceso a Experience Manager Assets.

1. Clic **Seleccionar**.

   Se añaden los elementos siguientes:

   * Los recursos del Experience Manager seleccionado se añaden al campo de registro vinculado.
   * Los campos vinculados (o campos de búsqueda) se rellenan con información de los recursos conectados del Experience Manager.
   * Página de detalles de sólo lectura en Maestro para el objeto de Experience Manager Assets conectado. Puede acceder a esta página haciendo clic en el nombre de un recurso en el campo vinculado de un registro de Maestro. Continúe con el paso 8. <!--accurate?-->

     >[!IMPORTANT]
     >
     > La página Detalles de Experience Manager Assets de sólo lectura del tipo de registro vinculado sólo se crea cuando se agregan recursos individuales a los registros de Maestro. La simple creación de una conexión entre un tipo de registro de Maestro y Experience Manager Assets no crea el tipo de registro de Experience Manager Assets.

     Cualquier información existente de los campos de los recursos del Experience Manager se muestra en los campos vinculados o de búsqueda.

     >[!TIP]
     >
     >
     >* Si habilitó la configuración Permitir varios registros, los valores de los objetos múltiples se mostrarán separados por comas.
     >
     >* No se crea un campo de registro vinculado a los registros vinculados de Maestro para los recursos de Experience Manager vinculados en la aplicación de Experience Manager Assets.


1. (Opcional) Vaya al tipo de registro desde el que vinculó a Experience Manager Assets y haga clic en el nombre de un recurso en el campo de registro vinculado. Los detalles del Experience Manager del recurso se muestran en una ventana emergente. <!--update screen shot with hi-rez picture-->

   ![](assets/asset-pop-up-window-with-aem-details-and-thumbnail.png)

   Se muestran los campos siguientes para un archivo de imagen:

   * Una miniatura de la imagen
   * El nombre del archivo de imagen
   * Dimensiones
   * Tamaño
   * Descripción
   * Ruta del archivo en el Experience Manager
   * El tipo de recurso
   * Fecha de creación
   * Fecha de modificación

1. (Opcional) Para abrir la página de detalles del registro de recursos de Experience Manager en Experience Manager, vaya a la página de tipo de registro de Maestro del registro desde el que está vinculando, haga clic en el nombre de un recurso en el campo de registro vinculado para abrir la ventana emergente y, a continuación, haga clic en **Abrir** icono ![](assets/open-asset-icon.png) para abrir el recurso.

   Esto abre el del recurso del Experience Manager **Detalles** página en Maestro.

1. Clic **Ir al origen** en la esquina superior derecha de la pantalla.

   ![](assets/go-to-source-asset-maestro-details-page.png)

   Esto abre el recurso en Adobe Experience Manager Assets si tiene acceso para verlo. Puede actualizar el recurso en esta aplicación si tiene permisos para hacerlo.

1. (Opcional) En la vista de tabla del tipo de registro Maestro, pase el ratón sobre el encabezado de columna del recurso de Experience Manager vinculado, haga clic en el menú desplegable y, a continuación, haga clic en **Editar campos de búsqueda**.

1. Agregue campos de objeto de Experience Manager Assets desde el **Campos no seleccionados** área

   O

   Quite los campos del objeto Workfront de **Campos seleccionados** área.

   Esto agrega o quita campos vinculados de los registros de Maestro. La información asociada con los campos eliminados permanece en Adobe Experience Assets.
