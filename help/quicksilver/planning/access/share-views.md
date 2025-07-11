---
title: Compartir vistas
description: Puede compartir una vista con otros usuarios para garantizar la colaboración cuando se utiliza Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 673dd888-3135-48b0-8198-c8d6d6706ddf
source-git-commit: d3d4a923dddb8685a981162918f34447300136cf
workflow-type: tm+mt
source-wordcount: '1969'
ht-degree: 44%

---


# Compartir vistas

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Puede compartir una vista con otros usuarios para garantizar la colaboración cuando se trabaja con registros en Adobe Workfront Planning.

>[!IMPORTANT]
>
>* La concesión de permisos a un espacio de trabajo no significa que se conceden permisos a otros usuarios para ver las páginas de tipo de registro. Es preciso conceder permisos a las vistas individuales de una página de tipo de registro para compartirlas con otros usuarios.
>
>* La concesión de permisos a una vista no cambia los permisos de visualización de los registros. Los permisos de registro se conceden al compartir espacios de trabajo.
>
>* Cuando comparte una vista, concede permisos a otros usuarios para que accedan a todos los elementos de la vista. Por ejemplo, cuando les concede permisos de administración para una vista, pueden modificar su agrupación, filtro, ordenación o apariencia de barra.


<!--
This article describes how you can share a view with others. For information about requesting, granting, or denying permissions to a view, see [Request permissions to a view or a workspace](/help/quicksilver/planning/access/request-permissions.md). -->

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso.

<!--at GA, check that the Workfront plans article linked below has Planning info-->

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
<p>La instancia de Workfront de su organización debe incorporarse a Adobe Unified Experience para poder acceder a Workfront Planning.</p> 
<p>Su organización debe incorporarse a la experiencia unificada de Adobe para que los usuarios puedan solicitar y conceder permisos a una vista desde una solicitud de permiso. </p>
<p>Los usuarios deben agregarse a Adobe Admin Console para obtener permisos en las vistas de Workfront Planning.</p>
<p>Para obtener más información, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience para Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront*</p></td> 
   <td><p> Estándar</p>
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
   <td>  <p>Permisos de administración de una vista</p>  
   <p>Solo los usuarios con permisos de Administración para un espacio de trabajo pueden compartir una vista públicamente.</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Plantilla de diseño</p></td> 
   <td> <p>En el entorno de producción, todos los usuarios, incluidos los administradores del sistema, deben estar asignados a una plantilla de diseño que incluya las áreas de planificación.</p>
<p><span class="preview">En el entorno de vista previa, los usuarios estándar y los administradores del sistema tienen activada de forma predeterminada el área de Planning.</span></p></td> 
  </tr> 
</tbody> 
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones al compartir vistas

* Puede compartir una vista de las siguientes maneras:

   * Internamente, con usuarios, grupos, equipos, empresas y funciones de Workfront
   * Públicamente, con usuarios de fuera de Workfront
   * Al copiar y luego compartir un vínculo a una vista
   * Exportándolo a un archivo de Excel o CSV. Sólo se puede exportar la vista de tabla a un archivo. Para obtener más información, consulte [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md).

* Para obtener información general sobre cómo compartir objetos en Workfront Planning, consulte también [Información general sobre los permisos de uso compartido en Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).
* Puede conceder permisos de visualización o administración para una vista a usuarios internos de Workfront.

* Los usuarios con permisos de administración pueden modificar la configuración de vista, compartirla, duplicarla o eliminarla.

* Puede compartir vistas con personas de fuera de su organización mediante un vínculo público.

* Cuando comparte una vista públicamente, cualquier persona de fuera de la compañía puede acceder al vínculo durante un tiempo limitado, como lo indica su fecha de caducidad. No se requiere iniciar sesión para ver la vista compartida.

* Las personas de fuera de la organización que tienen acceso a una vista no pueden crear otras vistas, editar la vista compartida ni añadir, eliminar o editar la información de registro de la vista.

## Compartir permisos para una vista internamente

Puede compartir las vistas que ha creado o las vistas en las que tiene permiso de administración con usuarios, grupos, equipos, empresas y roles en Workfront Planning.

>[!NOTE]
>
>Los administradores del sistema no pueden ver ni compartir vistas que no hayan creado ellos mismos. Solo pueden acceder o compartir las vistas que se han compartido con ellos.
>
>Los administradores del sistema solo pueden tener permisos de administración para una vista.

{{step1-to-planning}}

1. Abra el espacio de trabajo cuya vista desee compartir y, a continuación, haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.

