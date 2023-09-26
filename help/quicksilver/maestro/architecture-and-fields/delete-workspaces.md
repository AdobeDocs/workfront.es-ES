---
title: Eliminar espacios de trabajo
description: Puede eliminar los espacios de trabajo cuando ya no sean relevantes.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 28602d66b43ec4c30a9f13cff43157b978439d99
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Eliminar espacios de trabajo

>[!IMPORTANT]
>
>En la actualidad, Adobe Maestro forma parte de un programa beta cerrado que está abierto a un número limitado de clientes.
>
>Póngase en contacto con su representante de cuentas para obtener más información acerca de cómo unirse al programa beta de Maestro.
>
>Para obtener más información, consulte [Introducción a Adobe Maestro](../maestro-overview.md).

En Adobe Maestro, los espacios de trabajo son ubicaciones centralizadas para que los equipos planifiquen el trabajo. Para obtener más información, consulte [Creación de espacios de trabajo](../architecture-and-fields/create-workspaces.md).

Puede eliminar los espacios de trabajo que ya no sean relevantes.

Se recomienda volver a crear algunos o todos los tipos de registros y taxonomías asociados al espacio de trabajo que desee eliminar en otro espacio de trabajo antes de eliminarlo.

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
<p>Su organización debe estar inscrita en el programa beta de Adobe Maestro. Póngase en contacto con el representante de cuentas para obtener más información sobre esta nueva oferta. </p>
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

## Consideraciones sobre la eliminación de espacios de trabajo

* Puede eliminar cualquier espacio de trabajo que haya creado usted o cualquier miembro de su organización. <!--this will change with access levels and permissions-->
* Al eliminar espacios de trabajo, también se eliminan todos los tipos de registros, taxonomías y sus campos. <!--asked Lilit because the confirmation says the records don't delete, but not sure how they can exist outside of a workspace?!-->
* Los espacios de trabajo eliminados y la información que contienen no se pueden recuperar.

## Eliminar un espacio de trabajo

1. Haga clic en **Menú principal** icono ![](assets/main-menu-workfront.png) en la esquina superior derecha de Workfront, <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> luego haga clic en **Maestro** ![](assets/maestro-icon.png).

   Esto abre el último espacio de trabajo al que accedió.

1. (Opcional) Expanda la flecha hacia abajo a la derecha del nombre de un espacio de trabajo existente y seleccione el espacio de trabajo que desea eliminar.
1. Haga clic en **Más** menú ![](assets/more-menu.png) junto al nombre del espacio de trabajo y haga clic en **Eliminar**.
1. Clic **Eliminar** para confirmar.

   El espacio de trabajo se elimina y no se puede recuperar. También se elimina cualquier tipo de registro, taxonomía, sus registros y los campos asociados a ellos. <!--ensure this is right after closed beta-->
