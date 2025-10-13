---
title: Editar tipos de registro
description: Puede editar los tipos de registro una vez guardados. Los tipos de registro son los tipos de objetos de Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: 393f858ba3711b367cf06ad846ea60be0d6d9034
workflow-type: tm+mt
source-wordcount: '692'
ht-degree: 33%

---


# Editar tipos de registro

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Los tipos de registro son los tipos de objetos de Adobe Workfront Planning. Puede editar el aspecto de los tipos de registro que usted o cualquier otra persona hayan creado. Para obtener información sobre cómo crear tipos de registro de Workfront Planning, consulte [Crear tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md).

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
   <td>   <p>Administración de permisos de un espacio de trabajo y tipo de registro </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>
   <p>Solo los administradores del sistema pueden habilitar tipos de registros para conectarse desde otros espacios de trabajo</p> </td> 
  </tr>

</tbody> 
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Editar tipos de registro

{{step1-to-planning}}

1. Haga clic en el área de trabajo cuyos tipos de registro desee editar.

   Se abre la página del espacio de trabajo y se muestran los tipos de registro.
1. Realice una de las siguientes acciones:

   * Pase el ratón sobre la tarjeta de un tipo de registro y haga clic en el menú **Más** ![Menú más](assets/more-menu.png) en la esquina superior derecha de la tarjeta de tipo de registro; a continuación, haga clic en **Editar**
O
   * <span class="preview">Haga clic en una tarjeta de tipo de registro para abrir la página de tipo de registro, haga clic en el menú **Más** ![Menú Más](assets/more-menu.png) a la derecha del nombre del tipo de registro y, a continuación, haga clic en **Editar**. </span>

   <span class="preview">![Más opciones de menú de la tarjeta de tipo de registro](assets/more-menu-options-from-record-type-card.png)</span>

1. En el cuadro **Editar tipo de registro**, la ficha **Apariencia** se abre de forma predeterminada.

   ![Editar ficha de apariencia del cuadro de tipo de registro ](assets/edit-record-type-box-appearance-tab.png)

   Actualice la siguiente información en la ficha **Apariencia**:

   * Edite el nombre del tipo de registro, si es necesario. <!--did they add a field label for this?-->
   * **Descripción**: edite o añada una descripción para el tipo de registro con más información al respecto.
   * Edite el color y la forma del icono asociado al tipo de registro. Haga lo siguiente:
      * Seleccione un color para identificar el tipo de registro. Es el color del icono de tipo de registro.
      * Seleccione un icono de la lista o empiece a escribir el nombre de un icono para describir lo que representa y, a continuación, selecciónelo cuando se muestre. Este es el icono del tipo de registro. De forma predeterminada, se selecciona un icono de archivo.

   <!--old info: 
   1. (Conditional) If you are a system administrator, click the **Advanced settings** tab in the **Edit record type** box. 
      ![Edit record type box advanced settings tab](assets/edit-record-type-box-advanced-settings-tab.png)
   1. (Conditional) Update the following information in the **Advanced settings** tab: 
      * Enable the **Connect from other workspace** setting. When enabled, the record type is accessible and can be connected from other workspaces. 
      * Choose from which workspaces the record type can be accessed. Choose from the following options:
         * **System wide**: Users can connect to this record type from all workspaces where they have manage permissions. 
         * **Specific workspaces**: Add the names of the workspaces where workspace managers can connect to this record type.-->


1. (Opcional y condicional) Si es administrador del sistema, haga clic en **Configuración avanzada** y actualice la siguiente información en la sección **Capacidad entre espacios de trabajo**: <!--take this info out and replace it with a link to this article: help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md-->
   * Habilitar la configuración **Permitir la conexión a este tipo de registro en otros espacios de trabajo**: permite a los administradores de espacios de trabajo conectarse a este tipo de registro desde otros espacios de trabajo.\
     Puede designar desde qué espacios de trabajo se puede conectar este tipo de registro. Puede ponerlo a disposición de todos los espacios de trabajo o designar espacios específicos donde pueda importarlo.
Para obtener más información, vea [Configurar las capacidades entre espacios de trabajo para los tipos de registro](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

   ![Ficha Editar configuración avanzada del cuadro de tipo de registro](assets/edit-record-type-box-advanced-settings-tab.png)

   <!--replace last point with this when we release dynamic record types:
      1. (Optional and conditional) If you are a system administrator, click **Advanced settings** and update the following information in the **Cross-workspace capability** section: **** the info here is duplicated in the Edit record types article ***
         * Enable the **Allow adding this record type to other workspaces** setting: This allows workspace managers to add this record type to other workspaces. 
               You can designate specific users who can add this record type to other workspaces. 
         * Enable the **Allow connecting to this record type in other workspaces** setting: This allows workspace managers to connect to this record type from other workspaces.  
               You can designate which workspaces this record type can be connected from. You can make it available for all workspaces or designate specific ones where you can import it.
         For more information, see [Configure cross-workspace capabilities for record types](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).  
         ******** replace screen shot below **********
         ![Create record type box on advanced settings tab](assets/create-record-type-box-advanced-settings-tab.png) 
      -->

1. Haga clic en **Guardar**.

   La tarjeta de tipo de registro del área de trabajo muestra un icono de conectividad ![Conectar desde el icono de otras áreas de trabajo](assets/connect-from-other-workspaces-icon.png) en la esquina superior derecha para indicar que ahora se puede obtener acceso al registro desde otras áreas de trabajo.

1. (Opcional) Haga clic en la tarjeta de tipo de registro del área de trabajo para abrir la página del tipo de registro y, a continuación, cambie el nombre del tipo de registro en el encabezado.

1. (Opcional) Para editar otro tipo de registro, en la página de tipo de registro, expanda la flecha hacia abajo a la derecha del nombre de un tipo de registro, busque un tipo de registro y selecciónelo cuando aparezca en la lista.

   ![Lista desplegable de tipo de registro en la página de tipo de registro con cuadro de búsqueda](assets/record-type-drop-down-on-record-type-page-with-search-box.png)
