---
title: Conectar registros
description: Después de crear conexiones entre tipos de registros, puede conectar registros individuales entre sí.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 17796cdc-6de8-4209-a5af-b255dc64d70a
source-git-commit: 5c7b60ac5b78bd065ffc270588ec72ab3eb2f41d
workflow-type: tm+mt
source-wordcount: '2507'
ht-degree: 1%

---

<!--when you make this live, update the metadata above to this: 
---
title: Connect records and objects
description: In addition to connecting records to one another, you can also connect records to objects from other applications.  
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->
<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--if you change steps here, also update steps in the "Connect records" article-->

# Conectar registros

{{planning-important-intro}}

Puede conectar registros de Adobe Workfront Planning entre sí o a objetos de otras aplicaciones.

Primero debe conectar dos tipos de registro entre sí o un tipo de registro a un tipo de objeto de otra aplicación. Esto crea campos de registro vinculados. A continuación, puede conectar registros entre sí o registros a otros objetos de otras aplicaciones mediante los campos de registro vinculados.

Conectar registros es similar a conectar registros a objetos de otra aplicación.

Para obtener información acerca de cómo conectar tipos de registros entre sí o con tipos de objetos de otras aplicaciones, vea [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).

Para ver un ejemplo de tipos de registros de conexión, vea [Ejemplo de tipos de registros de conexión y registros](/help/quicksilver/planning/architecture/example-connect-record-types-and-records.md).

Puede conectar lo siguiente:

* Registros de Adobe Workfront Planning
* Adobe Workfront Planning registra los objetos de otras aplicaciones.

  Puede conectar registros a objetos de los tipos que se indican a continuación desde las aplicaciones siguientes:

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

+++ Amplíe para ver los requisitos de acceso para Workfront Planning.

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
   <p>Para conectar registros de Adobe Workfront Planning con Experience Manager Assets, debe tener una licencia de Adobe Experience Manager Assets y la instancia de Workfront de su organización debe estar integrada en la experiencia unificada de Adobe. Para obtener más información, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiencia unificada de Adobe para Workfront</a>.</p>
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
   <p>Nuevo: estándar</p>
   <p>Actual: plan</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuración del nivel de acceso</p></td>
   <td> <p>No hay controles de nivel de acceso para Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permisos</p></td>
   <td> <p>Administración de permisos en un espacio de trabajo para conectar registros </p>  
   <p>Permite ver o aumentar los permisos de un espacio de trabajo para ver todas las conexiones a objetos y campos desde otras aplicaciones, independientemente del acceso en la otra aplicación. </p>
   <p>Permite ver o permisos superiores a los objetos que desea vincular desde Workfront o Experience Manager Assets. </p>
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon.</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>El administrador del grupo o de Workfront debe agregar el área de Planning a la plantilla de diseño. Para obtener más información, consulte <a href="/help/quicksilver/planning/access/access-overview.md">Resumen de acceso</a>. </p>  
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

## Consideraciones sobre la conexión de registros

* Después de conectar los tipos de registros, los tipos de registros conectados se muestran como campos de registro vinculados en la tabla de los tipos de registros desde los que están vinculados y en las páginas de los registros.
* Puede examinar y agregar registros y objetos de los tipos de registro y objeto vinculados desde los campos de registro vinculados.
* Puede agregar campos (campos de búsqueda) de los tipos de registro vinculados en la tabla del tipo de registro desde el que está vinculando.

  Puede agregar campos (campos de búsqueda) de los tipos de registro desde los que está vinculando en la tabla del tipo de registro al que está vinculando.

  Por ejemplo, si vincula el tipo de registro de Producto desde el tipo de registro de Campaña, puede mostrar campos de Producto para campañas, así como campos de Campaña para productos.
* No puede actualizar manualmente los valores de los campos de búsqueda en los registros desde los que está vinculando.

  Los valores de los campos de búsqueda de los registros vinculados rellenan el registro de Workfront Planning desde el que está vinculando automáticamente desde el registro u objeto original.

* Todas las personas con acceso a Workfront Planning y View o permisos superiores en el espacio de trabajo pueden ver las conexiones que se realizan entre registros o entre registros y objetos de otras aplicaciones. Pueden ver los registros y objetos conectados independientemente de sus permisos en las aplicaciones a las que se conecta.
* Puede ver y editar las conexiones de todos los demás, si tiene permisos de Administración en el espacio de trabajo donde se encuentran los registros conectados.
* Puede conectar un registro a uno o varios objetos desde otra aplicación.

* Puede conectar objetos de Workfront a registros de Workfront Planning en las siguientes áreas:
   * Desde un registro de Planning en Workfront Planning.
   * Desde la sección Planificación de un objeto de Workfront.

