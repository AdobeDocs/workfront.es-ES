---
title: Creación de un formulario de solicitud en Adobe Workfront Planning
description: Después de seleccionar un tipo de registro en el área de Adobe Workfront Planning, puede crear un formulario de solicitud asociado a dicho tipo de registro y compartir un vínculo con otros usuarios internos o externos.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 1ad86cd55459d92650ac7a24c41765e579f8bb94
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 2%

---

# Creación de un formulario de solicitud en Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

Después de seleccionar un tipo de registro en el área de Adobe Workfront Planning, puede crear un formulario de solicitud y asociarlo a ese tipo de registro. A continuación, puede compartir un vínculo con otros usuarios internos o externos. <!--double-check on the external part of it-->

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener lo siguiente para poder acceder a Workfront Planning:

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
   <td role="rowheader"><p>plan Adobe Workfront*</p></td>
   <td>
<p>Cualquiera de los siguientes planes de Workfront:</p>
<ul><li>Seleccionar</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning no está disponible para planes Workfront heredados</p>
   </td>

<tr>
   <td role="rowheader"><p>Plan de planificación de Adobe Workfront*</p></td>
   <td>
<p>Cualquiera </p>   </td>

<tr>
   <td role="rowheader"><p>plataforma de Adobe Workfront</p></td>
   <td>
<p>La instancia de Workfront de su organización debe incorporarse a la experiencia Adobe unificado para poder acceder a todas las funcionalidades de Workfront Planning.</p>
<p>Para obtener más información, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiencia unificada de Adobe para Workfront</a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Licencia de Adobe Workfront*</p></td>
   <td>
   <p>Estándar</p>
   <p>Workfront Planning no está disponible para licencias de Workfront heredadas</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Configuración del nivel de acceso</p></td>
   <td> <p>No hay controles de nivel de acceso para Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permisos de objeto</p></td>
   <td>
   <ul>
   <li><p>Administración de permisos en un espacio de trabajo</p></li>
    <li><p>Los administradores del sistema pueden administrar los espacios de trabajo que no hayan creado. </p></li>
    </ul>
   <p>Para obtener información acerca de los permisos de uso compartido para objetos de Workfront Planning, consulte  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Información general sobre los permisos de uso compartido en Adobe Workfront Planning</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>A todos los usuarios, incluidos los administradores de Workfront, se les debe asignar una plantilla de diseño que incluya el área de Planning en el menú principal. </p>  
</td>
  </tr>
 </tbody>
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creación de un formulario de solicitud para un tipo de registro

{{step1-to-planning}}

1. Haga clic en el área de trabajo donde desee agregar registros.

   El espacio de trabajo se abre y los tipos de registro se muestran como tarjetas.

1. Haga clic en una tarjeta de tipo de registro. Para obtener información acerca de cómo crear un tipo de registro, vea [Crear tipos de registros](/help/quicksilver/planning/architecture/create-record-types.md).

   La página de tipo de registro se abre en la vista a la que se accedió por última vez. De forma predeterminada, se abre una página de tipo de registro en la vista de tabla.

1. Haga clic en el menú **Más** ![](assets/more-menu.png) a la derecha del nombre del tipo de registro en el encabezado de la página y, a continuación, haga clic en **Crear formulario de solicitud**.
1. Actualice el nombre del formulario de solicitud. De manera predeterminada, el nombre del formulario es **Formulario de solicitud sin título**. <!--check this; you logged a bug to rename it to this but was it fixed?-->
1. (Opcional) Agregue una **Descripción** para el formulario de solicitud.

   <!--Not possible yet: The Description is visible when you access the request form from the Requests area of Workfront.-->

1. Haga clic en **Crear**. Se abrirá el formulario de solicitud del tipo de registro seleccionado.

   El formulario de solicitud contiene la siguiente información de forma predeterminada:

   * **Sección predeterminada**: Este es el salto de sección predeterminado que Workfront aplica al formulario de solicitud. No se puede cambiar el nombre de la sección predeterminada ni eliminarla.
   * Campo **Asunto**: Campo que identificará la solicitud en Workfront. Esta capacidad aún no está disponible.
   * Todos los campos asociados al tipo de registro.

   Los campos contenidos en el formulario de solicitud serán visibles para todos los que envíen una solicitud a este tipo de registro.

1. (Opcional) Elimine el campo **Asunto**, ya que esto no es visible en Workfront Planning. <!--remove this step when we connect intake with the Requests area in Workfront-->
1. Pase el ratón sobre cualquier campo del formulario que quiera eliminar. Se agregarán a la ficha **Campos** en la parte izquierda del formulario.
1. Haga clic en cualquier campo y, a continuación, utilice los controles situados en el lado derecho del formulario para definir cualquiera de la siguiente información sobre los campos:

   * **Etiqueta**: este es el nombre del campo tal como aparecerá en el formulario de solicitud. Esto no cambia el nombre del campo de registro.
   * **Instrucciones**: Agregue más información sobre el campo.
   * **Crear un campo obligatorio**: cuando se selecciona, el campo debe tener un valor. De lo contrario, el formulario no se podrá enviar.
   * **Agregar lógica**: defina qué condiciones deben cumplirse para que el campo se muestre o se oculte.

1. Haga clic en la pestaña Elementos de contenido, en la parte derecha del formulario, y añada cualquiera de los siguientes elementos:

   * Texto descriptivo
   * Salto de sección

   Para obtener más información acerca de cómo crear un formulario personalizado, vea [Diseñar un formulario con el diseñador de formularios](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).





