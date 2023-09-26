---
title: Edición de registros
description: Puede editar la información de los registros en Adobe Maestro. Debe crear tipos de registros antes de empezar a crear y editar registros.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 28602d66b43ec4c30a9f13cff43157b978439d99
workflow-type: tm+mt
source-wordcount: '567'
ht-degree: 1%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Edición de registros

>[!IMPORTANT]
>
>En la actualidad, Adobe Maestro forma parte de un programa beta abierto a un número limitado de clientes.
>
>Póngase en contacto con su representante de cuentas para obtener más información acerca de cómo unirse al programa beta de Maestro.
>
>Para obtener más información, consulte [Introducción a Adobe Maestro](../maestro-overview.md).

Puede editar la información de los registros en Adobe Maestro. Debe crear tipos de registros antes de empezar a crear y editar registros.
Para obtener más información, consulte [Creación de tipos de registros](../architecture-and-fields/create-record-types.md).

&lt;!— mencione aquí que los campos de la vista Detalles son los mismos que los de la vista de tabla — este artículo está vinculado desde Administrar vistas de registros a hacer referencia a esta información—>

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

## Consideraciones acerca de la edición de registros

* Puede editar los registros que usted u otro usuario hayan creado. <!--will change with access levels-->
* Si los registros editados están vinculados a otros registros, la nueva información de los registros que está editando se reflejará en los registros vinculados.
* No puede editar registros de forma masiva. <!--this will probably change-->


## Edición de registros

Puede editar un registro desde las siguientes áreas:

* [Desde la página Detalles de un registro](#edit-a-record-from-the-records-details-page)
* [Desde la vista de tabla de un tipo de registro](#edit-a-record-from-the-record-type-table-view)

### Editar un registro desde la página de detalles del registro

1. Haga clic en **Menú principal** ![](assets/main-menu-workfront.png) en la esquina superior derecha, o la **Menú principal** ![](assets/main-menu-shell.png) en la esquina superior izquierda, si está disponible, haga clic en Maestro.

   El espacio de trabajo al que se accede por última vez se abre.
1. Realice una de las siguientes acciones:

   * En la vista Tabla, haga clic en el nombre de un registro.
   * En la vista Tabla, pase el ratón sobre el nombre de un registro y haga clic en **Más** menú ![](assets/more-menu.png), luego haga clic en **Ver**

     ![](assets/contextual-menu-for-record-row.png)
   * En una vista Línea de tiempo, haga clic en una barra de registros.

   El registro **Detalles** se abre la página.

1. Haga clic en **Más** menú ![](assets/more-menu.png) a la derecha del nombre del registro y haga clic en **Editar**

   O

   Haga clic dentro de cualquier campo editable de la página Detalles para editar la información.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->

   >[!NOTE]
   >
   >    Los campos vinculados o los campos que contienen cálculos o que genera el sistema no se pueden editar.


1. Clic **Guardar cambios**. <!--logged a bug for this - this needs to be "Save"-->

### Editar un registro desde la vista de tabla de tipo de registro

1. Haga clic en **Menú principal** ![](assets/main-menu-workfront.png) en la esquina superior derecha, <!--or the **Main Menu** ![](assets/main-menu-shell.png) in the upper-left corner, if it is available,--> luego haga clic en **Maestro** ![](assets/maestro-icon.png).

   Se abre el espacio de trabajo al que accedió por última vez.
1. Haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.
1. (Condicional) Desde el **Ver** menú desplegable en la esquina superior derecha de la tabla, seleccione una Vista de tabla. Esta debe ser la vista predeterminada, a menos que haya visto el tipo de registro en la vista de escala de tiempo cuando accedió por última vez.

   Los registros asociados al tipo de registro seleccionado se muestran en la vista de tabla.
1. Haga clic dentro de la fila de un registro para comenzar a editar la información sobre el registro en línea y, a continuación, presione **Entrar** en el teclado para guardar los cambios. Los cambios se guardan automáticamente.

   >[!TIP]
   >
   >* Los campos vinculados no se pueden editar. La información de estos campos se rellena automáticamente a partir de los registros vinculados. Para obtener más información, consulte [Conectar tipos de registros](../architecture-and-fields/connect-record-types.md).
   >
   >* Las direcciones URL se reconocen como vínculos en tipos de campo de texto de una sola línea solo cuando comienzan con lo siguiente: http://, https://, ftp:// o www. .



