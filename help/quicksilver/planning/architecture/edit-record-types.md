---
title: Editar tipos de registro
description: Puede editar los tipos de registro una vez guardados. Los tipos de registro son los tipos de objetos de Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: 1dc2791bed0dfada109ee102e09c25ae9a52e6b0
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 37%

---


# Editar tipos de registro

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

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
   <td>   <p>Administrar permisos para un espacio de trabajo <span class="preview">y tipo de registro</span> </p>  
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

<!--replace the layout template info in the table with this at release: 


<p>In the Production environment, all users including the System Administrators must be assigned to a layout template that includes the Planning areas.</p>
<p><span class="preview">In the Preview environment, Standard users and System Administrators have the Planning area enabled by default.</span></p>

-->

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

1. (Condicional) Si es administrador del sistema, haga clic en la ficha **Configuración avanzada** en el cuadro **Editar tipo de registro**. <!--the info here is duplicated in the Create record types article-->

   ![Ficha Editar configuración avanzada del cuadro de tipo de registro](assets/edit-record-type-box-advanced-settings-tab.png)

1. (Condicional) Actualice la siguiente información en la ficha **Configuración avanzada**:

   * Habilitar la configuración **Conectar desde otro espacio de trabajo**. Cuando está habilitado, el tipo de registro es accesible y se puede conectar desde otros espacios de trabajo.
   * Elija desde qué espacios de trabajo se puede acceder al tipo de registro. Elija entre las siguientes opciones:

      * **En todo el sistema**: los usuarios pueden conectarse a este tipo de registro desde todos los espacios de trabajo donde tengan permisos de administración.
      * **Espacios de trabajo específicos**: agregue los nombres de los espacios de trabajo a los que los administradores de espacios de trabajo pueden conectarse para este tipo de registro.

1. Haga clic en **Guardar**.

   La tarjeta de tipo de registro del área de trabajo muestra un icono de conectividad ![Conectar desde el icono de otras áreas de trabajo](assets/connect-from-other-workspaces-icon.png) en la esquina superior derecha para indicar que ahora se puede obtener acceso al registro desde otras áreas de trabajo.

1. (Opcional) Haga clic en la tarjeta de tipo de registro del área de trabajo para abrir la página del tipo de registro y, a continuación, cambie el nombre del tipo de registro en el encabezado.

1. (Opcional) Para editar otro tipo de registro, en la página de tipo de registro, expanda la flecha hacia abajo a la derecha del nombre de un tipo de registro, busque un tipo de registro y selecciónelo cuando aparezca en la lista.

   ![Lista desplegable de tipo de registro en la página de tipo de registro con cuadro de búsqueda](assets/record-type-drop-down-on-record-type-page-with-search-box.png)