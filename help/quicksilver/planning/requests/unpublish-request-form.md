---
title: Cancelar la publicación de un formulario de solicitud en Adobe Workfront Planning
description: Puede cancelar la publicación de un formulario de solicitud si ya no es necesario o relevante. Al cancelar la publicación, se eliminan los permisos de todos los usuarios para acceder al formulario.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: df8c4926-e258-49c0-ab9d-563ccaf7a6aa
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '863'
ht-degree: 26%

---

# Cancelar la publicación de un formulario de solicitud en Adobe Workfront Planning


<!--take Preview and Production references at Production time-->

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Puede cancelar la publicación de un formulario de solicitud si ya no es necesario o relevante. Al cancelar la publicación, se eliminan los permisos de todos los usuarios para acceder al formulario.

También puede cambiar las entidades con las que comparte un formulario de solicitud si desea que esté disponible para un grupo más pequeño de personas.

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
<p>Para obtener más información sobre qué se incluye en cada plan de Workfront Planning, póngase en contacto con su administrador de cuentas de Workfront. </td>

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
   <li><p>Administrar permisos para un espacio de trabajo <span class="preview">y tipo de registro</span> </p></li>
    <li><p>Los administradores del sistema pueden administrar los espacios de trabajo que no hayan creado. </p></li>
    </ul>
   <p>Para obtener información acerca de los permisos de uso compartido para objetos de Workfront Planning, consulte 
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Información general sobre los permisos de uso compartido en Adobe Workfront Planning</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>En el entorno de producción, todos los usuarios, incluidos los administradores del sistema, deben estar asignados a una plantilla de diseño que incluya Planning.</p>
<p><span class="preview">En el entorno de vista previa, los usuarios estándar y los administradores del sistema tienen Planning habilitado de forma predeterminada.</span></p>  
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

   Todas las solicitudes agregadas anteriormente permanecen en el área Solicitudes de Workfront, en la pestaña Planificación.
