---
title: Compartir registros mediante un vínculo
description: Puede compartir registros con otros usuarios para aumentar la colaboración.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 83ff53ac-f18e-4b71-bdb2-57e05d69ed29
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/Ct6I5wnivCVr3V86Zj4F7stm2IVUJVH50yvTRyWFuUA
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 751
ht-degree: 42%

---

<!--should this move to the Access folder when we have sharing for ALL the objects???-->

<!--take out preview and production references at release-->

# Compartir registros usando un vínculo

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Para colaborar con otros usuarios, puede compartir registros con otros usuarios.

Puede compartir un registro de Adobe Workfront Planning de las siguientes maneras:

* Copie el vínculo de la página de registro desde el explorador cuando se abra la página.

* Copie un vínculo a la página del registro cuando vea registros en la vista de tabla del tipo de registro.

* En el entorno de producción:

   * Puede compartir todos los registros de un área de trabajo con otros usuarios compartiendo el área de trabajo y el tipo de registro.

     Para obtener más información, consulte los siguientes artículos:

      * [Compartir un espacio de trabajo](/help/quicksilver/planning/access/share-workspaces.md)

      * [Compartir un tipo de registro](/help/quicksilver/planning/access/share-record-types.md)

<div class="preview">

* En el entorno de vista previa:

   * Puede compartir registros individuales con personas, equipos, funciones, grupos o empresas.

     Para obtener más información, consulte [Compartir registros](/help/quicksilver/planning/access/share-records.md).

</div>



<!--take out the sentence below when we release record-level sharing-->

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
   <td role="rowheader"><p>Paquete de Adobe Workfront</p></td> 
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


<!--
Old:
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
</table>
-->


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

De forma predeterminada, los tipos de registro y los registros heredan los mismos permisos del espacio de trabajo.

Solo los usuarios con permisos de administración de un espacio de trabajo pueden compartirlo con otros.

Para obtener más información, consulte [Compartir un espacio de trabajo](/help/quicksilver/planning/access/share-workspaces.md).

## Compartir todos los registros de un tipo de registro compartiendo el tipo de registro

De forma predeterminada, los registros heredan los permisos del tipo de registro.

De forma predeterminada, los tipos de registro heredan los permisos del espacio de trabajo.

Sin embargo, puede realizar cualquiera de las siguientes acciones:

* Deshabilite los permisos heredados del espacio de trabajo en un tipo de registro. Esto quita los permisos más altos de los registros, pero mantiene los permisos de Vista en el espacio de trabajo, el tipo de registro y los registros.
* Conceder manualmente permisos a los usuarios para un tipo de registro, incluso cuando no tengan permisos para el espacio de trabajo. Esto les otorga automáticamente permisos de Vista al espacio de trabajo. De forma predeterminada, concede permisos de visualización a los usuarios de los registros.

Solo los usuarios con permisos de Administración de un espacio de trabajo pueden compartir sus tipos de registros y registros con otros usuarios.

Para obtener más información, vea [Compartir tipos de registros](/help/quicksilver/planning/access/share-record-types.md).

<div class="preview">

## Uso compartido de registros individuales

Los usuarios heredan los permisos de registro del espacio de trabajo y el tipo de registro de forma predeterminada.

Para conceder sólo a usuarios seleccionados con permisos de tipo de registro y permisos de administración sólo a determinados registros, puede deshabilitar los permisos heredados en registros seleccionados y conceder sólo a esos usuarios acceso de administración a esos registros.

Puede ajustar los permisos para un registro o para varios registros al mismo tiempo, de forma masiva.

Para obtener más información, consulte [Compartir registros](/help/quicksilver/planning/access/share-records.md).

</div>