* Puede conectar los registros de Workfront Planning a Experience Manager Assets en las siguientes áreas:

   * Desde un registro de Planning en Workfront Planning


## Requisitos previos para vincular registros

Para vincular registros con otros registros u objetos, debe tener lo siguiente:

* Al menos un espacio de trabajo, tipo de registro y registro.

  Para obtener más información, consulte los siguientes artículos:

   * [Creación de espacios de trabajo](/help/quicksilver/planning/architecture/create-workspaces.md)
   * [Creación de tipos de registros](/help/quicksilver/planning/architecture/create-record-types.md)
   * [Creación de registros](/help/quicksilver/planning/records/create-records.md)

* Conexiones entre tipos de registro o entre tipos de registro y objetos de otras aplicaciones. Para obtener más información, vea [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).

## Conectar registros de Workfront Planning

### Conectar registros de Adobe Workfront Planning

{{step1-to-planning}}

1. Haga clic en el área de trabajo cuyos registros desee conectar

   El espacio de trabajo se abre y los tipos de registro se muestran como tarjetas.
1. Haga clic en la tarjeta de un tipo de registro para abrir la página del tipo de registro.
1. Seleccione una vista de **Tabla** del menú desplegable **Vista** en la esquina superior derecha de la página de tipo de registro.
1. (Opcional) Agregue registros al tipo de registro seleccionado agregando una nueva fila a la tabla. Para obtener más información, consulte [Crear registros](/help/quicksilver/planning/records/create-records.md).
1. (Condicional) Después de conectar el tipo de registro seleccionado con otro tipo de registro, vaya a la columna de registro vinculado y haga doble clic en la celda correspondiente al registro que desea vincular con otros registros.

   ![](assets/connect-other-records-smaller-box-in-table-view.png)

1. Realice una de las siguientes acciones:

   * Haga clic en el nombre de un registro conectado de la lista para agregarlo al registro seleccionado. El registro se agrega automáticamente.
   * Empiece a escribir el nombre de un registro y haga clic en él cuando aparezca en la lista. El registro se agrega automáticamente.
   * Haga clic en **Ver todo** para mostrar todos los registros.

1. (Condicional) Si hizo clic en **Seleccionar todo** en el paso anterior, se muestra el cuadro **Conectar objetos**.

   ![](assets/connected-objects-table-for-records.png)

1. Comience a escribir el nombre de un registro en el cuadro de búsqueda y, a continuación, selecciónelo cuando aparezca en la lista

   O

   Seleccione el nombre de uno o varios registros en el cuadro y, a continuación, haga clic en **Conectar objetos** en la esquina superior derecha del cuadro Conectar objetos.

   >[!TIP]
   >
   >    Puede abrir la página de un registro, buscar el campo de registro vinculado y hacer clic en el campo conectado (si ya hay registros conectados), o hacer clic en **Conectar registros** (si el campo está vacío) para agregar registros del tipo de objeto o registro conectado.
   >
   >![](assets/connect-records-from-record-page-field.png)

   Se añaden los elementos siguientes:

   * Los registros vinculados se muestran en el campo de registro vinculado del registro seleccionado en el paso 6. <!--accurate?-->
   * Los campos vinculados se rellenan con la información de los registros vinculados, si agregó campos de búsqueda vinculados al conectar los tipos de registro.

   Al actualizar los registros vinculados, se actualizan automáticamente los campos vinculados de los registros que está vinculando. Los campos vinculados no se pueden editar manualmente.

   >[!TIP]
   >
   >* Utilizamos &quot;campos vinculados&quot; y &quot;campos de búsqueda&quot; indistintamente.
   >
   >* Si habilitó la opción **Permitir varios registros** al conectar los tipos de registros, los valores de los campos de los objetos seleccionados múltiples se mostrarán separados por comas o se agregarán según el agregador elegido.

1. (Opcional) Cierre la página de tipo de registro y vaya al espacio de trabajo seleccionado.
1. Haga clic en la tarjeta del tipo de registro al que está vinculado.

   Por ejemplo, si conectó el registro **Campaign** con el registro Product, haga clic en la tarjeta **Product**.

   La tarjeta de tipo de registro se debe abrir en la vista Tabla. Si no es así, seleccione una vista de tabla.

   Observe que el campo de registro vinculado **Campaign** muestra los nombres de las campañas que vinculó a los productos en la página Tipo de registro de producto. Al actualizar la información de Campaign, se actualiza automáticamente el campo de registro vinculado de Campaign para el tipo de registro de producto.

### Conexión de registros de Adobe Workfront Planning a objetos de Workfront

<!--when we will have more applications to link to from Planning, change the title to something like: Connect Workfront Planning records to objects from other applications-->

