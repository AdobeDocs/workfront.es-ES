---
title: Compartir registros
description: Puede compartir registros con otros usuarios para aumentar la colaboración.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 83ff53ac-f18e-4b71-bdb2-57e05d69ed29
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 50%

---


<!--should this move to the Access folder when we have sharing for ALL the objects???-->

<!--take out preview and production references at release-->

# Compartir registros

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>  -->

{{planning-important-intro}}

Para colaborar con otros usuarios, puede compartir registros con otros usuarios.

Puede compartir un registro de Adobe Workfront Planning de las siguientes maneras:

* Copie el vínculo de la página de registro desde el explorador cuando se abra la página.

* Copie un vínculo a la página del registro cuando vea registros en la vista de tabla del tipo de registro.

* Puede compartir todos los registros de un área de trabajo con otros usuarios compartiendo el área de trabajo y el tipo de registro.

  Para obtener más información, consulte los siguientes artículos:

   * [Compartir un espacio de trabajo](/help/quicksilver/planning/access/share-workspaces.md)

   * [Compartir un tipo de registro](/help/quicksilver/planning/access/share-record-types.md)

En este artículo se describe cómo copiar un vínculo a la página de un registro desde la vista de tabla de un tipo de registro.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>paquete de Adobe Workfront</p></td> 
   <td> 
<p>Cualquier Workfront y cualquier paquete de Planning</p> <p>Cualquier flujo de trabajo y cualquier paquete de Planning</p>
<p>Para obtener más información sobre lo que se incluye en cada paquete de Workfront Planning, póngase en contacto con su representante de cuentas de Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Colaborador o superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>  <p>Ver permisos superiores a un espacio de trabajo y tipo de registro para compartir un registro mediante un vínculo</p>
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>  </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> A los usuarios con una licencia Light o Contributor se les debe asignar una plantilla de diseño que incluya Planning.
   <p>Los usuarios estándar y los administradores del sistema tienen las áreas de Planning habilitadas de forma predeterminada.</p></div></li></ul>
</td>
  </tr> 
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++  


<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Contributor or higher license </p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>  <p>View or higher permissions to a workspace and record typeto share   a record using a link </p>
   <p>Manage permissions to a workspace and record type to share the records in the workspace </p>
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
</td>
  </tr>
</tbody> 
</table> -->


## Compartir vínculos de registros desde la vista de tabla de tipo de registro

{{step1-to-planning}}

Se abre el espacio de trabajo al que accedió por última vez.

1. Haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.

1. (Condicional) En el menú desplegable **Ver** de la esquina superior derecha de la tabla, seleccione una vista de tabla. Esta debe ser la vista predeterminada, a menos que haya visto el tipo de registro en la vista de cronología cuando accedió por última vez.

   Los registros asociados al tipo de registro seleccionado se muestran en la vista de tabla.

1. Haga clic con el botón derecho en una fila de registro

   O

   Pase el ratón sobre el nombre de un registro, haga clic en el menú **Más** ![Menú más](assets/more-menu.png) y, a continuación, haga clic en **Copiar vínculo**.

   ![Menú contextual para la fila de registros](assets/contextual-menu-for-record-row.png)

   El vínculo se copia en el portapapeles.

1. Pegue el vínculo en un correo electrónico o en una ventana de chat para compartirlo con otros usuarios. Cuando los usuarios reciben el vínculo, se abre la página de registro.

   >[!TIP]
   >
   >Los campos de la página de registro son los mismos campos disponibles en la vista Tabla del registro.


   <!--add there when it will be available: if they have access to this record-->

## Compartir todos los registros de un espacio de trabajo compartiendo el espacio de trabajo

Puede compartir todos los registros de un espacio de trabajo cuando comparta el espacio de trabajo con otros usuarios.

Los tipos de registro y los registros heredan los mismos permisos del espacio de trabajo.

Solo los usuarios con permisos de administración de un espacio de trabajo pueden compartirlo con otros.

Para obtener más información, consulte [Compartir un espacio de trabajo](/help/quicksilver/planning/access/share-workspaces.md).

## Compartir todos los registros de un tipo de registro compartiendo el tipo de registro

Los registros heredan los permisos del tipo de registro.

De forma predeterminada, los tipos de registro heredan los permisos del espacio de trabajo.

Sin embargo, puede realizar cualquiera de las siguientes acciones:

* Deshabilite los permisos heredados del espacio de trabajo en un tipo de registro. Esto quita los permisos más altos de los registros, pero mantiene los permisos de Vista en el espacio de trabajo, el tipo de registro y los registros.
* Conceder manualmente permisos a los usuarios para un tipo de registro, incluso cuando no tengan permisos para el espacio de trabajo. Esto les otorga automáticamente permisos de Vista al espacio de trabajo. Esto otorga permisos a los usuarios para acceder a los registros.

Solo los usuarios con permisos de Administración de un espacio de trabajo pueden compartir sus tipos de registros y registros con otros usuarios.

Para obtener más información, vea [Compartir tipos de registros](/help/quicksilver/planning/access/share-record-types.md).

