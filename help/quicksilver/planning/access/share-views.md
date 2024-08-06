---
title: Compartir vistas
description: Puede compartir una vista con otros usuarios para garantizar la colaboración al utilizar Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 673dd888-3135-48b0-8198-c8d6d6706ddf
source-git-commit: d5d517a0c9a1292c37e66db07f7ed17d0a9a59e1
workflow-type: tm+mt
source-wordcount: '1117'
ht-degree: 1%

---

<!--update the metadata and description when we turn this article live-->

# Compartir vistas

{{planning-important-intro}}

Puede compartir una vista con otros usuarios para garantizar la colaboración al trabajar con registros en Adobe Workfront Planning.

>[!IMPORTANT]
>
>* Al conceder permisos a un espacio de trabajo, no se conceden permisos a otros usuarios para las vistas de las páginas de tipo de registro. Debe conceder permisos a vistas individuales de una página de tipo de registro para compartirlas con otros usuarios.
>
>* La concesión de permisos a una vista no cambia los permisos de visualización de los registros. Los permisos de registro los concede compartir espacios de trabajo.
>
>* Cuando comparte una vista, otorga a otros permisos para acceder a todos los elementos de la vista. Por ejemplo, cuando se les conceden permisos de administración de una vista, pueden modificar la apariencia de agrupación, filtro, ordenación o barra.


Puede compartir una vista con las siguientes entidades:

* Internamente, con usuarios y grupos de Workfront
* Públicamente, con usuarios fuera de Workfront

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso para Workfront Planning.

<!--at GA the plan below will change to Prime, Select and Ultimate only-->

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
   <p> Adobe Workfront</p> </td>
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
   O
   <p>Actual: plan </p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuraciones de nivel de acceso</p></td>
   <td> No hay controles de acceso para Adobe Workfront Planning</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Permisos</p></td>
   <td> <p>Administración de permisos en una vista</p>  
   <p>Solo los usuarios con permisos de Administración de un espacio de trabajo pueden compartir una vista públicamente.</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>A todos los usuarios, incluidos los administradores de Workfront, se les debe asignar una plantilla de diseño que incluya el área de Planning en el menú principal. </p> <p>Para obtener más información, consulte <a href="/help/quicksilver/planning/access/access-overview.md">Resumen de acceso</a>. </p> 
</td>
  </tr>
 </tbody>
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones al compartir vistas

* Puede conceder permisos de Vista o Administración a una vista a usuarios internos de Workfront.

* Los usuarios con permisos de Administración pueden modificar la configuración de vista, compartirla, duplicarla o eliminarla.

* Puede compartir vistas con personas fuera de su organización mediante un vínculo público.

* Cuando comparte una vista públicamente, cualquier persona fuera de la compañía puede acceder al vínculo durante un tiempo limitado, indicado por la fecha de caducidad. No se requiere inicio de sesión para ver la vista compartida.

* Las personas externas a la organización que tienen acceso a una vista no pueden crear otras vistas, editar la vista compartida ni agregar, eliminar o editar la información de registro de la vista.

## Compartir permisos en una vista internamente

Puede compartir las vistas que ha creado o las vistas en las que tiene permiso de administración con usuarios o grupos en Workfront.

>[!NOTE]
>
>Los administradores del sistema no pueden ver ni compartir vistas que no hayan creado ellos mismos. Solo pueden acceder a las vistas que se comparten con ellos o compartirlas.
>
>Los administradores del sistema solo pueden tener permisos de Administración para una vista.

{{step1-to-planning}}

1. Abra el espacio de trabajo cuya vista desee compartir y, a continuación, haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.

1. En la pestaña Ver, pase el ratón sobre la vista que quiera compartir, haga clic en el menú **Más** ![](assets/more-menu.png), a la derecha del nombre de la vista y, a continuación, haga clic en **Compartir**.

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

   La ficha **Uso compartido interno** debe estar seleccionada de manera predeterminada.

1. (Opcional) En el área **Que tiene acceso**, seleccione una de las siguientes opciones:

   * **Solo las personas invitadas pueden tener acceso**: debe especificar los usuarios o grupos con los que desea compartir la vista. Esta es la opción predeterminada.
   * **Todos los usuarios del área de trabajo pueden ver**: todos los usuarios que tengan permisos de Vista o superiores en los espacios de trabajo pueden tener acceso a la vista.

