---
title: Configuración del área de configuración de un tipo de registro
description: Puede editar los tipos de registros una vez guardados en la página Configuración.
hide: true
hidefromtoc: true
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 11%

---


<!--add better metadata at release:

title: Configure Record Type Settings
description: You can edit record types after they have been saved in the Settings page. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog 

-->

# Configuración del área Configuración de un tipo de registro

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Puede establecer opciones adicionales para un tipo de registro después de guardarlos en Adobe Workfront Planning.

En función de las funciones que desee definir para un tipo de registro, puede establecer configuraciones adicionales para él mediante uno de los procedimientos siguientes:

<!--the above will need to be reworded when we add automations and manage request forms to this area-->

* Edición de ellos

  Para obtener más información, consulte [Editar tipos de registros](/help/quicksilver/planning/architecture/edit-record-types.md).

* Configuración de la página Configuración de un tipo de registro.

  Este artículo describe cómo se puede editar un tipo de registro mediante la configuración de la página Configuración.

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
<ul><li><p>Cualquier paquete de Workfront</p></li>
<p>Y</p>
<li><p>Cualquier paquete de Planning para crear tipos de registros conectables</p></li>
<li><p>Paquete de Planning Plus para crear tipos de registros centralizados</p></li>
</ul>
<p>O</p>
<ul><li><p>Un flujo de trabajo y planificación para Prime o Ultimate</p> </li></ul>
<p>Para obtener más información sobre lo que se incluye en cada paquete de Workfront Planning, póngase en contacto con su administrador de cuentas de Workfront. </p> 
   </td>

<tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Estándar</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Permisos de administración en un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>  </td> 
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
   <td><p> Standard </p>
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
   <td>   <p>Manage permissions to a workspace and record type </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Only system administrators can enable record types to connect from other workspaces</p> </td> 
  </tr> 

</tbody> 
</table> 

-->

## Configure la información de tipo de registro en la página Configuración

Puede definir las funcionalidades de varios espacios de trabajo para un tipo de registro configurando la información en la página Configuración.

<!--the intro above will change when we can configure more in this area -->

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo cuyos tipos de registro desee editar.

   Se abre la página del espacio de trabajo y se muestran los tipos de registro.
1. Realice una de las siguientes acciones:

   * Pase el ratón sobre la tarjeta de un tipo de registro y haga clic en el menú **Más** ![Menú más](assets/more-menu.png) en la esquina superior derecha de la tarjeta de tipo de registro; a continuación, haga clic en **Configuración**
O
   * Haga clic en una tarjeta de tipo de registro para abrir la página de tipo de registro, haga clic en el menú **Más** ![Menú Más](assets/more-menu.png) a la derecha del nombre del tipo de registro y, a continuación, haga clic en **Configuración**.

   <!--update screen shot at release-->

   ![Más opciones de menú de la tarjeta de tipo de registro](assets/more-menu-options-from-record-type-card.png)

1. La sección **Configuración del área de trabajo cruzada** está seleccionada de forma predeterminada.
1. Active o desactive una de las siguientes opciones de configuración:

   * **Permita agregar este tipo de registro a otros espacios de trabajo** para indicar que es un tipo de registro global
   * **Permitir la conexión a este tipo de registro en otros espacios de trabajo** para indicar que se trata de un tipo de registro conectable.

   La configuración está desactivada de forma predeterminada.

   Para obtener más información, vea [Configurar las capacidades entre espacios de trabajo para los tipos de registro](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)