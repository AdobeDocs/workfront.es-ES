---
title: Eliminar campos
description: En Adobe Maestro, puede eliminar los campos personalizados que ya no son relevantes.
hidefromtoc: true
hide: true
source-git-commit: f058c369bdb3b991910d3a820895de73ea4709f0
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 0%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Eliminar campos

>[!IMPORTANT]
>
>En la actualidad, Adobe Maestro forma parte de un programa beta abierto a un número limitado de clientes.
>
>Póngase en contacto con su representante de cuentas para obtener más información acerca de cómo unirse al programa beta de Maestro.
>
>Para obtener más información, consulte [Introducción a Adobe Maestro](../maestro-overview.md).

En Adobe Maestro, puede crear campos personalizados para almacenar información sobre los registros.

Para obtener información sobre cómo crear campos personalizados en Maestro, consulte [Creación de campos](../architecture-and-fields/create-fields.md).

Puede eliminar los campos de Maestro que ya no sean relevantes.

## Consideraciones acerca de la eliminación de campos Maestro:

* Puede eliminar los campos que haya creado o los creados por otros usuarios. <!--this will change with access levels/ permissions-->
* Los campos sólo se pueden eliminar en la tabla de tipo de registro.
* La información almacenada en el campo se elimina y no se puede recuperar.
  <!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

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

## Eliminar campos

<!--When they release the sharing of fields between other records, revise this section.  -->

1. Haga clic en **Menú principal** icono ![](assets/main-menu-workfront.png) en la esquina superior derecha de Workfront, <!--or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> luego haga clic en **Maestro** ![](assets/maestro-icon.png).

   Se abrirá el área de trabajo a la que se accedió por última vez en Maestro.
1. Haga clic en la tarjeta de un tipo de registro cuyos campos desee eliminar.
1. (Condicional) Seleccione una **Vista de tabla** desde el **Ver** menú desplegable en la esquina superior derecha de la página tipo de registro.
1. Busque el campo que desea eliminar en los encabezados de columna, pase el ratón sobre el encabezado de columna y, a continuación, haga clic en la flecha hacia abajo situada después del nombre del campo.
1. Clic **Eliminar**. <!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. Clic **Eliminar** para confirmar.

   El campo se elimina, no se puede recuperar y ya no se puede asociar a ningún registro.