1. En la ficha Ver, <span class="preview">realice una de las siguientes acciones:</span>

   * Pase el ratón sobre el nombre de la ficha de la vista que quiera compartir y haga clic en el menú **Más** ![Menú más](assets/more-menu.png) que se encuentra a la derecha del nombre de la vista; a continuación, haga clic en **Compartir**.

     ![Menú más para una vista](assets/more-menu-for-views-expanded-with-share-option.png)

   * <span class="preview">Haga clic en **Compartir** > **Compartir la vista actual**</span>

     <span class="preview">![Botón Compartir con tipo de registro y ver opciones de uso compartido](assets/share-button-with-record-type-and-view-sharing-options.png)</span>

   Se abre el cuadro **Compartir vista** y la ficha **Uso compartido interno** debe estar seleccionada de forma predeterminada.

1. (Opcional) En el área **Quién tiene acceso**, seleccione una de las siguientes opciones:

   * **Solo las personas invitadas pueden tener acceso**: debe especificar los usuarios, grupos, equipos, empresas o roles con los que desea compartir la vista. Esta es la opción predeterminada.

     >[!NOTE]
     >
     >   Además de los equipos, grupos, empresas y funciones del puesto, solo puede compartir con los usuarios que se han añadido a Adobe Admin Console.


   * **Todos los usuarios del espacio de trabajo pueden ver**: todos los usuarios que tengan permisos de visualización o superiores en los espacios de trabajo pueden acceder a la vista.

1. En el campo **Conceder acceso a esta vista**, empiece a escribir el nombre de un usuario, un grupo, un equipo, una empresa o un rol y, a continuación, haga clic en él cuando se muestre en la lista.

   ![Compartir una vista con grupos](assets/sharing-a-view-ui-with-groups.png)