Después de crear una conexión entre un tipo de registro y un tipo de objeto de Workfront, puede conectar registros individuales a objetos en Workfront. Los campos de Workfront que ha conectado se rellenan automáticamente en los registros desde los que está vinculando los objetos.

>[!NOTE]
>
>No puede conectar tipos de objetos de Workfront con tipos de registros de Workfront Planning desde Workfront.


{{step1-to-planning}}

1. Haga clic en el área de trabajo cuyos registros desee conectar.

   El espacio de trabajo se abre y los tipos de registro se muestran como tarjetas.
1. Haga clic en la tarjeta de un tipo de registro para abrir la página del tipo de registro.
1. Seleccione una vista de **Tabla** del menú desplegable **Vista**.

1. Haga clic en **Nuevo registro** para agregar registros individuales al tipo de registro que seleccionó. Para obtener más información, consulte [Crear registros](/help/quicksilver/planning/records/create-records.md).
1. (Condicional) Después de conectar el tipo de registro seleccionado con un tipo de objeto de Workfront, vaya a la columna de objeto vinculado y haga doble clic en la celda correspondiente al registro que desea vincular con los objetos de Workfront.

   ![](assets/connect-projects-smaller-box-in-table-view.png)

1. Realice una de las siguientes acciones:

   * Haga clic en un objeto de la lista para agregarlo al registro seleccionado. Los objetos se muestran alfabéticamente. El objeto se agrega automáticamente.
   * Empiece a escribir el nombre de un objeto y haga clic en él cuando se muestre en la lista. El objeto se agrega automáticamente.
   * Haga clic en **Ver todo** para mostrar todos los objetos para los que tiene al menos permisos de visualización.

1. (Condicional) Si hizo clic en **Ver todo** en el paso anterior, se muestra el cuadro **Conectar objetos**.

   ![](assets/connect-objects-box-to-select-projects.png)

1. Comience a escribir el nombre de un objeto de Workfront en el cuadro de búsqueda y, a continuación, selecciónelo cuando se muestre en la lista

   O

   Seleccione el nombre de uno o varios objetos en el cuadro y, a continuación, haga clic en **Conectar objetos** en la esquina superior derecha del cuadro Conectar objetos.

   >[!IMPORTANT]
   >
   >* Solo puede agregar objetos Workfront para los que tenga acceso de visualización.
   >
   >* Una vez agregados los objetos de Workfront, todas las personas con permisos de Vista o superiores al espacio de trabajo pueden ver los objetos de Workfront y su información de campo, independientemente de sus permisos o acceso en Workfront.

   Se añaden los elementos siguientes:

   * Los objetos Workfront seleccionados se agregan al campo de registro vinculado.
   * Si los agregó al conectar el tipo de registro con Workfront, los campos vinculados (o los campos de búsqueda) de los objetos de Workfront se rellenan automáticamente con información de Workfront.

   >[!TIP]
   >
   >Puede abrir la página de un registro, buscar el campo de registro vinculado y hacer clic en el icono **+** del campo para agregar objetos del tipo de objeto conectado.

   Para obtener más información sobre cómo conectar tipos de registros con objetos de otra aplicación, vea [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).

1. (Opcional) Haga clic en el nombre de un objeto de Workfront conectado a un registro de Workfront Planning, ya sea en el campo vinculado de una vista de tabla o desde el campo vinculado de la página de registro.

   Se abrirá el objeto Workfront en Workfront si tiene al menos permisos de visualización sobre el objeto.

   >[!TIP]
   >
   >* Al habilitar la configuración Permitir varios registros, los valores de los campos de búsqueda se muestran separados por comas o se agregan según el agregador elegido.
   >
   >* No se crea un campo de registro vinculado para los objetos de Workfront vinculados en Workfront.

1. (Opcional) En la vista de tabla del tipo de registro, pase el ratón sobre el encabezado de columna del objeto de Workfront vinculado, haga clic en el menú desplegable y, a continuación, haga clic en **Editar campos de búsqueda**.

1. Agregar campos de objeto de Workfront desde el área **Campos no seleccionados**

   O

   Quitar campos del objeto Workfront del área **Campos seleccionados**.

   Esto agrega o quita campos vinculados de los registros de Workfront Planning. La información asociada con los campos eliminados permanece en Workfront.


### Conexión de registros de Workfront Planning a objetos de Adobe Experience Manager

<!--when we will have more applications to link to from Planning, change the title to something like: Connect Workfront Planning records to objects from other applications-->

