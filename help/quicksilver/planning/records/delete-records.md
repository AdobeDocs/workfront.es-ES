---
title: Eliminación de registros
description: Puede eliminar los registros que usted u otro usuario hayan creado. No se pueden recuperar los registros eliminados.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
source-git-commit: 5c7b60ac5b78bd065ffc270588ec72ab3eb2f41d
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 2%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Eliminación de registros

{{planning-important-intro}}

Puede eliminar los registros que ya no sean relevantes en Adobe Workfront Planning.

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
   <td role="rowheader"><p>Licencia de Adobe Workfront*</p>
   </td>
   <td>
   <p>Nuevo: estándar</p>
   <p>Actual: plan</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuraciones de nivel de acceso</p></td>
   <td> <p>No hay controles de nivel de acceso para Adobe Workfront Planning </p>  
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

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++
<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Consideraciones acerca de la eliminación de registros

* Puede eliminar los registros que usted u otro usuario hayan creado.
* No se pueden recuperar los registros eliminados. <!--the above statements (and in the metadata description) will change with access levels and recycle bin??-->
* Si los registros eliminados están vinculados a otros registros, los registros vinculados no se eliminan, pero también se elimina la información del registro eliminado.
* No puede eliminar registros de forma masiva. <!--this will probably change-->
* No se pueden eliminar registros de la vista de escala de tiempo.

## Eliminación de registros

Puede eliminar un registro de las siguientes áreas:

* [Desde la página del registro](#delete-a-record-from-the-records-page)
* [Desde la vista de tabla de un tipo de registro](#delete-a-record-from-the-record-type-table-view)

### Eliminar un registro de la página del registro

{{step1-to-planning}}

1. Haga clic en el área de trabajo cuyos registros desee eliminar.

   El espacio de trabajo se abre y los tipos de registro se muestran como tarjetas.

1. Haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.
1. Realice una de las siguientes acciones:

   * En la vista Tabla, haga clic en el nombre de un registro.
   * En la vista Tabla, pase el ratón sobre el nombre de un registro, haga clic en el menú **Más** ![](assets/more-menu.png) y, a continuación, haga clic en **Ver**

     ![](assets/contextual-menu-for-record-row.png)
   * En una vista Línea de tiempo, haga clic en una barra de registros.

   Se abre la página de registro.

1. Haga clic en el menú **Más** ![](assets/more-menu.png) que se encuentra a la derecha del nombre del registro, luego haga clic en **Eliminar** y después en **Eliminar** de nuevo para confirmar.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
El registro se elimina y no se puede recuperar.

### Eliminar un registro de la vista de tabla de tipo de registro

{{step1-to-planning}}

1. Haga clic en el área de trabajo cuyos registros desee eliminar.

   El espacio de trabajo se abre y los tipos de registro se muestran como tarjetas.

1. Haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.
1. (Condicional) En el menú desplegable **Vista** de la esquina superior izquierda de la tabla, seleccione una Vista de tabla. Esta debe ser la vista predeterminada, a menos que haya visto el tipo de registro en la vista de escala de tiempo cuando accedió por última vez.

   Los registros asociados al tipo de registro seleccionado se muestran en la vista de tabla.
1. Realice una de las siguientes acciones:

   * Haga clic con el botón secundario en una fila de registro y luego haga clic en **Eliminar**.
   * Haga clic en el menú **Más** ![](assets/more-menu.png) a la derecha del nombre del registro y, a continuación, haga clic en **Eliminar**

     ![](assets/contextual-menu-for-record-row.png)

   * Haga clic en el icono **Abrir detalles** ![](assets/open-details-icon-in-table-name-field.png) para abrir el cuadro con la información detallada del registro, y haga clic en **Más** ![](assets/more-menu.png) a la derecha del nombre del registro y, a continuación, en **Eliminar**.

   El registro se elimina y no se puede recuperar.

1. (Opcional) Utilice los siguientes métodos abreviados del teclado para deshacer o rehacer la eliminación de un registro:

   * CTRL + Z (⌘ + Z para Mac) para deshacer un cambio
   * CTRL + Mayús + Z (⌘ + Mayús + Z para Mac) para rehacer un cambio
