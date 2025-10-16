---
title: Editar tipos de registro
description: Puede editar los tipos de registro una vez guardados. Los tipos de registro son los tipos de objetos de Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: 2fb95d37c32984e248767993c4858038d27e0590
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 31%

---


# Editar tipos de registro

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Los tipos de registro son los tipos de objetos de Adobe Workfront Planning. Puede editar el aspecto de los tipos de registro que usted o cualquier otra persona hayan creado. Para obtener información sobre cómo crear tipos de registro de Workfront Planning, consulte [Crear tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md).

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
<p>Cualquier paquete de Workfront y Planning</p>
<p>Cualquier paquete de Workfront y Planning</p>
<p><b>NOTA</b></p>
<p>Para configurar tipos de registros conectables: </p>
<ul> 
<li><p>Cualquier paquete Workfront y cualquier paquete Planning</p></li>
<p>O</p>
<li><p>Cualquier flujo de trabajo y un paquete de Planning Prime o Ultimate</p></li></ul>

<div class="preview">
<p>Para configurar tipos de registros globales:</p>

<ul> 
<li><p>Cualquier paquete Workfront y un paquete Planning Plus</p></li>
<p>O</p>
<li><p>Cualquier flujo de trabajo y un paquete de Planning Prime o Ultimate</p></li></ul>
<p>Para obtener más información sobre lo que se incluye en cada paquete de Workfront Planning, póngase en contacto con su representante de cuentas de Workfront. </p>

</div>
   </td> </tr>
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Estándar</p>
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
</table> -->

## Editar tipos de registro

{{step1-to-planning}}

1. Haga clic en el área de trabajo cuyos tipos de registro desee editar.

   Se abre la página del espacio de trabajo y se muestran los tipos de registro.
1. Realice una de las siguientes acciones:

   * Pase el ratón sobre la tarjeta de un tipo de registro y haga clic en el menú **Más** ![Menú más](assets/more-menu.png) en la esquina superior derecha de la tarjeta de tipo de registro; a continuación, haga clic en **Editar**
     <span class="preview">o **Configuración**</span>
O
   * Haga clic en una tarjeta de tipo de registro para abrir la página de tipo de registro, haga clic en el menú **Más** ![Menú más](assets/more-menu.png) a la derecha del nombre del tipo de registro y, a continuación, haga clic en **Editar** <span class="preview">o en **Configuración**</span>.

   <span class="preview">![Más opciones de menú de la tarjeta de tipo de registro con Configuración](assets/more-menu-options-from-record-type-card-with-settings-link.png)</span>

1. En el cuadro **Editar tipo de registro**, la ficha **Apariencia** se abre de forma predeterminada. <!--update screen shot below at production-->

   ![Editar ficha de apariencia del cuadro de tipo de registro &#x200B;](assets/edit-record-type-box-appearance-tab.png)

   Actualice la siguiente información en la ficha **Apariencia**:

   * Edite el nombre del tipo de registro, si es necesario. <!--did they add a field label for this?-->
   * **Descripción**: edite o añada una descripción para el tipo de registro con más información al respecto.
   * Edite el color y la forma del icono asociado al tipo de registro. Haga lo siguiente:
      * Seleccione un color para identificar el tipo de registro. Es el color del icono de tipo de registro.
      * Seleccione un icono de la lista o empiece a escribir el nombre de un icono para describir lo que representa y, a continuación, selecciónelo cuando se muestre. Este es el icono del tipo de registro. De forma predeterminada, se selecciona un icono de archivo.

1. (Opcional y condicional) Si es administrador del sistema, haga clic en la pestaña **Configuración avanzada** <span class="preview">o **Configuración en todo el espacio de trabajo**</span> y actualice la información sobre las capacidades en todo el espacio de trabajo del tipo de registro.

   Para obtener más información, vea [Configurar las capacidades entre espacios de trabajo para los tipos de registro](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md). <!--update screen shot at production - Jan 2026-->

   ![Editar cuadro de tipo de registro con ficha de configuración avanzada](assets/edit-record-type-box-advanced-settings-tab.png)

1. Haga clic en **Guardar**.

   Si seleccionó conectar este registro desde otros espacios de trabajo, se mostrará el icono **Registro conectable** ![Conectarse desde otros espacios](assets/connect-from-other-workspaces-icon.png) en la tarjeta de registro.

   <span class="preview">Si ha seleccionado permitir la adición de este registro a otros espacios de trabajo, se muestra el icono **Registro global** ![Icono de tipo de registro global](assets/global-icon.png) en la tarjeta de registro. </span>

1. (Opcional) Haga clic en la tarjeta de tipo de registro del área de trabajo para abrir la página del tipo de registro y, a continuación, cambie el nombre del tipo de registro en el encabezado.

1. (Opcional) Para editar otro tipo de registro, en la página de tipo de registro, expanda la flecha hacia abajo a la derecha del nombre de un tipo de registro, busque un tipo de registro y selecciónelo cuando aparezca en la lista.

   ![Lista desplegable de tipo de registro en la página de tipo de registro con cuadro de búsqueda](assets/record-type-drop-down-on-record-type-page-with-search-box.png)
