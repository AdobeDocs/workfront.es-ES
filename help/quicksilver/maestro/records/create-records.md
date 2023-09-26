---
title: Creación de registros
description: En Adobe Maestro, un registro es una instancia de un tipo de registro. Debe crear tipos de registros para poder crear registros individuales.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 28602d66b43ec4c30a9f13cff43157b978439d99
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 0%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Creación de registros

>[!IMPORTANT]
>
>En la actualidad, Adobe Maestro forma parte de un programa beta abierto a un número limitado de clientes.
>
>Póngase en contacto con su representante de cuentas para obtener más información acerca de cómo unirse al programa beta de Maestro.
>
>Para obtener más información, consulte [Introducción a Adobe Maestro](../maestro-overview.md).

En Adobe Maestro, un registro es una instancia de un tipo de registro.

Puede tener los siguientes tipos de registros:

* **Registros operativos**: representan objetos relacionados con el trabajo. Por ejemplo, para un registro operativo llamado &quot;Campaña&quot;, puede tener registros con nombre como &quot;Boletín mensual&quot; o &quot;Venta de verano&quot;.
* **Registros de taxonomía**: representan atributos que pueden asociarse con registros operativos. Por ejemplo, para un tipo de registro de taxonomía llamado &quot;Canal&quot;, puede tener taxonomías con nombres como &quot;Correo electrónico&quot;, &quot;Medios sociales&quot; o &quot;Publicidad&quot;.

La creación de registros operativos es idéntica a la creación de registros de taxonomía o taxonomías.

Para crear registros en Maestro, siga uno de estos procedimientos:

* Crearlos manualmente para los tipos de registros de Maestro
* Conéctelos a los registros de Maestro desde aplicaciones de terceros.

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

## Crear registros agregándolos manualmente a un tipo de registro <!--in a record type table (I don't think you can create them elsewhere right now)-->

Puede crear registros en la vista de tabla de una página de tipo de registro.

1. Haga clic en **Menú principal** icono ![](assets/main-menu-workfront.png) en la esquina superior derecha <!--or the **Main Menu** icon ![](assets/main-menu-shell.png) in the upper-left corner, if available-->, luego haga clic en **Maestro** ![](assets/maestro-icon.png).
El espacio de trabajo al que se accedió por última vez se abre de forma predeterminada. Para obtener información sobre la creación de espacios de trabajo, consulte [Creación de espacios de trabajo](../architecture-and-fields/create-workspaces.md).
1. Haga clic en una tarjeta de tipo de registro. Para obtener información sobre cómo crear un tipo de registro, consulte [Creación de tipos de registros](../architecture-and-fields/create-record-types.md).

   La página de tipo de registro se abre en la vista a la que se accedió por última vez. De forma predeterminada, se abre una página de tipo de registro en la vista de tabla.
Todos los registros del tipo seleccionado se muestran en la vista de tabla.

1. (Condicional) Si la página de tipo de registro no se abre en la vista de tabla, haga clic en **Ver** y seleccione una de las opciones existentes. **Vista de tabla** ![](assets/table-view-icon.png) o haga clic en **Crear vista > Tabla** para crear una vista de tabla.

1. Clic **Nuevo &lt; Nombre del tipo de registro >** en la última fila de la tabla para agregar una nueva fila a la tabla.

   ![](assets/adding-a-new-campaign-in-table-row.png)

1. Empiece a escribir información en la nueva fila sobre el nuevo registro.

   >[!NOTE]
   >
   >  * El campo Nombre no es un campo obligatorio. Sin embargo, se recomienda agregar un nombre para el registro, ya que es útil identificar registros al vincularlos entre sí.
   >
   >  * Los campos que hacen referencia a otros tipos de registro o campos calculados son campos de sólo lectura.

1. Siga agregando información en cada fila y haga clic en **Entrar** en el teclado para guardar los cambios.

## Crear registros conectándolos desde otra aplicación

Puede importar registros de otras aplicaciones vinculándolos a registros vinculados de Maestro.

1. Cree un tipo de registro Maestro, tal como se describe en la sección [Creación de tipos de registros](../architecture-and-fields/create-record-types.md).

1. Cree registros Maestro para el tipo de registro que creó en el paso anterior. Para obtener más información, consulte la sección [Crear registros agregándolos manualmente a un tipo de registro](#create-records-by-manually-adding-them-to-a-record-type) en este artículo.

1. Cree una conexión a un tipo de objeto desde una aplicación de terceros para el tipo de registro de Maestro que ha creado. Para obtener más información, consulte [Conectar tipos de registros](../architecture-and-fields/connect-record-types.md).

1. Agregue registros de la aplicación de terceros a los registros de Maestro creados anteriormente mediante el campo de registro vinculado creado en el paso anterior. Para obtener más información, consulte [Conectar registros](../records/connect-records.md).

   Los siguientes elementos se crean en Maestro:

   * Tipo de registro de Maestro de sólo lectura que hace referencia al tipo de registro de terceros al que se vinculó en el campo de registro conectado.

     Por ejemplo, si conecta un tipo de registro Maestro a proyectos de Workfront, se crea un tipo de registro de sólo lectura denominado &quot;proyectos de Workfront&quot; en el mismo área de trabajo.
   * Registros de solo lectura en la página de tipo de registro de terceros. Los registros importados de la aplicación de terceros siguen siendo de solo lectura y solo se pueden actualizar en su aplicación original.


## Crear registros copiando y pegando información de una lista externa

1. En Maestro, comience a crear registros en la vista Tabla, tal como se describe en la sección [Crear registros agregándolos manualmente a un tipo de registro](#create-records-by-manually-adding-them-to-a-record-type) en este artículo.

   Asegúrese de que la vista de tabla de Maestro tiene las columnas (o los campos) que desea rellenar con la información del nuevo registro.

1. Clic **Nuevo &lt; Nombre del tipo de registro >** en la última fila de la tabla para agregar a la tabla tantas filas nuevas como desee que estén los registros nuevos.

   Por ejemplo, agregue 10 filas a la vista de tabla si desea pegar la información de 10 registros nuevos de otra aplicación.

1. En otra aplicación, cree una lista de registros que desee importar en Maestro.

   Por ejemplo, puede utilizar una hoja de cálculo de Excel para crear la lista.

   La lista debe contener información en formato tabular.

   >[!TIP]
   >
   > Las columnas de la lista deben contener información sobre los campos existentes de Maestro.
   >
   > Asegúrese de que ya ha creado los campos deseados en Maestro y de que la información de la hoja se muestra en el formato correcto que coincida con el de cada campo de Maestro.

1. En la aplicación de terceros, seleccione varias filas y columnas y, a continuación, pegue la información en la vista de tabla de tipo de registro, empezando por el primer registro nuevo.

   La siguiente información se importa en Maestro:

   * Las filas contienen los registros nuevos
   * Las columnas rellenan la información de los campos de los registros.

