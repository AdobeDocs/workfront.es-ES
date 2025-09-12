---
title: Duplicar vistas de registros
description: Si desea conservar varias versiones de una vista y realizar ligeros cambios entre ellas, puede duplicar una vista en Adobe Workfront Planning. Este artículo describe cómo duplicar una vista.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 441a53d1-ad39-41b7-93fe-2ae1836476c9
source-git-commit: bfb0fd2956ffb9384a09882864668d5dba33a53b
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 41%

---

# Duplicar vistas de registros

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


{{planning-important-intro}}

Si desea conservar varias versiones de una vista y realizar ligeros cambios entre ellas, puede duplicar una vista en Adobe Workfront Planning.

Al duplicar una vista, se crean copias idénticas de una vista existente.

Los permisos de uso compartido de la vista original no se transfieren a la vista duplicada.

La duplicación de vistas es idéntica para todos los tipos de vistas en Workfront Planning.

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso. 

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
<p>La instancia de Workfront de su organización debe incorporarse a Adobe Unified Experience para poder acceder a Workfront Planning.</p> 
<p>Para obtener más información, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience para Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront*</p></td> 
   <td><p> Estándar </p>
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
   <td>   <p>Permisos de administración de una vista</p>  
   <p>Ver permisos en una vista para cambiar temporalmente la configuración de la vista o para duplicarla.</p> </td> 
  </tr> 
</tbody> 
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Duplicación de una vista de registros

{{step1-to-planning}}

1. Haga clic en la tarjeta de un espacio de trabajo.

   El espacio de trabajo se abre y los tipos de registro se muestran como tarjetas.

1. Haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.
De forma predeterminada, todos los registros del tipo seleccionado se muestran en la vista de tabla.

1. Pase el ratón sobre la pestaña de la vista que quiera duplicar y haga clic en el menú **Más** ![Menú más](assets/more-menu.png), a la derecha del nombre de la vista; a continuación, haga clic en **Duplicar**.

   ![Menú Ver más en una vista de registro](assets/view-more-menu-with-duplicate-option.png)

   <!--at preview release, replace the step above with this one: 
    1. Depending on which environment you use, do the following: 
    * In the Production environment, hover over one the of the view's names in the view tab, then click **More** ![More menu](assets/more-menu.png) to the left of the view name, then click **Duplicate**. 
    * <span class="preview">In the Preview environment, click the dropdown icon ![Dropdown icon](assets/drop-down-icon.png) next to the current view name, hover over the name of a view, click **More**, then **Duplicate**.</span>-->
   La vista está duplicada y el nombre de la nueva vista sigue el siguiente patrón: `Original view's name (Copy)`. La nueva ficha de vista se muestra al final de todas las fichas de vista.
