---
title: Conceder acceso a Adobe Maestro
description: Obtenga información sobre cómo conceder acceso y compartir información en Adobe Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 475a519d-d3bd-4461-8099-0e296d556d34
source-git-commit: 85f499a429d4223c62b7b13dc0b1d10e8e79e9ed
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 0%

---

<!--update the metadata and description when we turn this article live; also, update title after Bob adds Maestro as a product-->

# Conceder acceso a Adobe Maestro

>[!IMPORTANT]
>
>La información de este artículo hace referencia a Adobe Maestro, que es una nueva oferta de Adobe Workfront.
>
>En la actualidad, Adobe Maestro forma parte de un programa beta abierto a un número limitado de clientes. Para tener acceso a Maestro, debe ser cliente de Workfront
>
>Póngase en contacto con su representante de cuentas para obtener más información acerca de cómo unirse al programa beta de Maestro.
>
>Para obtener más información, consulte [Introducción a Adobe Maestro](../maestro-overview.md).

Todos los usuarios de su organización pueden tener acceso a Maestro si se cumplen los siguientes requisitos previos:

<!--the first requisite will be removed when we go to GA-->

* Su organización está inscrita en el programa beta cerrado de Adobe Maestro.
* Como administrador del sistema, debe agregar el área de Maestro al menú principal mediante una plantilla de diseño.

  Maestro no se muestra en el menú principal de forma predeterminada para ningún usuario, incluidos los administradores del sistema.

  Para obtener más información, consulte [Personalización del menú principal mediante una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

<!-- take out the note below when we release permissions-->

>[!NOTE]
>
>No hay niveles de acceso ni permisos asociados a los usuarios ni a la información de Maestro. Todos los usuarios que tengan activado Maestro en su entorno pueden ver, editar y eliminar toda la información que cualquier otro usuario agregue a Maestro.

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
   <td role="rowheader"><p>Nivel de acceso</p></td>
   <td> <p>Cualquiera que utilice Maestro</p>
   <p>Administrador del sistema o Planifique compartir el área de Maestro en una plantilla de diseño</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>El administrador de Workfront o de grupo debe agregar el área de Maestro a la plantilla de diseño. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--
When permissions is released:

* leave as is for Access levels (I think)
* Add a new row for Permissions: System admin or Manage access to the workspace to share a workspace with others
-->

## Compartir el área de Maestro en el menú principal con otros usuarios

<!--First, contact your account manager to obtain access to the current Maestro closed beta program.-->

Una vez que su organización se haya inscrito en el programa beta de Maestro, puede agregar el área de Maestro al menú principal de todos los usuarios mediante una plantilla de diseño.

1. Iniciar sesión en **Workfront** como administrador de Workfront.

1. Añada el **Maestro** icono ![](assets/maestro-icon.png) a la **Menú principal** uso de un **Plantilla de diseño**.

   Para obtener más información, consulte [Personalización del menú principal mediante una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

1. Asigne la plantilla de diseño a los usuarios que desea que tengan acceso a Maestro.

   Para obtener más información, consulte [Asignar usuarios a una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

   Todos los usuarios asignados a la plantilla ahora pueden acceder a Maestro en su menú principal.

   Los usuarios pueden empezar a crear espacios de trabajo, tipos de registros, registros y campos.

<!--

## Share permissions to a workspace

The following users can share a workspace with other users:

* System administrators can share all workspaces, including the ones that they did not create.
* All other users can share only workspaces for which they have Manage permissions to. 

To share a workspace with others: 

1. Click the **Main Menu** icon ![](assets/dots-main-menu.png) in the upper-right or the **Main Menu** icon ![](assets/lines-main-menu.png) in the upper-left corner or Workfront, if available, then click **Maestro**.
1. Open the workspace you want to share, then click **Share** in the upper-right corner of the screen. (*************add screen shot when UI is finalized and maybe edit the steps*********)
1. In the field provided, start typing the name of a user or a group (******ensure you can share with groups*******), then click it when it displays in the list. 
1. Select one of the following permission levels from the drop-down menu: 
    * View
    * Contribute
    * Manage

        For information about permission levels and what actions users can perform for each level, see [Overview of sharing permissions in Adobe Maestro](../access/sharing-permissions-overview.md).
1. Click **Save**.


## Remove permissions to a workspace

1. Click the **Main Menu** icon ![](assets/dots-main-menu.png) in the upper-right or the **Main Menu** icon ![](assets/lines-main-menu.png) in the upper-left corner of Workfront, if available, then click **Maestro**.
1. Open the workspace you want to remove permissions to, then click **Share** in the upper-right corner of the screen. (********add screen shot when UI is finalized and maybe edit the steps???****)
1. Click the drop-down menu to the right of a user or group name, then click **Remove**. 
1. Click **Save**.

    The user or the users that belong to the group removed no longer have access to the workspace or its objects. 

-->