1. Seleccione uno de los siguientes niveles de permisos en el menú desplegable:
   * Ver
   * Administrar

     Para obtener información acerca de los niveles de permisos y las acciones que los usuarios pueden realizar en cada nivel, consulte [Información general sobre los permisos de uso compartido en Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

     Los administradores del sistema siempre reciben permisos de administración para las vistas compartidas con ellos.

1. Haga clic en **Guardar**.

   La vista se actualiza con un icono de personas ![Vista compartida con otros iconos](assets/view-shared-with-others-people-icon.png) para indicar que la vista ahora se comparte con otros usuarios.

   Los usuarios con los que compartió la vista reciben una notificación dentro de la aplicación y por correo electrónico sobre si tienen permisos para ella.

   >[!TIP]
   >
   >Las vistas sin un icono de personas o global son vistas que ha creado y no se comparten con otros. Las vistas no compartidas solo son visibles para usted.

1. Comparta el vínculo copiado con otros usuarios. Los usuarios que reciban el vínculo deben ser usuarios activos e iniciar sesión en Workfront para poder acceder a la página de tipo de registro y mostrarla en la vista seleccionada.

## Compartir permisos para una vista públicamente

Puede compartir las vistas que ha creado o las vistas para las que tiene permisos de administración con personas que no tienen una licencia de Workfront y que pueden ser ajenas a su organización.

>[!IMPORTANT]
>
>Solo los usuarios con permisos de administración para un espacio de trabajo pueden compartir las vistas del espacio de trabajo públicamente.


Para compartir una vista públicamente en Workfront Planning:

{{step1-to-planning}}

1. Abra el espacio de trabajo cuya vista desee compartir y, a continuación, haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.

1. En la pestaña Ver, realice una de las siguientes acciones:

   * Pase el ratón sobre el nombre de la ficha de la vista que quiera compartir y haga clic en el menú **Más** ![Menú más](assets/more-menu.png) que se encuentra a la derecha del nombre de la vista; a continuación, haga clic en **Compartir**.

   ![Menú más para vistas expandido con la opción de uso compartido](assets/more-menu-for-views-expanded-with-share-option.png)
   * <span class="preview">Haga clic en **Compartir** > **Compartir la vista actual**</span>

   Se abre el cuadro **Compartir vista**.

1. Haga clic en **Uso compartido público**.

   ![Ficha de uso compartido público para vistas](assets/public-sharing-tab-for-views.png)

1. Habilitar la configuración **Crear vínculo público**.

   Aparecerá un vínculo disponible. Este es un vínculo público. Cuando se comparte, cualquier persona que tenga el vínculo, incluidas las personas de fuera de la organización, puede acceder a la página de tipo de registro y ver los registros y campos de la página.

1. Haga clic en el icono **Copiar vínculo** ![Copiar vista de vínculo](assets/copy-link-view.png) para copiar el vínculo en el portapapeles.

1. Introduzca una fecha manualmente o use el calendario del campo **Fecha de caducidad del vínculo** para seleccionar una fecha de caducidad para el vínculo público. No se podrá acceder a la vista de página del registro después de la fecha seleccionada.

1. Haga clic en **Guardar**.

   La vista se actualiza con un icono global ![Icono de vista compartida pública resaltado](assets/public-shared-view-icon-highlighted.png) para indicar que la vista se comparte públicamente.

   >[!TIP]
   >
   >Las vistas sin un icono de personas o global son vistas que ha creado y no se comparten con otros. Las vistas no compartidas solo son visibles para usted.


1. (Opcional) Pegue el vínculo que ha copiado en un correo electrónico, mensaje de chat, documento o comentario de Workfront para compartirlo con otros usuarios.

## Copia de un vínculo a una vista

Puede copiar un vínculo a una vista en el portapapeles e incluirlo en otra aplicación o compartirlo con otros usuarios.

Para copiar un vínculo a una vista compartida públicamente, consulte la sección [Compartir permisos en una vista compartida públicamente](#share-permissions-to-a-view-publicly) en este artículo.

Esta sección describe cómo compartir una vista internamente.

>[!IMPORTANT]
>
>En primer lugar, debe compartir la vista con los usuarios antes de compartir el vínculo a la vista para que puedan verlo.


{{step1-to-planning}}

1. Abra el espacio de trabajo cuya vista desee copiar y compartir el vínculo y, a continuación, haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.

1. En la pestaña de una vista, realice una de las siguientes acciones:

   * Pase el ratón sobre la pestaña de la vista que quiera compartir y haga clic en el menú **Más** ![Menú más](assets/more-menu.png) a la derecha del nombre de la vista, luego haga clic en **Compartir** > **Copiar vínculo** en el cuadro **Compartir vista**.
   * <span class="preview">Haga clic en **Compartir** > **Copie el vínculo de vista**</span> > **Copiar vínculo** en el cuadro **Compartir vista**.

   Se copia un vínculo a la vista en el portapapeles y se recibe una confirmación en la parte inferior de la pantalla.

   Ahora puede pegar el vínculo en otra aplicación o enviarlo a otras personas.

## Conceder permisos a una vista desde una solicitud de permiso

Los usuarios que acceden a un vínculo a una vista para la que no tienen permisos pueden solicitar permisos. Todos los usuarios con permisos de Administración de la vista reciben la solicitud de permiso y pueden concederlos o denegarlos.

1. (Condicional) Si es el administrador de una vista, es posible que otro usuario le solicite el acceso a la vista en las áreas siguientes:

   * Una notificación en la aplicación
     ![Notificación en la aplicación para solicitud de acceso de vista](assets/in-app-notification-for-access-request-for-view.png)
   * Una notificación por correo electrónico
     ![Notificación en la aplicación para solicitud de acceso de vista](assets/in-app-notification-for-access-request-for-view.png)
1. (Condicional) En el área de notificación de Workfront, haga clic en la notificación dentro de la aplicación
O
En la notificación por correo electrónico, haga clic en **Ver todas las notificaciones** y, a continuación, haga clic en la notificación en la lista.

   Se muestra el cuadro **Solicitudes de acceso pendientes**.

   ![Cuadro de aprobación de lista de notificaciones](assets/notifications-list-approval-box.png)
1. (Opcional) Para el usuario cuyos permisos desea aprobar, seleccione una de las siguientes opciones en el menú desplegable situado a la derecha del nombre del usuario:
   * **Vista**
   * **Administrar**
1. Seleccione el usuario para el que desea aprobar o denegar el permiso y, a continuación, haga clic en **Aprobar todo** o **Denegar todo**.
1. Haga clic en la flecha que señala a la izquierda de **Solicitudes de acceso pendientes** y, a continuación, haga clic en **Guardar**.

   Si ha aprobado la solicitud, los usuarios se agregan al cuadro para compartir de la vista. El usuario que solicita el permiso recibe un correo electrónico de confirmación de que su solicitud se ha aprobado. <!--will they also get an in-app notification??-->

## Quitar permisos para una vista

{{step1-to-planning}}

1. Abra el espacio de trabajo cuya vista desee dejar de compartir y, a continuación, haga clic en una tarjeta de tipo de registro. Se abre la página de tipo de registro.
1. En la ficha Ver, <span class="preview"> realice una de las siguientes acciones:</span>

   * Pase el ratón sobre el nombre de la ficha de la vista que quiera compartir y haga clic en el menú **Más** ![Menú más](assets/more-menu.png) que se encuentra a la derecha del nombre de la vista; a continuación, haga clic en **Compartir**.

   * <span class="preview">Haga clic en **Compartir** > **Compartir la vista actual**</span>

   Se abre el cuadro **Compartir vista**.
1. Para quitar el uso compartido interno de una vista, haga lo siguiente:

   1. Asegúrese de que la pestaña **Uso compartido interno** esté seleccionada.
   1. Busque el usuario, grupo, equipo, empresa o rol que desea quitar, expanda el menú desplegable de permisos a la derecha del nombre de la entidad con la que comparte la vista y, a continuación, haga clic en **Quitar**.

1. Para quitar el uso compartido público de una vista, haga lo siguiente:

   1. Haga clic en la pestaña **Uso compartido público**.
   1. Anule la selección de la opción **Crear vínculo público**.

1. Haga clic en **Guardar**.

   Las personas ya no tienen acceso a la vista. A los usuarios a los que se les ha retirado el acceso a la vista no se les notifica de ninguna manera que ya no tienen acceso a ella.
