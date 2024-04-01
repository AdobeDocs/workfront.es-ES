---
title: Eliminar tipos de registros
description: Puede eliminar los tipos de registro cuando ya no sean relevantes. Al eliminar los tipos de registro también se elimina toda la información asociada a los tipos de registro, como sus registros, campos y vistas.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: f4fb9d5c22ec6216a05e31cbcf80f1cf9add125f
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav:
---
title: Delete record types
description: You can delete record types when they are no longer relevant. 
author: Alina
feature: Work Management
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->

# Eliminar tipos de registros

{{maestro-important-intro}}

Puede eliminar los tipos de registro cuando ya no sean relevantes.

Sin embargo, al eliminar los tipos de registro también se elimina toda la información asociada a los tipos de registro. Para obtener más información, consulte la [Consideraciones al eliminar tipos de registros](#considerations-when-deleting-record-types) de este artículo.

Para obtener información sobre los tipos de registros, consulte [Resumen de los tipos de registro](../architecture/overview-of-record-types-and-taxonomies.md).

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

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
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>acuerdo con Adobe Workfront</p></td>
   <td>
<p>Su organización debe estar inscrita en el programa beta de Adobe Workfront Planning. Póngase en contacto con el representante de cuentas para obtener más información sobre esta nueva oferta. </p>
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
   <td role="rowheader"><p>Configuraciones de nivel de acceso</p></td>
   <td> <p>No hay controles de nivel de acceso para Adobe Workfront Planning</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Permisos</p></td>
   <td> <p>Administración de permisos en un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>El administrador del grupo o de Workfront debe agregar el área de Planning a la plantilla de diseño. Para obtener más información, consulte <a href="../access/access-overview.md">Acceso a información general</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Consideraciones al eliminar tipos de registros

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* Solo puede eliminar tipos de registro de espacios de trabajo en los que tenga permisos de administración.
* Al eliminar los tipos de registro, se elimina la siguiente información asociada a ellos:

   * Todos los registros de ese tipo.
   * Todos los campos asociados al tipo de registro.
   * Todas las vistas (incluidos filtros, agrupaciones y criterios de ordenación) del tipo de registro.
* El tipo de registro se elimina de todos los usuarios que acceden al espacio de trabajo.
* No se pueden recuperar los tipos de registros eliminados ni su información.
* Se recomienda volver a crear los campos y los registros asociados al tipo de registro que desea eliminar en otro tipo de registro antes de eliminarlos.

## Eliminar tipos de registros

{{step1-to-maestro}}

El espacio de trabajo al que se accedió por última vez debe abrirse de forma predeterminada.

1. (Opcional) Expanda la flecha hacia abajo a la derecha del nombre de un área de trabajo existente y seleccione el área de trabajo para la que desea eliminar los tipos de registros.

   Se abre el espacio de trabajo y se muestran los tipos de registro.
1. Haga clic en la tarjeta del tipo de registro que desee eliminar.

   Se abre la página del tipo de registro.
1. Haga clic en **Más** menú ![](assets/more-menu.png) a la derecha del nombre del tipo de registro y haga clic en **Eliminar**. <!--add screen shot when they finalize the UI-->
1. Tipo **Eliminar** en el cuadro de confirmación, haga clic en **Eliminar permanentemente**.

   El tipo de registro seleccionado, junto con sus campos, registros asociados y vistas, se eliminan.
