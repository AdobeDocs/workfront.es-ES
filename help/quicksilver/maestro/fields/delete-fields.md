---
title: Eliminar campos
description: En la planificación de Adobe Workfront, puede eliminar los campos personalizados que ya no sean relevantes.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: a0f12a016ae8ac73136f05bf3255f9882e2ce6d4
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!---
title: Delete fields
description: In Adobe Maestro, you can delete custom fields that are no longer relevant.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

# Eliminar campos

{{maestro-important-intro}}

En Adobe Workfront Planning, puede crear campos personalizados para almacenar información sobre registros.

Para obtener información sobre la creación de campos personalizados en la planificación de Workfront, consulte [Creación de campos](../fields/create-fields.md).

Puede eliminar los campos de planificación de Workfront que ya no sean relevantes.

## Consideraciones sobre la eliminación de campos de planificación de Workfront:

* Sólo puede eliminar un campo en la vista de tabla de tipo de registro.
* No se puede eliminar el campo principal de un registro.
* La información almacenada en el campo se elimina y no se puede recuperar.
* Cuando se elimina un campo de registro vinculado, todos los campos de búsqueda vinculados también se eliminan del tipo de registro desde el que se establece el vínculo. Los campos de registro vinculados de los tipos de registro a los que está vinculado no se eliminan.

  Para obtener más información, consulte [Conectar tipos de registros](../architecture/connect-record-types.md).

<!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

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
<p>Su organización debe estar inscrita en el programa beta de planificación de Adobe Workfront. Póngase en contacto con el representante de cuentas para obtener más información sobre esta nueva oferta. </p>
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
   <td> <p>No hay controles de nivel de acceso para la planificación de Workfront</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>El administrador del grupo o de Workfront debe agregar el área de Planning a la plantilla de diseño. Para obtener más información, consulte <a href="../access/access-overview.md">Acceso a información general</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permisos</p></td>
   <td> <p>Administración de permisos en un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>
</td>
  </tr>
 </tbody>
</table>



<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Eliminar campos

<!--When they release the sharing of fields between other records, revise this section.  -->

{{step1-to-maestro}}

Esto abre el espacio de trabajo al que se accedió por última vez en Workfront Planning.
1. Haga clic en la tarjeta de un tipo de registro cuyos campos desee eliminar.
1. (Condicional) Seleccione una **Vista de tabla** desde el **Ver** menú desplegable en la esquina superior derecha de la página tipo de registro.
1. Busque el campo que desea eliminar en los encabezados de columna, pase el ratón sobre el encabezado de columna y, a continuación, haga clic en la flecha hacia abajo situada después del nombre del campo.

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Clic **Eliminar**. <!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. Clic **Eliminar** para confirmar.

   El campo se elimina, no se puede recuperar y ya no se puede asociar a ningún registro.