>[!IMPORTANT]
>
>Debe tener una licencia de Adobe Experience Manager Assets y la instancia de Workfront de su organización debe estar integrada en Adobe Business Platform o Adobe Admin Console para poder conectar los registros de Workfront Planning a Adobe Experience Manager Assets.
>
>Si tiene preguntas acerca de la incorporación a Adobe Admin Console, consulte las [Preguntas frecuentes sobre la experiencia unificada de Adobe](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

Después de crear una conexión entre un tipo de registro y Adobe Experience Manager Assets, puede conectar registros individuales a recursos de Experience Manager. Los campos de recurso que conectó desde Experience Manager Assets al crear la conexión se rellenan automáticamente en el tipo de registro vinculado desde.

>[!NOTE]
>
>Se puede acceder a los registros de Planning y a sus campos desde Experience Manager Assets cuando el administrador de Workfront configura la asignación de metadatos mediante la integración entre Workfront y Adobe Experience Manager Assets. Para obtener más información, consulte [Configuración de la asignación de metadatos de recursos entre Adobe Workfront y Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).


{{step1-to-planning}}

1. Haga clic en el área de trabajo cuyos registros desee conectar.

   Se abre el espacio de trabajo y se muestran los tipos de registro.
1. Haga clic en la tarjeta de un tipo de registro para abrir la página del tipo de registro.
1. Seleccione una vista de **Tabla** del menú desplegable **Vista** en la esquina superior derecha de la página de tipo de registro.

1. (Opcional) Haga clic en **Nuevo registro** para agregar nuevos registros al tipo de registro que seleccionó. Para obtener más información, consulte [Crear registros](/help/quicksilver/planning/records/create-records.md).
1. (Condicional) Después de conectar el tipo de registro seleccionado con Experience Manager Assets, vaya a la columna de objeto vinculado, pase el ratón sobre la celda correspondiente al registro que desea vincular con otros objetos del Experience Manager y, a continuación, haga clic en el icono **+**.

   >[!TIP]
   >
   >  Puede agregar hacer clic en el icono **+** en el campo de objeto vinculado en la página de registro para conectar recursos al registro.

   Se muestra el cuadro **Seleccionar Assets**. <!--we might change this to Connect assets-->

   ![](assets/select-assets-box-for-aem-record-connections.png)

1. Haga clic para seleccionar algunos de los siguientes tipos de recursos:

   * Imágenes
   * Carpetas

   Puede seleccionar varios recursos.

   >[!IMPORTANT]
   >
   > Solo puede conectar recursos a los que tenga acceso para verlos en Experience Manager. Una vez conectado, todos los usuarios de Workfront Planning pueden ver los recursos en Workfront Planning, independientemente de su acceso en Experience Manager Assets.

1. Haga clic en **Seleccionar**. <!-- we might change this to Connect-->

   Se añaden los elementos siguientes:

   * Los recursos del Experience Manager seleccionado se añaden al campo de registro vinculado.
   * Los campos vinculados (o campos de búsqueda) se rellenan con información de los recursos conectados del Experience Manager.

     Cualquier información existente de los campos de los recursos del Experience Manager se muestra automáticamente en los campos vinculados o de búsqueda.

     >[!TIP]
     >
     >* Si habilitó la configuración Permitir varios registros, los valores de los objetos múltiples se mostrarán separados por comas o agregados según el agregador elegido.
     >
     >* No se crea un campo de registro vinculado a los registros vinculados de Workfront Planning para los recursos de Experience Manager vinculados en la aplicación de Experience Manager Assets.

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

1. (Opcional) Para abrir la página de registro de recursos del Experience Manager en Experience Manager AEM, vaya a la página de tipo de registro del registro desde el que está vinculando, haga clic en el nombre de un recurso en el campo de registro vinculado para abrir la ventana emergente y, a continuación, haga clic en el icono **Abrir en** ![](assets/open-asset-icon.png) para abrir el recurso.

   Se abrirá el recurso del Experience Manager en Adobe Experience Manager Assets.

1. (Opcional) En la vista de tabla del tipo de registro, pase el ratón sobre el encabezado de columna del recurso de Experience Manager vinculado, haga clic en el menú desplegable y, a continuación, haga clic en **Editar campos de búsqueda**.

1. Agregar campos de objeto de Experience Manager Assets desde el área **Campos no seleccionados**

   O

   Quitar campos del objeto Workfront del área **Campos seleccionados**.

   Esto agrega o quita campos vinculados de los registros. La información asociada con los campos eliminados permanece en Adobe Experience Assets.

## Conexión de registros de objetos de Workfront

Debe tener lo siguiente para conectar registros de Workfront Planning desde objetos de Workfront:

* Conexiones entre tipos de registros y tipos de objetos de Workfront.
* Al menos una conexión entre un registro y un objeto de Workfront.
* El administrador de Workfront o de grupo debe agregar la sección de Planning a los tipos de objeto de Workfront que pueden conectarse a los tipos de registro de Planning.

Para obtener más información, consulte [Administrar registros en la sección Planificación de objetos de Adobe Workfront](/help/quicksilver/planning/records/manage-records-in-planning-section.md).
