---
title: Editar tipos de registro
description: Puede editar los tipos de registro una vez guardados. Los tipos de registro son los tipos de objetos de Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: 609396b2eb6413c8f6e84361757f00c2cc5e3ad6
workflow-type: tm+mt
source-wordcount: '714'
ht-degree: 40%

---


# Editar tipos de registro

{{planning-important-intro}}

Los tipos de registro son los tipos de objetos de Adobe Workfront Planning. Puede editar el aspecto de los tipos de registro que usted o cualquier otra persona hayan creado. Para obtener información sobre cómo crear tipos de registro de Workfront Planning, consulte [Crear tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md).

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
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>
   <p>Solo los administradores del sistema pueden habilitar tipos de registros para conectarse desde otros espacios de trabajo</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Plantilla de diseño</p></td> 
   <td> <p>A todos los usuarios, incluidos los administradores de Workfront, se les debe asignar una plantilla de diseño que incluya el área de Planning en el menú principal. </p> </td> 
  </tr> 
</tbody> 
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
OLD:

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
   <p> Adobe Workfront</p> <p>To connect Adobe Workfront Planning record types with Experience Manager Assets, you must have an Adobe Experience Manager Assets license and your organization's instance of Workfront must be onboarded to the Adobe Business Platform or the Adobe Admin Console.</p> </td>
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
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access level controls for Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Only system administrators can enable record types to connect from other workspaces</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).-->

## Editar tipos de registro

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo cuyos tipos de registro desee editar.

   Se abre la página del espacio de trabajo y se muestran los tipos de registro.
1. Realice una de las siguientes acciones:

   * Pase el ratón sobre la tarjeta de un tipo de registro y haga clic en el menú **Más** ![Menú más](assets/more-menu.png) en la esquina superior derecha de la tarjeta de tipo de registro; a continuación, haga clic en **Editar**
O
   * Haga clic en una tarjeta de tipo de registro para abrir la página de tipo de registro, haga clic en el menú **Más** ![Menú Más](assets/more-menu.png) a la derecha del nombre del tipo de registro y, a continuación, haga clic en **Editar**.

   ![Más opciones de menú de la tarjeta de tipo de registro](assets/more-menu-options-from-record-type-card.png)

1. En el cuadro **Editar tipo de registro**, la ficha **Apariencia** se abre de forma predeterminada.

   ![Editar ficha de apariencia del cuadro de tipo de registro ](assets/edit-record-type-box-appearance-tab.png)

   Actualice la siguiente información en la ficha **Apariencia**:

   * Edite el nombre del tipo de registro, si es necesario. <!--did they add a field label for this?-->
   * **Descripción**: edite o añada una descripción para el tipo de registro con más información al respecto.
   * Edite el color y la forma del icono asociado al tipo de registro. Haga lo siguiente:
      * Seleccione un color para identificar el tipo de registro. Es el color del icono de tipo de registro.
      * Seleccione un icono de la lista o empiece a escribir el nombre de un icono para describir lo que representa y, a continuación, selecciónelo cuando se muestre. Este es el icono del tipo de registro. De forma predeterminada, se selecciona un icono de archivo.

1. (Condicional) Si es administrador del sistema, haga clic en la ficha **Configuración avanzada** en el cuadro **Editar tipo de registro**.

   ![Ficha Editar configuración avanzada del cuadro de tipo de registro](assets/edit-record-type-box-advanced-settings-tab.png)

1. (Condicional) Como administrador del sistema, actualice la siguiente información en la ficha **Configuración avanzada**:

   * **Conectar desde otros espacios de trabajo**: seleccione esta opción para permitir que los usuarios se conecten a este tipo de registro desde otros espacios de trabajo. Esta opción está desactivada de forma predeterminada.
   * **En todo el sistema**: seleccione esta opción para permitir que los usuarios se conecten a este registro desde todos los espacios de trabajo del sistema.
   * **Espacios de trabajo específicos**: seleccione esta opción para restringir los espacios de trabajo desde los cuales los usuarios pueden conectarse a este tipo de registro; a continuación, expanda el menú desplegable y seleccione los espacios de trabajo desde los que desea que los usuarios se conecten a este tipo de registro. Puede empezar a escribir el nombre de un espacio de trabajo y seleccionarlo cuando se muestre en la lista.

1. Haga clic en **Guardar**.

   La tarjeta de tipo de registro del área de trabajo muestra un icono de conectividad ![Conectar desde el icono de otras áreas de trabajo](assets/connect-from-other-workspaces-icon.png) en la esquina superior derecha para indicar que ahora se puede obtener acceso al registro desde otras áreas de trabajo.

1. (Opcional) Haga clic en la tarjeta de tipo de registro del área de trabajo para abrir la página del tipo de registro y, a continuación, cambie el nombre del tipo de registro en el encabezado.

1. (Opcional) Para editar otro tipo de registro, en la página de tipo de registro, expanda la flecha hacia abajo a la derecha del nombre de un tipo de registro, busque un tipo de registro y selecciónelo cuando aparezca en la lista.

   ![Lista desplegable de tipo de registro en la página de tipo de registro con cuadro de búsqueda](assets/record-type-drop-down-on-record-type-page-with-search-box.png)