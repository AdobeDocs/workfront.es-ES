---
title: Cancelar la publicación de un formulario de solicitud en Adobe Workfront Planning
description: Puede cancelar la publicación de un formulario de solicitud si ya no es necesario o relevante. Al cancelar la publicación, se eliminan los permisos de todos los usuarios para acceder al formulario.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: df8c4926-e258-49c0-ab9d-563ccaf7a6aa
source-git-commit: 66d59467e7e9857ca5573b819d51da839ddbd4f7
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 21%

---

# Cancelar la publicación de un formulario de solicitud en Adobe Workfront Planning


<!--take Preview and Production references at Production time-->

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

-->

{{planning-important-intro}}

Puede cancelar la publicación de un formulario de solicitud si ya no es necesario o relevante. Al cancelar la publicación, se eliminan los permisos de todos los usuarios para acceder al formulario.

También puede cambiar las entidades con las que comparte un formulario de solicitud si desea que esté disponible para un grupo más pequeño de personas.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Paquetes de Adobe Workfront</p></td> 
   <td> 
<p>Cualquier paquete Workfront y cualquier paquete Planning</p>
O
<p>Cualquier paquete de flujo de trabajo y cualquier paquete de Planning</p>
<p>Para obtener más información sobre lo que se incluye en cada paquete de Workfront Planning, póngase en contacto con su representante de cuentas de Workfront.</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Estándar</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Administrar permisos a un espacio de trabajo y tipo de registro</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modificación del uso compartido de un formulario de solicitud

Si comparte una solicitud de públicamente con todos, incluidos los usuarios de fuera de la organización, puede considerar la posibilidad de restringir este acceso a determinados usuarios que vean o administren el espacio de trabajo al que está asociado el formulario.

Para cambiar el uso compartido de un formulario de solicitud:

{{step1-to-planning}}

1. Haga clic en el área de trabajo donde desee compartir un formulario.

   El espacio de trabajo se abre y los tipos de registro se muestran como tarjetas.

1. Haga clic en una tarjeta de tipo de registro. Para obtener información acerca de cómo crear un tipo de registro, consulte [Crear tipos de registros](/help/quicksilver/planning/architecture/create-record-types.md).

   La página de tipo de registro se abre en la vista a la que se accedió por última vez. De forma predeterminada, se abre una página de tipo de registro en la vista de tabla.

1. Haga clic en el menú **Más** ![Menú más](assets/more-menu.png) que se encuentra a la derecha del nombre del tipo de registro en el encabezado de la página y, a continuación, haga clic en **Administrar formularios de solicitud**.

   Todos los formularios de solicitud asociados al tipo de registro se muestran en una vista de tabla.
1. Pase el ratón sobre el nombre de un formulario de solicitud, luego haga clic en el menú **Más** ![Menú más](assets/more-menu.png) a la derecha de su nombre y luego haga clic en **Compartir**.
1. Actualice las opciones de uso compartido seleccionando una de las siguientes opciones:

   * Cualquiera con acceso de visualización o más alto al espacio de trabajo
   * Cualquiera con acceso de aportación o más alto al espacio de trabajo
   * Cualquiera con el vínculo

   Para obtener más información, consulte [Crear y administrar un formulario de solicitud en Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. (Opcional) Haga clic en **Copiar vínculo**, si ha cambiado el uso compartido del formulario de solicitud y desea compartirlo con el nuevo grupo de personas con un nuevo vínculo.

## Cancelar la publicación de un formulario de solicitud para un tipo de registro

Cuando un formulario de solicitud deja de ser relevante y ya no desea que nadie acceda a él, puede cancelar la publicación.

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo donde desee añadir registros.

   El espacio de trabajo se abre y los tipos de registro se muestran como tarjetas.

1. Haga clic en una tarjeta de tipo de registro. Para obtener información acerca de cómo crear un tipo de registro, consulte [Crear tipos de registros](/help/quicksilver/planning/architecture/create-record-types.md).

   La página de tipo de registro se abre en la vista a la que se accedió por última vez. De forma predeterminada, se abre una página de tipo de registro en la vista de tabla.

1. Haga clic en el menú **Más** ![Menú más](assets/more-menu.png) que se encuentra a la derecha del nombre del tipo de registro en el encabezado de la página y, a continuación, haga clic en **Administrar formularios de solicitud**.

   Todos los formularios de solicitud asociados al tipo de registro se muestran en una vista de tabla.
1. Pase el ratón sobre el nombre de un formulario de solicitud, luego haga clic en el menú **Más** ![Menú más](assets/more-menu.png) a la derecha de su nombre y luego haga clic en **Cancelar publicación**

O

Haga clic en el nombre del formulario de solicitud para abrirlo y luego haga clic en **Cancelar la publicación** en la esquina superior derecha del formulario de solicitud.

![Botón Cancelar publicación resaltado](assets/unpublish-button-highlighted.png)

Aparece una confirmación en la parte inferior de la pantalla que le notifica que se ha cancelado la publicación del formulario.

El vínculo o botón **Cancelar la publicación** cambia a **Publicar**.

1. (Condicional) Haga clic en **Guardar** si canceló la publicación del formulario después de abrirlo.

   Los usuarios ya no pueden acceder al formulario de solicitud desde un vínculo o desde la cola de solicitudes del área de Solicitudes de Workfront.

   Cualquier registro agregado anteriormente mediante el formulario de solicitud permanece en la página de tipo de registro.

   Todas las solicitudes agregadas anteriormente permanecen en el área Solicitudes de Workfront.
