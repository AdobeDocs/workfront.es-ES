---
title: Compartir vistas
description: Puede compartir una vista con otros usuarios para garantizar la colaboración al utilizar Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 673dd888-3135-48b0-8198-c8d6d6706ddf
source-git-commit: 6ec985d10a5fd7a4a9307b705f48734d76aec181
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 0%

---

<!--update the metadata and description when we turn this article live-->

# Compartir vistas

{{maestro-important-intro}}

Puede compartir una vista con otros usuarios para garantizar la colaboración al trabajar con registros en Adobe Workfront Planning.

Al conceder permisos a un espacio de trabajo, no se conceden permisos a otros usuarios para las vistas de las páginas de tipo de registro. Debe conceder permisos a vistas individuales de una página de tipo de registro para compartirlas con otros usuarios.

Cuando comparte una vista, otorga a otros permisos para acceder a todos los elementos de la vista. Por ejemplo, cuando se les conceden permisos de administración de una vista, pueden modificar la apariencia de agrupación, filtro, ordenación o barra.

<!--
You can share a view with the following entities: 

* Workfront users
* Workfront groups
* Publicly, with users outside Workfront
-->

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
<p>Su organización debe estar inscrita en el programa beta cerrado de Adobe Workfront Planning. Póngase en contacto con el representante de cuentas para obtener más información sobre esta nueva oferta. </p>
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
   <td> No hay controles de acceso para Adobe Workfront Planning </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Permisos de objeto</p></td>
   <td> <p>Administración de permisos en una vista</p>

</td>
  </tr>

<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>A todos los usuarios, incluidos los administradores de Workfront, se les debe asignar una plantilla de diseño que incluya el área de Planning en el menú principal. </p> <p>Para obtener más información, consulte <a href="/help/quicksilver/maestro/access/access-overview.md">Acceso a información general</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

## Compartir permisos en una vista <!--internally-->

Puede compartir las vistas que ha creado o las vistas para las que tiene permisos de administración <!--with users or groups in Workfront-->.

>[!NOTE]
>
>Los administradores del sistema no pueden ver ni compartir vistas que no hayan creado ellos mismos. Solo pueden acceder a las vistas que se comparten con ellos o compartirlas.
>
>Los administradores del sistema solo pueden tener permisos de Administración para una vista.

{{step1-to-maestro}}

1. Abra el espacio de trabajo cuya vista desee compartir y, a continuación, haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.

1. En la pestaña Ver, pase el ratón sobre la vista que quiera compartir y haga clic en **Más** menú ![](assets/more-menu.png) a la derecha del nombre de la vista y haga clic en **Compartir**.

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

   <!--The Internal sharing tab should be selected by default.-->

1. En el **Conceder acceso de visualización a** , empiece a escribir el nombre de un usuario o grupo y, a continuación, haga clic en él cuando se muestre en la lista.  <!--replace screen shot below-->

   ![](assets/sharing-a-view-ui-with-groups.png)

1. Seleccione uno de los siguientes niveles de permisos en el menú desplegable:
   * Ver
   * Administrar

     Para obtener información sobre los niveles de permisos y las acciones que los usuarios pueden realizar para cada nivel, consulte [Información general sobre los permisos de uso compartido en Adobe Workfront Planning](../access/sharing-permissions-overview.md).

     Los administradores del sistema siempre reciben permisos de administración para las vistas compartidas con ellos.

1. Clic **Copiar vínculo** para copiar un vínculo a la vista en el portapapeles.
1. Compartir el vínculo copiado con otros usuarios. Los usuarios que reciban el vínculo deben ser usuarios activos e iniciar sesión en Workfront para poder acceder a la página de tipo de registro y mostrarla en la vista seleccionada.
1. Haga clic en **Guardar**.

<!--
## Share permissions to a view publicly

You can share views you created or views you have Manage permissions to with people that do not have a Workfront license and who might be external to your organization. 

Consider the following when publicly sharing a Workfront Planning view: 

* You can share a public link to a record type page that displays in the view you are sharing.
* People accessing the record type with the public link you provide have View permissions to the record page. They cannot modify the view, the records, or any of the fields that are visible in the view. 
* The shared public link must have an expiration date after which the link is no longer accessible. 

To share a view publicly in Workfront Planning: 

{{step1-to-maestro}}

1. Open the workspace whose view you want to share, then click a record type card. 

   This opens the record type page.

1. From the view tab, hover over the view you want to share and click the **More** menu ![](assets/more-menu.png) to the right of the view name, then click **Share**. 

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

1. Click **Public sharing**.

1. Enable the **Create public link** setting.

   A link becomes available. This is a public link. When shared, anyone with the link, including people from outside your organization can access the record type page, and view records and fields on the page. 

1. Click the **Copy link** icon ![](assets/copy-link-view.png) to copy the link to your clipboard. 

1. Manually enter a date, or use the calendar in the **Link expiration date** field to select an expiration date for the public link. The record page view will not be accessible after the selected date. 

1. Click **Save**.

1. Paste the link you copied to an email, chat message, document, or in a Workfront comment to share it with others. 

-->


## Eliminación de permisos de una vista

{{step1-to-maestro}}

1. Abra el espacio de trabajo cuya vista desee dejar de compartir y, a continuación, haga clic en una tarjeta de tipo de registro. Se abre la página de tipo de registro.
1. Pase el ratón sobre el nombre de la pestaña de la vista desde la que quiera quitar el uso compartido y haga clic en **Más** menú ![](assets/more-menu.png), luego haga clic en **Compartir**.
1. Busque el usuario o grupo que desea eliminar y haga clic en **Eliminar** en el menú desplegable de permisos, a la derecha del nombre del usuario o grupo.
1. Clic **Guardar**.
El usuario o los usuarios que pertenecen al grupo eliminado ya no tienen acceso a la vista. No hay ninguna notificación para los usuarios que se han eliminado del acceso a la vista de que perdieron este acceso.

<!--Replace the above instructions with the following when public sharing is released: 

{{step1-to-maestro}}

1. Open the workspace whose view you want to stop sharing, then click a record type card. This opens the record type page.
1. Hover over the tab name of the view you want to remove sharing from and click the **More** menu ![](assets/more-menu.png), then click **Share**.
1. To remove the internal sharing of a view, do the following: 

   1. Ensure the **Internal sharing** tab is selected.
   1. Find the user or group what you want to remove, expand the permissions drop-down menu to the right of the user's or group's name, then click **Remove**.

1. To remove the public sharing of a view, do the following: 

   1. Click the **Public sharing** tab.
   1. Deselect the **Create public link** option. 

1. Click **Save**.
   
   People no longer have access to the view. There is no notification for the users that have been removed from accessing the view that they no longer have this access.-->