---
title: Compartir vistas
description: Puede compartir una vista con otros usuarios para garantizar la colaboración al utilizar las funcionalidades de planificación de Adobe Workfront.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 4c62b567fa1ebec37fc64831757eb67d4a048c1f
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 0%

---


<!--update the metadata and description when we turn this article live-->

# Compartir vistas

{{maestro-important-intro}}

Puede compartir una vista con otros usuarios para garantizar la colaboración al trabajar con registros en las funciones de planificación de Adobe Workfront.

Al conceder permisos a un espacio de trabajo, no se conceden permisos a otros usuarios para las vistas de las páginas de tipo de registro. Debe conceder permisos a vistas individuales de una página de tipo de registro para compartirlas con otros usuarios.

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
<p>Su organización debe estar inscrita en el programa beta cerrado de capacidades de planificación de Adobe Workfront. Póngase en contacto con el representante de cuentas para obtener más información sobre esta nueva oferta. </p>
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
   <td> No hay controles de acceso para las funciones de planificación de Adobe Workfront</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Permisos de objeto</p></td>
   <td> <p>Administración de permisos en una vista</p>

</td>
  </tr>

<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>A todos los usuarios, incluidos los administradores de Workfront, se les debe asignar una plantilla de diseño que incluya el área de Maestro en el menú principal. </p> <p>Para obtener más información, consulte <a href="/help/quicksilver/maestro/access/access-overview.md">Acceso a información general</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

## Compartir permisos en una vista

Puede compartir vistas que haya creado o vistas para las que tenga permisos de administración.

>[!NOTE]
>
>Los administradores del sistema no pueden ver ni compartir vistas que no hayan creado ellos mismos. Solo pueden acceder a las vistas que se comparten con ellos o compartirlas.

<!--for above note - add when this releases: System administrators can have only Manage permissions to a view.-->

{{step1-to-maestro}}

1. Abra el espacio de trabajo cuya vista desee compartir y, a continuación, haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.

1. En el menú desplegable de vista <!--tab-->, pase el ratón sobre la vista que quiera compartir y haga clic en **Más** menú ![](assets/more-menu.png) a la derecha del nombre de la vista y haga clic en **Compartir**.

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

1. En el **Conceder acceso de visualización a** , empiece a escribir el nombre de un usuario o grupo y, a continuación, haga clic en él cuando se muestre en la lista.

   ![](assets/sharing-a-view-ui-with-groups.png)

1. Seleccione uno de los siguientes niveles de permisos en el menú desplegable:
   * Ver
   * Administrar

     Para obtener información sobre los niveles de permisos y las acciones que los usuarios pueden realizar para cada nivel, consulte [Información general sobre los permisos de uso compartido en las funciones de planificación de Adobe Workfront](../access/sharing-permissions-overview.md).
1. Clic **Copiar vínculo** para copiar un vínculo a la vista en el portapapeles.
1. Compartir el vínculo copiado con otros usuarios. Los usuarios que reciban el vínculo deben ser usuarios activos e iniciar sesión en Workfront para poder acceder a la página de tipo de registro y mostrarla en la vista seleccionada.
1. Haga clic en **Guardar**.

## Eliminación de permisos de una vista

{{step1-to-maestro}}

1. Abra el espacio de trabajo cuya vista desee compartir y, a continuación, haga clic en una tarjeta de tipo de registro. Se abre la página de tipo de registro.
1. En el menú desplegable de vista, pase el ratón sobre la vista que quiera compartir y haga clic en **Más** menú ![](assets/more-menu.png) a la derecha del nombre de la vista y haga clic en **Compartir**.
1. Busque el usuario o grupo que desea eliminar y haga clic en **Eliminar** en el menú desplegable de permisos, a la derecha del nombre del usuario o grupo.
1. Clic **Guardar**.
El usuario o los usuarios que pertenecen al grupo eliminado ya no tienen acceso a la vista. No hay ninguna notificación para los usuarios que se han eliminado del acceso a la vista.
