---
title: Eliminar espacios de trabajo
description: Puede eliminar los espacios de trabajo cuando ya no sean relevantes.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
source-git-commit: ce015eba8291995eec1611917896a0e797f820cc
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Eliminar espacios de trabajo

>[!IMPORTANT]
>
>La información de este artículo hace referencia a Adobe Maestro, que es una nueva oferta de Adobe Workfront.
>
>En la actualidad, Adobe Maestro forma parte de un programa beta abierto a un número limitado de clientes. Debe ser cliente de Workfront para utilizar las funciones de Maestro.
>
>Póngase en contacto con su representante de cuentas para obtener más información acerca de cómo unirse al programa beta de Maestro.
>
>Para obtener más información, consulte [Introducción a Adobe Maestro](../maestro-overview.md).

En Adobe Maestro, los espacios de trabajo son ubicaciones centralizadas para que los equipos planifiquen el trabajo. Para obtener más información, consulte [Creación de espacios de trabajo](../architecture/delete-workspaces.md).

Puede eliminar los espacios de trabajo que ya no sean relevantes.

Se recomienda volver a crear algunos o todos los tipos de registros y taxonomías asociados al espacio de trabajo que desee eliminar en otro espacio de trabajo antes de eliminarlo.

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
   <td role="rowheader"><p>Configuración del nivel de acceso</p></td>
   <td> <p>No hay controles de nivel de acceso para Maestro</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Permisos</p></td>
   <td> <p>Administración de permisos en un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>
   <p><b>NOTA</b></p>
   Los usuarios de licencias de trabajo y solicitud no pueden crear un espacio de trabajo, pero sí eliminarlo, si tienen permisos de administración. 
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>El administrador de Workfront o de grupo debe agregar el área de Maestro en la plantilla de diseño. Para obtener más información, consulte <a href="../access/access-overview.md">Acceso a información general</a>. </p>  
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

* Al eliminar espacios de trabajo, también se eliminan todos los tipos de registros, taxonomías, registros y sus campos.
* Los espacios de trabajo eliminados y la información que contienen no se pueden recuperar.

## Eliminar un espacio de trabajo

1. Haga clic en **Menú principal** icono ![](assets/main-menu-workfront.png) en la esquina superior derecha de Workfront o en la **Menú principal** icono ![](assets/main-menu-shell.png)  en la esquina superior izquierda, si está disponible, haga clic en **Maestro** ![](assets/maestro-icon.png).

   Esto abre el último espacio de trabajo al que accedió.

1. (Opcional) Expanda la flecha hacia abajo a la derecha del nombre de un espacio de trabajo existente y seleccione el espacio de trabajo que desea eliminar.
1. Haga clic en **Más** menú ![](assets/more-menu.png) junto al nombre del espacio de trabajo y haga clic en **Eliminar**.
1. Clic **Eliminar** para confirmar.

   El espacio de trabajo se elimina y no se puede recuperar. También se elimina cualquier tipo de registro, taxonomía, sus registros y los campos asociados a ellos. <!--ensure this is right after closed beta-->