1. En el campo **Conceder acceso de vista a**, empiece a escribir el nombre de un usuario o grupo y, a continuación, haga clic en él cuando aparezca en la lista.

   ![](assets/sharing-a-view-ui-with-groups.png)

1. Seleccione uno de los siguientes niveles de permisos en el menú desplegable:
   * Ver
   * Administrar

     Para obtener información acerca de los niveles de permisos y las acciones que los usuarios pueden realizar en cada nivel, vea [Información general sobre los permisos de uso compartido en Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

     Los administradores del sistema siempre reciben permisos de administración para las vistas compartidas con ellos.

1. Haga clic en **Copiar vínculo** para copiar un vínculo a la vista en el portapapeles.
1. Haga clic en **Guardar**.

   La vista se actualiza con un icono de personas ![](assets/view-shared-with-others-people-icon.png) para indicar que la vista ahora se comparte con otros usuarios.

   >>
   [!TIP]
   >>
   Las vistas sin un icono de persona o global son vistas que ha creado y no se comparten con otros. Las vistas no compartidas solo son visibles para usted.

1. Compartir el vínculo copiado con otros usuarios. Los usuarios que reciban el vínculo deben ser usuarios activos e iniciar sesión en Workfront para poder acceder a la página de tipo de registro y mostrarla en la vista seleccionada.

## Compartir permisos en una vista públicamente

Puede compartir las vistas que ha creado o las vistas en las que tiene permisos de administración con personas que no tienen una licencia de Workfront y que pueden ser externas a su organización.

>[!IMPORTANT]
>
Solo los usuarios con permisos de Administración de un espacio de trabajo pueden compartir las vistas del espacio de trabajo de forma pública.


Para compartir una vista públicamente en Workfront Planning:

{{step1-to-planning}}

1. Abra el espacio de trabajo cuya vista desee compartir y, a continuación, haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.

1. En la pestaña Ver, pase el ratón sobre la vista que quiera compartir, haga clic en el menú **Más** ![](assets/more-menu.png), a la derecha del nombre de la vista y, a continuación, haga clic en **Compartir**.

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

1. Haga clic en **Uso compartido público**.

   ![](assets/public-sharing-tab-for-views.png)

1. Habilitar la configuración **Crear vínculo público**.

   Aparecerá un vínculo disponible. Este es un vínculo público. Cuando se comparte, cualquier persona que tenga el vínculo, incluidas las personas externas a la organización, puede acceder a la página de tipo de registro y ver los registros y campos de la página.

1. Haga clic en el icono **Copiar vínculo** ![](assets/copy-link-view.png) para copiar el vínculo en el portapapeles.

1. Escriba una fecha manualmente o use el calendario del campo **Fecha de caducidad del vínculo** para seleccionar una fecha de caducidad para el vínculo público. No se podrá acceder a la vista de página de registros después de la fecha seleccionada.

1. Haga clic en **Guardar**.

   La vista se actualiza con un icono global ![](assets/public-shared-view-icon-highlighted.png) para indicar que la vista se comparte públicamente.

   >>
   [!TIP]
   >
   >Las vistas sin un icono de persona o global son vistas que ha creado y no se comparten con otros. Las vistas no compartidas solo son visibles para usted.


1. (Opcional) Pegue el vínculo que ha copiado en un correo electrónico, mensaje de chat, documento o comentario de Workfront para compartirlo con otros usuarios.

## Eliminación de permisos de una vista

{{step1-to-planning}}

1. Abra el espacio de trabajo cuya vista desee dejar de compartir y, a continuación, haga clic en una tarjeta de tipo de registro. Se abre la página de tipo de registro.
1. Pase el ratón sobre el nombre de la ficha de la vista de la que quiera quitar el uso compartido y haga clic en el menú **Más** ![](assets/more-menu.png); a continuación, haga clic en **Compartir**.
1. Para eliminar el uso compartido interno de una vista, haga lo siguiente:

   1. Asegúrese de que la ficha **Uso compartido interno** esté seleccionada.
   1. Busque el usuario o grupo que desea quitar, expanda el menú desplegable de permisos a la derecha del nombre del usuario o grupo y, a continuación, haga clic en **Quitar**.

1. Para quitar el uso compartido público de una vista, haga lo siguiente:

   1. Haga clic en la ficha **Uso compartido público**.
   1. Anule la selección de la opción **Crear vínculo público**.

1. Haga clic en **Guardar**.

   Las personas ya no tienen acceso a la vista. No hay notificación para los usuarios que se han eliminado del acceso a la vista de que ya no tienen este acceso.