---
title: Compartir vistas
description: Puede compartir una vista con otros usuarios para garantizar la colaboración cuando se utiliza Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 673dd888-3135-48b0-8198-c8d6d6706ddf
source-git-commit: 1dc2791bed0dfada109ee102e09c25ae9a52e6b0
workflow-type: tm+mt
source-wordcount: '1540'
ht-degree: 58%

---


# Compartir vistas

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Puede compartir una vista con otros usuarios para garantizar la colaboración cuando se trabaja con registros en Adobe Workfront Planning.

>[!IMPORTANT]
>
>* La concesión de permisos a un espacio de trabajo no significa que se conceden permisos a otros usuarios para ver las páginas de tipo de registro. Es preciso conceder permisos a las vistas individuales de una página de tipo de registro para compartirlas con otros usuarios.
>
>* La concesión de permisos a una vista no cambia los permisos de visualización de los registros. Los permisos de registro se conceden al compartir espacios de trabajo.
>
>* Cuando comparte una vista, concede permisos a otros usuarios para que accedan a todos los elementos de la vista. Por ejemplo, cuando les concede permisos de administración para una vista, pueden modificar su agrupación, filtro, ordenación o apariencia de barra.


Puede compartir una vista con las siguientes entidades:

* Internamente, con usuarios, grupos, equipos, empresas y funciones de Workfront
* Públicamente, con usuarios de fuera de Workfront

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
<p>La instancia de Workfront de su organización debe incorporarse a Adobe Unified Experience para poder acceder a todas las funcionalidades de Workfront Planning.</p> 
<p>Su organización debe incorporarse a la experiencia unificada de Adobe para que los usuarios puedan solicitar y conceder permisos a una vista desde una solicitud de permiso. </p>
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

## Consideraciones al compartir vistas

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

1. En la pestaña Ver, pase el ratón sobre la vista que quiera compartir, haga clic en el menú **Más** ![Menú Más](assets/more-menu.png), a la derecha del nombre de la vista y, a continuación, haga clic en **Compartir**.

   ![Menú más para vistas expandido con la opción de uso compartido](assets/more-menu-for-views-expanded-with-share-option.png)

   La pestaña **Uso compartido interno** debería estar seleccionada de manera predeterminada.

1. (Opcional) En el área **Quién tiene acceso**, seleccione una de las siguientes opciones:

   * **Solo las personas invitadas pueden tener acceso**: debe especificar los usuarios, grupos, equipos, empresas o roles con los que desea compartir la vista. Esta es la opción predeterminada.
   * **Todos los usuarios del espacio de trabajo pueden ver**: todos los usuarios que tengan permisos de visualización o superiores en los espacios de trabajo pueden acceder a la vista.

1. En el campo **Conceder acceso a esta vista**, empiece a escribir el nombre de un usuario, un grupo, un equipo, una empresa o un rol y, a continuación, haga clic en él cuando se muestre en la lista.

   ![Compartir una vista con grupos](assets/sharing-a-view-ui-with-groups.png)

1. Seleccione uno de los siguientes niveles de permisos en el menú desplegable:
   * Ver
   * Administrar

     Para obtener información acerca de los niveles de permisos y las acciones que los usuarios pueden realizar en cada nivel, consulte [Información general sobre los permisos de uso compartido en Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

     Los administradores del sistema siempre reciben permisos de administración para las vistas compartidas con ellos.

1. Haga clic en **Copiar vínculo** para copiar un vínculo a la vista en el portapapeles.
1. Haga clic en **Guardar**.

   La vista se actualiza con un icono de personas ![Vista compartida con otros iconos](assets/view-shared-with-others-people-icon.png) para indicar que la vista ahora se comparte con otros usuarios.

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

1. En la pestaña Ver, pase el ratón sobre la vista que quiera compartir, haga clic en el menú **Más** ![Menú Más](assets/more-menu.png), a la derecha del nombre de la vista y, a continuación, haga clic en **Compartir**.

   ![Menú más para vistas expandido con la opción de uso compartido](assets/more-menu-for-views-expanded-with-share-option.png)

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
1. Pase el ratón sobre el nombre de la ficha de la vista de la que quiera quitar el uso compartido y haga clic en el menú **Más** ![Menú más](assets/more-menu.png); a continuación, haga clic en **Compartir**.
1. Para quitar el uso compartido interno de una vista, haga lo siguiente:

   1. Asegúrese de que la pestaña **Uso compartido interno** esté seleccionada.
   1. Busque el usuario, grupo, equipo, empresa o rol que desea quitar, expanda el menú desplegable de permisos a la derecha del nombre de la entidad con la que comparte la vista y, a continuación, haga clic en **Quitar**.

1. Para quitar el uso compartido público de una vista, haga lo siguiente:

   1. Haga clic en la pestaña **Uso compartido público**.
   1. Anule la selección de la opción **Crear vínculo público**.

1. Haga clic en **Guardar**.

   Las personas ya no tienen acceso a la vista. A los usuarios a los que se les ha retirado el acceso a la vista no se les notifica de ninguna manera que ya no tienen acceso a ella.
