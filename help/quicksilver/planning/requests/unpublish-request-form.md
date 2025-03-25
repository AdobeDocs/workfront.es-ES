---
title: Cancelar la publicación de un formulario de solicitud en Adobe Workfront Planning
description: Puede cancelar la publicación de un formulario de solicitud si ya no es necesario o relevante. Al cancelar la publicación, se eliminan los permisos de todos los usuarios para acceder al formulario.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: df8c4926-e258-49c0-ab9d-563ccaf7a6aa
source-git-commit: 15ddf6b4d82ccc694ec7a6c60d8e2d5b6b3645d6
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 33%

---

# Cancelar la publicación de un formulario de solicitud en Adobe Workfront Planning


<!--take Preview and Production references at Production time-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Puede cancelar la publicación de un formulario de solicitud si ya no es necesario o relevante. Al cancelar la publicación, se eliminan los permisos de todos los usuarios para acceder al formulario.

También puede cambiar las entidades con las que comparte un formulario de solicitud si desea que esté disponible para un grupo más pequeño de personas.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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
<p>Para obtener más información sobre qué se incluye en cada plan de Workfront Planning, póngase en contacto con su administrador de cuentas de Workfront. </td>

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
   <td>
   <p>Estándar</p>
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
   <td>
   <ul>
   <li><p>Administrar permisos en un área de trabajo <!--<span class="preview">and record type</span>--> </p></li>
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

## Modificación del uso compartido de un formulario de solicitud

Si comparte una solicitud de públicamente con todos, incluidos los usuarios de fuera de la organización, puede considerar la posibilidad de restringir este acceso a determinados usuarios que vean o administren el espacio de trabajo al que está asociado el formulario.

Para cambiar el uso compartido de un formulario de solicitud:

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo donde desee añadir registros.

   El espacio de trabajo se abre y los tipos de registro se muestran como tarjetas.

1. Haga clic en una tarjeta de tipo de registro. Para obtener información acerca de cómo crear un tipo de registro, consulte [Crear tipos de registros](/help/quicksilver/planning/architecture/create-record-types.md).

   La página de tipo de registro se abre en la vista a la que se accedió por última vez. De forma predeterminada, se abre una página de tipo de registro en la vista de tabla.

1. Haga clic en el menú **Más** ![Menú más](assets/more-menu.png) a la derecha del nombre del tipo de registro en el encabezado de la página y, a continuación, haga clic en **Actualizar formulario de solicitud**.
1. Haga clic en **Compartir** en la esquina superior derecha de la pantalla y, a continuación, actualice las opciones para compartir. Para obtener más información, consulte [Crear y administrar un formulario de solicitud en Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. (Opcional) Haga clic en **Copiar vínculo**, si ha cambiado el uso compartido del formulario de solicitud y desea compartirlo con el nuevo grupo de personas con un nuevo vínculo.

## Cancelar la publicación de un formulario de solicitud para un tipo de registro

Cuando un formulario de solicitud deja de ser relevante y ya no desea que nadie acceda a él, puede cancelar la publicación.

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo donde desee añadir registros.

   El espacio de trabajo se abre y los tipos de registro se muestran como tarjetas.

1. Haga clic en una tarjeta de tipo de registro. Para obtener información acerca de cómo crear un tipo de registro, consulte [Crear tipos de registros](/help/quicksilver/planning/architecture/create-record-types.md).

   La página de tipo de registro se abre en la vista a la que se accedió por última vez. De forma predeterminada, se abre una página de tipo de registro en la vista de tabla.

1. Haga clic en el menú **Más** ![Menú más](assets/more-menu.png) que se encuentra a la derecha del nombre del tipo de registro en el encabezado de la página y, a continuación, haga clic en **Actualizar formulario de solicitud**.
1. Haga clic en **Cancelar publicación** en la esquina superior derecha.

   ![Botón Cancelar publicación resaltado](assets/unpublish-button-highlighted.png)

   Aparece una confirmación en la parte inferior de la pantalla que le notifica que se ha cancelado la publicación del formulario.

   El botón **Cancelar publicación** cambia a **Publicar**.

1. Haga clic en **Guardar**.

   Ya no se puede obtener acceso al formulario desde un vínculo <!--or from the request queue in the Requests area of Workfront-->.

   Cualquier registro agregado anteriormente mediante el formulario de solicitud permanece en la página de tipo de registro.

   Todas las solicitudes agregadas anteriormente permanecen en el área Solicitudes de Workfront, en la pestaña Planificación.
