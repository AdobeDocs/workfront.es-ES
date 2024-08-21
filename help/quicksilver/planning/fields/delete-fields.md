---
title: Eliminar campos
description: En Adobe Workfront Planning, puede eliminar campos personalizados que ya no sean relevantes.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: 1ad86cd55459d92650ac7a24c41765e579f8bb94
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!---
title: Delete fields
description: In Adobe Planning, you can delete custom fields that are no longer relevant.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

# Eliminar campos

{{planning-important-intro}}

En Adobe Workfront Planning, puede crear campos personalizados para almacenar información sobre registros.

Para obtener información acerca de cómo crear campos personalizados en Workfront Planning, vea [Crear campos](/help/quicksilver/planning/fields/create-fields.md).

Puede eliminar los campos de Workfront Planning que ya no sean relevantes.

## Consideraciones sobre la eliminación de campos de Workfront Planning:

* Sólo puede eliminar un campo en la vista de tabla de tipo de registro.
* No se puede eliminar el campo principal de un registro.
* La información almacenada en el campo se elimina y no se puede recuperar.
* Al eliminar un campo de registro conectado, todos los campos de búsqueda conectados también se eliminan del tipo de registro desde el que se conecta. Los campos de registro conectados de los tipos de registro a los que se conecta también se eliminan del registro al que se conecta.

  Por ejemplo, cuando conecta campañas a otro tipo de registro llamado producto y elimina el campo Producto conectado y el campo de búsqueda Estado del producto de la campaña, se eliminan los siguientes elementos:

   * El campo Product connected de la campaña
   * El campo de búsqueda Estado del producto de la campaña
   * El campo conectado a Campaign desde el producto.

  Para obtener más información, vea [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).

<!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

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
   <td role="rowheader"><p>Licencia de Adobe Workfront*</p></td>
   <td>
   <p>Nuevo: estándar</p>
   <p>Actual: plan</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuraciones de nivel de acceso</p></td>
   <td> <p>No hay controles de nivel de acceso para Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>El administrador del grupo o de Workfront debe agregar el área de Planning a la plantilla de diseño. Para obtener más información, consulte <a href="/help/quicksilver/planning/access/access-overview.md">Resumen de acceso</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permisos</p></td>
   <td> <p>Administrar permisos en un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>
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

## Eliminar campos

<!--When they release the sharing of fields between other records, revise this section.  -->

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo cuyos campos de registro desee eliminar.

   Se abre el espacio de trabajo y se muestran los tipos de registro.

1. Haga clic en la tarjeta de un tipo de registro.

1. (Condicional) Si aún no está seleccionado, haga clic en la ficha de una **vista de tabla** en la página de tipo de registro.

   Todos los registros existentes asociados al tipo de registro se muestran en las filas de la vista de tabla.

1. Busque el campo que desea eliminar en los encabezados de columna, pase el ratón sobre el encabezado de columna y, a continuación, haga clic en la flecha hacia abajo situada después del nombre del campo.

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Haga clic en **Eliminar**. <!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. Haga clic en **Eliminar** para confirmar.

   El campo se elimina, no se puede recuperar y ya no se puede asociar a ningún registro.
