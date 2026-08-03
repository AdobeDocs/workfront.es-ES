---
title: Eliminar espacios de trabajo
description: Puede eliminar los espacios de trabajo cuando ya no sean relevantes.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/yzpirNfY0Hsp0cbClQA8dFqhgqbpK8ZryIyeq4tBAgw
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 347c3e87fea0289616bf1a52779c07501a8ec69d
workflow-type: tm+mt
source-wordcount: 459
ht-degree: 38%

---

# Eliminar espacios de trabajo

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

En Adobe Workfront Planning, los espacios de trabajo son ubicaciones centralizadas para que los equipos planifiquen el trabajo. Para obtener más información, consulte [Crear espacios de trabajo](/help/quicksilver/planning/architecture/create-workspaces.md).

Puede eliminar los espacios de trabajo que ya no sean relevantes.

Se recomienda volver a crear algunos o todos los tipos de registros, registros, campos y vistas asociados con el espacio de trabajo que desee eliminar en otro espacio de trabajo antes de eliminarlo.

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
<p>Cualquier Workfront o flujo de trabajo con un paquete de Planning</p> 
O
<p>Cualquier planificación de Workfront cuando se compra como producto independiente</p> 
 </tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Cualquiera</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de planificación de Adobe</p></td> 
   <td><p>Cualquiera</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuración de nivel de acceso</p></td> 
   <td> <p>Debe agregar un tipo de licencia de flujo de trabajo y de Planning al nivel de acceso cuando tenga un flujo de trabajo y un paquete de Planning a la vez</p>   
</td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Administración de permisos en un espacio de trabajo</p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>  </td> 
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
   <td><p> Standard </p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>You must add both a Workflow and a Planning license type to the access level when you have both a Workflow and a Planning package</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table>
-->

## Consideraciones sobre la eliminación de espacios de trabajo

* Al eliminar espacios de trabajo, también se eliminan todos los tipos de registros, registros, sus campos y vistas.
* Los espacios de trabajo eliminados y la información que contienen no se pueden recuperar.

## Eliminación de un espacio de trabajo

{{step1-to-planning}}

1. (Condicional) Si es administrador de Workfront, haga clic en una de las siguientes opciones:

   * **Espacios de trabajo en los que participo** para acceder a los espacios de trabajo que ha creado
   * **Todos los espacios de trabajo** para tener acceso a los espacios de trabajo compartidos con usted o creados

   >[!NOTE]
   >
   >No puede eliminar los espacios de trabajo en la ficha **Espacios de trabajo de ejemplo**. Se recomienda utilizar el paquete de plantillas de varios espacios de trabajo para crear espacios de trabajo similares a los de la pestaña Espacio de trabajo de muestra. Para obtener más información, consulte [Creación de espacios de trabajo](/help/quicksilver/planning/architecture/create-workspaces.md).

1. (Opcional) Haga clic en **Mostrar todo** para mostrar espacios de trabajo adicionales. El vínculo **Mostrar todo** solo se muestra cuando tiene más de dos filas de tarjetas de área de trabajo.
1. (Opcional) Haga clic en **Mostrar menos** para limitar el número de espacios de trabajo que se muestran en la pantalla.
1. Para eliminar un espacio de trabajo, realice una de las siguientes acciones:

   * Pase el ratón sobre la tarjeta del área de trabajo y luego haga clic en el menú **Más** ![Menú Más](assets/more-menu.png) en la esquina superior derecha de la tarjeta
     O
   * Haga clic en el icono **search** ![icono de búsqueda](assets/search-icon.png) en la esquina superior derecha de la página de Workspaces para buscar un área de trabajo por nombre y haga clic en una tarjeta de área de trabajo para abrir el área de trabajo; a continuación, haga clic en el menú **Más** ![Menú Más](assets/more-menu.png) situado a la derecha del nombre del área de trabajo.

   >[!TIP]
   >
   >Puede utilizar la siguiente combinación de teclas para abrir el cuadro de búsqueda global desde cualquier página de Workfront Planning y buscar espacios de trabajo:
   >
   >* CTRL+K para Windows
   >* ⌘+K para Mac

1. Haga clic **eliminar**.

   ![Eliminar permanentemente la confirmación del espacio de trabajo](assets/permanently-delete-workspace-confirmation.png)

1. Escriba “**Eliminar**” en el espacio proporcionado y haga clic en **Eliminar permanentemente**. Esto no distingue entre mayúsculas y minúsculas.

   El espacio de trabajo se elimina y no se puede recuperar. También se elimina cualquier tipo de registro, registro, campo y vista asociada con ellos. <!--ensure this is right at or before GA-->


