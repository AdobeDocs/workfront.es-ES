---
title: Editar tipos de registros
description: Puede editar los tipos de registro una vez guardados. Los tipos de registro son los tipos de objetos de Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: ded6db27fa3fba9195e2133134f60bcadb0f897a
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 1%

---

<!--update the metadata with real information when making this available in TOC and in the left nav
---
title: Edit record types
description: You can edit record types after they have been saved. Record types are the object types of Adobe Workfront Planning.
author: Alina
role: User
feature: Work Management 
topic: Architecture
hidefromtoc: yes
hide: yes
---

-->

# Editar tipos de registros

{{planning-important-intro}}

Los tipos de registro son los tipos de objetos de Adobe Workfront Planning. Puede editar el aspecto de los tipos de registro que usted o cualquier otra persona hayan creado. Para obtener información acerca de cómo crear tipos de registros de Workfront Planning, vea [Crear tipos de registros](/help/quicksilver/planning/architecture/create-record-types.md).

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso para Workfront Planning.

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
   <p> Adobe Workfront</p> <p>Para conectar los tipos de registros de Adobe Workfront Planning con Experience Manager Assets, debe tener una licencia de Adobe Experience Manager Assets y la instancia de Workfront de su organización debe estar integrada en Adobe Business Platform o Adobe Admin Console.</p> </td>
  </tr>  
 <td role="rowheader"><p>acuerdo con Adobe Workfront</p></td>
   <td>
<p>Su organización debe estar inscrita en la fase de acceso anticipado para Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>plan de Adobe Workfront</p></td>
   <td>
<p>Cualquiera</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licencia de Adobe Workfront*</p></td>
   <td>
   <p>Nuevo: estándar</p>
   <p>Actual: plan</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuraciones de nivel de acceso</p></td>
   <td> <p>No hay controles de nivel de acceso para Workfront Planning</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Permisos</p></td>
   <td> <p>Administrar permisos en un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>
   <p>Solo los administradores del sistema pueden habilitar tipos de registros para conectarse desde otros espacios de trabajo</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>El administrador del grupo o de Workfront debe agregar el área de Planning a la plantilla de diseño. Para obtener más información, consulte <a href="/help/quicksilver/planning/access/access-overview.md">Resumen de acceso</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Editar tipos de registros

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo cuyos tipos de registros desee editar.

   Se abre la página del espacio de trabajo y se muestran los tipos de registro.
1. Realice una de las siguientes acciones:

   * Pase el ratón sobre la tarjeta de un tipo de registro y haga clic en el menú **Más** ![](assets/more-menu.png) en la esquina superior derecha de la tarjeta del tipo de registro; a continuación, haga clic en **Editar**
O
   * Haga clic en una tarjeta de tipo de registro para abrir la página de tipo de registro, haga clic en el menú **Más** ![](assets/more-menu.png) a la derecha del nombre del tipo de registro y, a continuación, haga clic en **Editar**.

   ![](assets/more-menu-options-from-record-type-card.png)

1. En el cuadro **Editar tipo de registro**, la ficha **Apariencia** se abre de forma predeterminada.

   ![](assets/edit-record-type-box-appearance-tab.png)

   Actualice la siguiente información en la ficha **Apariencia**:

   * Edite el nombre del tipo de registro si es necesario. <!--did they add a field label for this?-->
   * **Descripción**: edite o agregue una descripción para el tipo de registro con más información al respecto.
   * Edite el color y la forma del icono asociado al tipo de registro. Haga lo siguiente:
      * Seleccione un color para identificar el tipo de registro. Es el color del icono de tipo de registro.
      * Seleccione un icono de la lista o empiece a escribir el nombre de un icono para describir lo que representa y, a continuación, selecciónelo cuando se muestre. Este es el icono del tipo de registro. De forma predeterminada, se selecciona un icono de archivo.

1. (Condicional) Si es administrador del sistema, haga clic en la ficha **Configuración avanzada** en el cuadro **Editar tipo de registro**.

   ![](assets/edit-record-type-box-advanced-settings-tab.png)

1. (Condicional) Como administrador del sistema, actualice la siguiente información en la ficha **Configuración avanzada**:

   * **Conectar desde otros espacios de trabajo**: seleccione esta opción para permitir que los usuarios se conecten a este tipo de registro desde otros espacios de trabajo. De forma predeterminada, esta opción no está seleccionada.
   * **En todo el sistema**: seleccione esta opción para permitir que los usuarios se conecten a este registro desde todos los espacios de trabajo del sistema.
   * **Espacios de trabajo específicos**: seleccione esta opción para restringir los espacios de trabajo desde los cuales los usuarios pueden conectarse a este tipo de registro; a continuación, expanda el menú desplegable y seleccione los espacios de trabajo desde los que desea que los usuarios se conecten a este tipo de registro. Puede empezar a escribir el nombre de un espacio de trabajo y seleccionarlo cuando se muestre en la lista.

1. Haga clic en **Guardar**.

   La tarjeta de tipo de registro del área de trabajo muestra un icono de conectividad ![](assets/connect-from-other-workspaces-icon.png) en la esquina superior derecha para indicar que ahora se puede obtener acceso al registro desde otras áreas de trabajo.

1. (Opcional) Haga clic en la tarjeta de tipo de registro del área de trabajo para abrir la página del tipo de registro y, a continuación, cambie el nombre del tipo de registro en el encabezado.

1. (Opcional) Para editar otro tipo de registro, en la página de tipo de registro, expanda la flecha hacia abajo a la derecha del nombre de un tipo de registro, busque un tipo de registro y selecciónelo cuando aparezca en la lista.

   ![](assets/record-type-drop-down-on-record-type-page-with-search-box.png)