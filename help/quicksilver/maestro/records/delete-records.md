---
title: Eliminación de registros
description: Puede eliminar los registros que usted u otro usuario hayan creado. No se pueden recuperar los registros eliminados.
hidefromtoc: true
hide: true
source-git-commit: 14b456f32dd2c8735e0a5252387f25305efc7610
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 1%

---


<!--udpate the metadata with real information when making this available in TOC and in the left nav-->

# Eliminación de registros

>[!IMPORTANT]
>
>En la actualidad, Adobe Maestro forma parte de un programa beta cerrado que está abierto a un número limitado de clientes.
>
>Póngase en contacto con su representante de cuentas para obtener más información acerca de cómo unirse al programa beta de Maestro.
>
>Para obtener más información, consulte [Introducción a Adobe Maestro](../maestro-overview.md).

Puede eliminar registros que ya no sean relevantes en Adobe Maestro.

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

## Consideraciones acerca de la eliminación de registros

* Puede eliminar los registros que usted u otro usuario hayan creado.
* No se pueden recuperar los registros eliminados. <!--the above statements (and in the metadata description) will change with access levels and recycle bin??-->
* Si los registros eliminados están vinculados a otros registros, los registros vinculados no se eliminan, pero también se elimina la información del registro eliminado.
* No puede eliminar registros de forma masiva. <!--this will probably change-->
* No se pueden eliminar registros de la vista de escala de tiempo.

## Eliminación de registros

Puede eliminar un registro de las siguientes áreas:

* [Desde la página Detalles de un registro](#delete-a-record-from-the-records-details-page)
* [Desde la vista de tabla de un tipo de registro](#delete-a-record-from-the-record-type-table-view)

### Eliminar un registro de la página Detalles del registro

1. Haga clic en **Menú principal** ![](assets/main-menu-workfront.png) en la esquina superior derecha, o la **Menú principal** ![](assets/main-menu-shell.png) en la esquina superior izquierda, si está disponible, haga clic en Maestro.

   El espacio de trabajo al que se accede por última vez se abre.
1. Haga clic en un tipo de registro.

   Se abre la página de tipo de registro.
1. Realice una de las siguientes acciones:

   * En la vista Tabla, haga clic en el nombre de un registro.
   * En la vista Tabla, pase el ratón sobre el nombre de un registro y haga clic en **Más** menú ![](assets/more-menu.png), luego haga clic en **Ver**

     ![](assets/contextual-menu-for-record-row.png)
   * En una vista Línea de tiempo, haga clic en una barra de registros.

   El registro **Detalles** se abre la página.

1. Haga clic en **Más** menú ![](assets/more-menu.png) a la derecha del nombre del registro y haga clic en **Eliminar**, entonces **Eliminar** de nuevo para confirmar.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
El registro se elimina y no se puede recuperar.

### Eliminar un registro de la vista de tabla de tipo de registro

1. Haga clic en **Menú principal** ![](assets/main-menu-workfront.png) en la esquina superior derecha, o la **Menú principal** ![](assets/main-menu-shell.png) en la esquina superior izquierda, si está disponible, haga clic en **Maestro**.

   Se abre el espacio de trabajo al que accedió por última vez.
1. Haga clic en un tipo de registro.

   Se abre la página de tipo de registro.
1. (Condicional) Desde el **Ver** menú desplegable en la esquina superior derecha de la tabla, seleccione una Vista de tabla. Esta debe ser la vista predeterminada, a menos que haya visto el tipo de registro en la vista de escala de tiempo cuando accedió por última vez.

   Los registros asociados al tipo de registro seleccionado se muestran en la vista de tabla.
1. Haga clic con el botón secundario en una fila de registro y luego haga clic en **Eliminar**.

   ![](assets/contextual-menu-for-record-row.png)

   El registro se elimina y no se puede recuperar.
