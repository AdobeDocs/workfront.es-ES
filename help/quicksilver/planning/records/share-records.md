---
title: Compartir registros
description: Puede compartir registros con otros usuarios para aumentar la colaboración.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 83ff53ac-f18e-4b71-bdb2-57e05d69ed29
source-git-commit: 5a4ceb3bd7a5f121312d26775b6cf91604585775
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 52%

---


<!--should this move to the Access folder when we have sharing for ALL the objects???-->

<!--take out preview and production references at release-->

# Compartir registros

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Para colaborar con otros usuarios, puede compartir registros con otros usuarios.

Puede compartir un registro de Adobe Workfront Planning de las siguientes maneras:

* Copie el vínculo de la página de registro desde el explorador cuando se abra la página.

* Copie un vínculo a la página del registro cuando vea registros en la vista de tabla del tipo de registro.

* Puede compartir todos los registros de un área de trabajo con otros usuarios compartiendo el área de trabajo <span class="preview"> y el tipo de registro.</span>

  Para obtener más información, consulte los siguientes artículos:

   * [Compartir un espacio de trabajo](/help/quicksilver/planning/access/share-workspaces.md)

  <div class="preview">

   * [Compartir un tipo de registro](/help/quicksilver/planning/access/share-record-types.md)

  </div>

En este artículo se describe cómo copiar un vínculo a la página de un registro desde la vista de tabla de un tipo de registro.

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso.

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
   <p> Productos</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Planificación de Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Plan de Adobe Workfront*</p></td> 
   <td> 
<p>Cualquiera de los siguientes planes de Workfront:</p> 
<ul><li>Seleccionar</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning no está disponible para planes Workfront heredados</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Paquete de planificación de Adobe Workfront*</p></td> 
   <td> 
<p>Cualquiera </p> 
<p>Para obtener más información sobre qué se incluye en cada plan de Workfront Planning, póngase en contacto con su administrador de cuentas de Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>plataforma de Adobe Workfront</p></td> 
   <td> 
<p>La instancia de Workfront de su organización debe incorporarse a Adobe Unified Experience para poder acceder a todas las funcionalidades de Workfront Planning.</p> 
<p>Para obtener más información, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience para Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront*</p></td> 
   <td><p> Colaborador, Ligero o Estándar </p>
   <p>Workfront Planning no está disponible para licencias de Workfront heredadas</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuración de nivel de acceso</p></td> 
   <td> <p>No hay controles de nivel de acceso para Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>  <p>Ver permisos superiores a un espacio de trabajo <span class="preview">y tipo de registro</span> para compartir   Crear un registro mediante un vínculo </p>
   <p>Administre permisos a un espacio de trabajo <span class="preview">y tipo de registro</span> para compartir los registros del espacio de trabajo </p>
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Plantilla de diseño</p></td> 
   <td> <p>A todos los usuarios, incluidos los administradores de Workfront, se les debe asignar una plantilla de diseño que incluya el área de Planning en el menú principal. </p> </td> 
  </tr> 
</tbody> 
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--OLD:

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
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls for Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace to share a record using a link </p>
   <p>Manage permissions to a workspace to share the workspace the record belongs to </p>
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
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

Solo los usuarios con permisos de administración de un espacio de trabajo pueden compartirlo con otros.

Para obtener más información, consulte [Compartir un espacio de trabajo](/help/quicksilver/planning/access/share-workspaces.md).


<div class="preview">

## Compartir todos los registros de un tipo de registro compartiendo el tipo de registro

En el entorno Producción, los registros heredan los permisos del espacio de trabajo.

En el entorno de vista previa, los registros heredan los permisos del tipo de registro.

De forma predeterminada, los tipos de registro heredan los permisos del espacio de trabajo.

Sin embargo, puede realizar cualquiera de las siguientes acciones:

* Deshabilite los permisos heredados del espacio de trabajo en un tipo de registro. Esto quita los permisos más altos de los registros, pero mantiene los permisos de Vista en el espacio de trabajo, el tipo de registro y los registros.
* Conceder manualmente permisos a los usuarios para un tipo de registro, incluso cuando no tengan permisos para el espacio de trabajo. Esto les otorga automáticamente permisos de Vista al espacio de trabajo. Esto otorga permisos a los usuarios para acceder a los registros.

Solo los usuarios con permisos de Administración de un espacio de trabajo pueden compartir sus tipos de registros y registros con otros usuarios.

Para obtener más información, vea [Compartir tipos de registros](/help/quicksilver/planning/access/share-record-types.md).

</div>
