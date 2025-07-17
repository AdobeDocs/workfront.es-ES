---
title: Eliminar espacios de trabajo
description: Puede eliminar los espacios de trabajo cuando ya no sean relevantes.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 53%

---


# Eliminar espacios de trabajo

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

En Adobe Workfront Planning, los espacios de trabajo son ubicaciones centralizadas para que los equipos planifiquen el trabajo. Para obtener más información, consulte [Crear espacios de trabajo](/help/quicksilver/planning/architecture/create-workspaces.md).

Puede eliminar los espacios de trabajo que ya no sean relevantes.

Se recomienda volver a crear algunos o todos los tipos de registros, registros, campos y vistas asociados con el espacio de trabajo que desee eliminar en otro espacio de trabajo antes de eliminarlo.

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
   <td>   <p>Permisos de administración en un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p> </td> 
  </tr> 
</tbody> 
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones sobre la eliminación de espacios de trabajo

* Al eliminar espacios de trabajo, también se eliminan todos los tipos de registros, registros, sus campos y vistas.
* Los espacios de trabajo eliminados y la información que contienen no se pueden recuperar.

## Eliminación de un espacio de trabajo

{{step1-to-planning}}

1. (Condicional) Si es administrador de Workfront, haga clic en **Espacios de trabajo en los que participo** para obtener acceso a los espacios de trabajo que creó, o en **Otros espacios de trabajo** para obtener acceso a los espacios de trabajo que otros compartieron con usted.

1. (Opcional) Haga clic en **Mostrar todo** para mostrar espacios de trabajo adicionales. El vínculo **Mostrar todo** solo se muestra cuando tiene más de dos filas de tarjetas de área de trabajo.
1. (Opcional) Haga clic en **Mostrar menos** para limitar el número de espacios de trabajo que se muestran en la pantalla.
1. Para eliminar un espacio de trabajo, realice una de las siguientes acciones:

   * Pase el ratón sobre la tarjeta del área de trabajo y luego haga clic en el menú **Más** ![Menú Más](assets/more-menu.png) en la esquina superior derecha de la tarjeta
O
   * Haga clic en una tarjeta de área de trabajo para abrir el área de trabajo y, a continuación, haga clic en el menú **Más** ![Menú Más](assets/more-menu.png) situado a la derecha del nombre del área de trabajo.
1. Haga clic **eliminar**.

   ![Eliminar permanentemente la confirmación del espacio de trabajo](assets/permanently-delete-workspace-confirmation.png)

1. Escriba “**Eliminar**” en el espacio proporcionado y haga clic en **Eliminar permanentemente**. Esto no distingue entre mayúsculas y minúsculas.

   El espacio de trabajo se elimina y no se puede recuperar. También se elimina cualquier tipo de registro, registro, campo y vista asociada con ellos. <!--ensure this is right at or before GA-->
