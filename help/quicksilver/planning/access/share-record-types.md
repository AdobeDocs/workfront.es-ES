---
title: Compartir tipos de registros
description: Puede compartir un tipo de registro con otros usuarios para garantizar la colaboración al utilizar Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: bf49db73-09f1-417e-836b-16c6062740d4
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '1505'
ht-degree: 8%

---


<!-- take the Remove permissions section out, at the end - this is what Lilit said: Because of "Everyone in the workspace can view" wildcard, currently it's not possible to entirely remove access to a record type. Let's take out this section. -->

# Compartir tipos de registros

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Puede compartir un tipo de registro con otros usuarios para garantizar la colaboración al trabajar con registros en Adobe Workfront Planning.

>[!IMPORTANT]
>
>Los usuarios con acceso a un espacio de trabajo obtienen automáticamente al menos permisos de visualización para todos los tipos de registros del espacio de trabajo.
>>Al compartir vistas, los usuarios no conceden permisos a los tipos de registro. Sólo los espacios de trabajo compartidos pueden conceder permisos de usuario a los tipos de registro.
>
>* Para obtener información general sobre cómo compartir objetos en Workfront Planning, consulte también [Información general sobre los permisos de uso compartido en Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).
>* Para obtener más información, vea la sección [Consideraciones al compartir tipos de registros](#considerations-when-sharing-record-types) en este artículo.

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
   <td>  <p>Administración de permisos para un tipo de registro</p>  
   <p>Solo los usuarios con permisos de administración en un espacio de trabajo pueden compartir permisos de administración en un tipo de registro</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Plantilla de diseño</p></td> 
   <td> <p>En el entorno de producción, todos los usuarios, incluidos los administradores del sistema, deben estar asignados a una plantilla de diseño que incluya las áreas de planificación.</p>
<p><span class="preview">En el entorno de vista previa, los usuarios estándar y los administradores del sistema tienen activada de forma predeterminada el área de Planning.</span></p> </td> 
  </tr> 
</tbody> 
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones al compartir tipos de registros

* De forma predeterminada, la concesión de permisos a un espacio de trabajo proporciona a los usuarios los mismos permisos para los tipos de registros del espacio de trabajo.

  Además, puede ajustar los permisos en tipos de registros individuales.

  Sin embargo, no puede conceder a las personas permisos superiores a los permisos que tienen para el espacio de trabajo.
* Puede conceder a los usuarios permisos inferiores a los que tienen en el espacio de trabajo. Por ejemplo, pueden tener permisos de contribución en el espacio de trabajo y permisos de visualización en un tipo de registro.
* Las personas con permiso de administración en el espacio de trabajo siempre mantienen su acceso de administración en todos los tipos de registros del espacio de trabajo. Sus permisos no se pueden reducir en los tipos de registro, aunque los permisos heredados estén desactivados.

* Actualmente puede lograr lo siguiente cuando comparte tipos de registros:

   * Asigne permisos de visualización a las personas en un espacio de trabajo cuando comparta un tipo de registro con ellas por primera vez y no tengan permisos para el espacio de trabajo.

     Esto también les proporciona permisos de Vista para todos los tipos de registros del espacio de trabajo.

     A medida que se les otorgan permisos para el tipo de registro, en el cuadro para compartir se indica que también se agregan al espacio de trabajo.
   * Convierta el tipo de registro en de solo lectura para todos los usuarios del espacio de trabajo (excepto para los administradores del espacio de trabajo) cuando desactive los permisos heredados.

     Las personas con permisos de Administración en el espacio de trabajo siempre tienen permisos de Administración en los tipos de registro, incluso cuando se desactivan los permisos heredados en el tipo de registro.
   * Reduzca el permiso de las personas a un tipo de registro. No se puede aumentar el permiso de una persona a un tipo de registro con respecto a lo que tiene en el área de trabajo.

     Por ejemplo, si alguien tiene permiso para contribuir en el área de trabajo, puede cambiar su permiso a un tipo de registro específico a Ver. Sin embargo, si tienen permiso de visualización en el espacio de trabajo, no se les puede otorgar permiso de contribución a ningún tipo de registro.

* No es posible eliminar el acceso a un tipo de registro para las personas en el espacio de trabajo. Todos los usuarios siempre tienen al menos permiso de visualización en todos los tipos de registro si tienen al menos permisos de visualización en el espacio de trabajo.

* Puede compartir un tipo de registro internamente con las siguientes entidades:

  Usuarios, grupos, equipos, empresas y funciones del Workfront
* No puede compartir tipos de registros externamente con usuarios fuera de Workfront.
* Para conceder a un usuario que no tenga permisos de área de trabajo superiores a los permisos de Vista para un tipo de registro, primero debe compartir el área de trabajo con él con un permiso superior al de Vista. Los permisos superiores para el espacio de trabajo se aplicarán a los tipos de registro.

## Permisos de uso compartido para un tipo de registro

Puede ajustar los permisos a los tipos de registro individuales de un espacio de trabajo si tiene permiso de administración en el espacio de trabajo.

{{step1-to-planning}}

1. Abra el espacio de trabajo cuyos tipos de registro desee compartir y, a continuación, haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.

1. En la pestaña de cualquier vista, haga clic en **Compartir** en la esquina superior derecha del tipo de registro.

   Se abre el cuadro **Compartir**.

   ![Permisos para tipos de registros con permisos heredados en](assets/permissions-for-record-types-with-inherited-permissions-on.png)

1. (Opcional) En el área **Que tiene acceso**, la opción **Todos los que están en el área de trabajo pueden ver** está seleccionada de forma predeterminada.  Todos los usuarios que tengan permisos de Vista o superiores en el espacio de trabajo pueden ver el tipo de registro.

1. (Opcional) Haga clic en el número de usuarios en la opción **Permisos heredados** para ver los usuarios, equipos, grupos, empresas o roles de trabajo que heredan los permisos del área de trabajo.

   >[!TIP]
   >
   >No se pueden quitar entidades individuales de la lista Permisos heredados.


1. (Opcional y condicional) Si desea compartir el tipo de registro con entidades específicas y otorgarles un acceso al tipo de registro diferente del que ya tienen para el espacio de trabajo, haga lo siguiente:

   1. Seleccione **Deshabilitar** del menú desplegable **Permisos heredados**.

   >[!TIP]
   >
   >Los administradores de Workspace siguen teniendo permisos de administración en el tipo de registro.

   1. En el campo **Conceder acceso a este tipo de registro**, agregue los usuarios, equipos, grupos, empresas o roles de trabajo a los que desee conceder un nivel de permiso diferente del que tienen para el área de trabajo.
   1. Elija un nivel de permisos.

   >[!IMPORTANT]
   >
   >* Además de los equipos, grupos, empresas y funciones del puesto, solo puede compartir con los usuarios que se han añadido a Adobe Admin Console.
   >* Nunca puede conceder a los usuarios permisos superiores a los que tienen en un espacio de trabajo.
   >* No puede conceder a los usuarios un permiso inferior al de Administrar a un tipo de registro si tienen permisos de Administración en el espacio de trabajo.
   >* Puede conceder a los usuarios un permiso inferior al tipo de registro si tienen permisos de contribución en el espacio de trabajo.
   > Para obtener más información, consulte [Información general sobre los permisos de uso compartido en Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

1. Para que los usuarios que no tengan permisos de acceso al área de trabajo puedan ver un tipo de registro, en el campo **Conceder acceso a esta vista**, empiece a escribir el nombre de un usuario, un grupo, un equipo, una empresa o un rol y, a continuación, haga clic en él cuando aparezca en la lista.

   La entidad seleccionada se agrega al tipo de registro y al área de trabajo con permisos de **Ver**.

   Los administradores del sistema siempre reciben permisos de administración para los tipos de registros compartidos con ellos y existe una indicación de que un usuario es administrador del sistema.

1. (Opcional) Haga clic en **Copiar vínculo** para copiar un vínculo al tipo de registro en el portapapeles y compartirlo con otros usuarios.
1. Haga clic en **Guardar**.

   El tipo de registro ahora se comparte con otros usuarios.

1. Comparta el vínculo copiado con otros usuarios. Los usuarios que reciban el vínculo deben ser usuarios activos e iniciar sesión en Workfront para poder acceder a la página de tipo de registro y mostrarla en la vista seleccionada. Deben tener permisos sobre el tipo de registro para poder verlo.

## Eliminación de permisos de un tipo de registro

Puede quitar los permisos de los usuarios de un tipo de registro. Sin embargo, conservarán al menos los permisos de Vista en el espacio de trabajo, que también les otorga al menos permisos de Vista en el tipo de registro. Debe quitar su acceso al espacio de trabajo si desea que no tengan permisos para los tipos de registro del espacio de trabajo.

{{step1-to-planning}}

1. Abra el espacio de trabajo cuyos tipos de registros desee dejar de compartir y, a continuación, haga clic en una tarjeta de tipo de registro. Se abre la página de tipo de registro.

1. En la pestaña de cualquier vista, haga clic en **Compartir** en la esquina superior derecha del tipo de registro.

   Se abre el cuadro **Compartir**.
1. Busque el usuario, grupo, equipo, empresa o función de trabajo cuyos permisos desee quitar, expanda el menú desplegable de permisos a la derecha de su nombre y, a continuación, haga clic en **Quitar**. <!--check the screen shot below - the UI text for View might not be accurate-->

   ![Quitar opción en la lista desplegable de uso compartido de tipo de registro](assets/remove-option-on-record-type-sharing-drop-down.png)

1. Haga clic en **Guardar**.

   Las personas ya no tienen los permisos indicados para el tipo de registro. Sin embargo, siguen teniendo permisos en el espacio de trabajo, a menos que también los quite de los permisos del espacio de trabajo.

   A los usuarios a los que se les ha retirado el acceso a la vista no se les notifica de ninguna manera que ya no tienen acceso a ella.

<!-- This is not working yet: *************************** edit this before publishing, because this was not tested with record types - this section came from sharing views *******************: 

## Grant permissions to a record type from a permission request

Users who access a link to a record type to which they do not have permissions can request permissions to the record type. All users with Manage permissions to the view receive the permission request and can grant or deny the permissions. 

1. (Conditional) If you are are the manager of a view, you might receive a request from another user to access the view in the following areas:
   
   * An in-app notification
      ![In-app notification for access request for view](assets/in-app-notification-for-access-request-for-view.png)
   * An email notification
      ![In-app notification for access request for view](assets/in-app-notification-for-access-request-for-view.png)
1. (Conditional) From the notification area in Workfront, click the in-app notification
   Or
   From the email notification, click **View all notifications**, then click the notification in the list.

   The **Pending access requests** box displays. 

      ![Notifications list approval box](assets/notifications-list-approval-box.png)
1. (Optional) For the user whose permissions you want to approve, select one of the following options from the drop-down menu to the right of the user's name: 
   * **View**
   * **Manage**
1. Select the user for whom you want to approve or deny the permission, then click **Approve all** or **Deny all**. 
1. Click the left-pointing arrow to the left of **Pending access requests**, then click **Save**.

   If you approved the request, the users are added to the sharing box of the view. The user requesting the permission receives an email confirmation that their request was approved. <!--will they also get an in-app notification??-->

