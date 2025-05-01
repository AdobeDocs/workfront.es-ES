---
title: Compartir tipos de registros
description: Puede compartir un tipo de registro con otros para asegurarse de colaboración al utilizar Adobe Systems Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: bf49db73-09f1-417e-836b-16c6062740d4
source-git-commit: 6e2e337969fccba88ea7089fe9a6d9db605343f7
workflow-type: tm+mt
source-wordcount: '1499'
ht-degree: 9%

---


<!-- take the Remove permissions section out, at the end - this is what Lilit said: Because of "Everyone in the workspace can view" wildcard, currently it's not possible to entirely remove access to a record type. Let's take out this section. -->

# Compartir tipos de registros

<span class="preview">La información sobre este Página se refiere a funcionalidad aún no están generalmente disponibles. Solo está disponible en la entorno de Vista previa para todos los clientes. Después de los lanzamientos mensuales para Producción, las mismas características también están disponibles en el entorno de producción para los clientes que habilitaron lanzamientos rápidos. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Puede compartir un tipo de registro con otros para asegurarse de colaboración al trabajar con registros en Adobe Systems Workfront Planning.

>[!IMPORTANT]
>
>Los usuarios con acceso a una espacio de trabajo obtienen automáticamente al menos Ver permisos para todos los tipos de registros de la espacio de trabajo.
>Compartir vistas no otorga a los usuarios permisos para grabar tipos. Solo los espacios de trabajo compartidos pueden otorgar a los usuarios permisos para grabar tipos.
>
>* Para obtener información general sobre cómo compartir objetos en Workfront Planning, consulte [también Información general sobre el uso compartido de permisos en Adobe Systems Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).
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
<p>La planificación de Workfront no está disponible para los planes de Workfront heredados</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Paquete Adobe Systems Workfront Planning*</p></td> 
   <td> 
<p>Cualquiera </p> 
<p>Para obtener más información sobre lo que se incluye en cada plan de planificación de Workfront, comuníquese con su Administrador de cuentas de Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Plataforma Adobe Systems Workfront</p></td> 
   <td> 
<p>El instancia de Workfront de su organización debe incorporarse a la Adobe Systems Unified Experience para poder acceder a todas las capacidades de Workfront Planning.</p> 
<p>Su organización debe estar integrada a la Experiencia unificada de Adobe Systems para que los usuarios puedan solicitud y conceder permisos a una vista desde una solicitud de permiso. </p>
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
   <td>  <p>Administrar permisos para un tipo de registro</p>  
   <p>Solo los usuarios con permisos de administración de una espacio de trabajo pueden compartir permisos de administración para un tipo de registro.</p></td> 
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

## Consideraciones al compartir tipos de registros

* De forma predeterminada, la concesión de permisos a un espacio de trabajo proporciona a los usuarios los mismos permisos para los tipos de registros del espacio de trabajo.

  Además, puede ajustar los permisos en tipos de registros individuales.

  Sin embargo, no se pueden conceder a las personas permisos más altos para un tipo de registro que los permisos que tienen para el espacio de trabajo.
* Puede conceder a los usuarios permisos para el tipo de registro menores que los que tienen en el espacio de trabajo. Por ejemplo, pueden tener permisos Contribute para el espacio de trabajo y permisos Ver en un tipo de registro.
* Las personas con Manage permiso al espacio de trabajo siempre mantienen su acceso Manage a todos los tipos de registros del espacio de trabajo. Sus permisos no se pueden reducir en los tipos de registro, igualado cuando los permisos heredados están desactivados.

* Actualmente puede lograr lo siguiente al compartir tipos de registros:

   * Asigne permisos de visualización a las personas en un espacio de trabajo cuando comparta un tipo de registro con ellas por primera vez y no tengan permisos para el espacio de trabajo.

     Esto también les otorga Ver permisos para todos los tipos de registros del espacio de trabajo.

     A medida que les otorga permisos para el tipo de registro, hay una indicación en el cuadro de uso compartido de que también se agregan al espacio de trabajo.
   * Haga que el tipo de registro sea solo vista para todos los usuarios del espacio de trabajo (excepto para los administradores de espacio de trabajo), cuando deshabilite los permisos heredados.

     Las personas con permisos Administrar al espacio de trabajo siempre tienen permisos Administrar en los tipos de registro, igualado cuando desactiva los permisos heredados en el tipo de registro.
   * Baja la permiso de las personas a un tipo de registro. No se puede aumentar el permiso de una persona a un tipo de registro con respecto a lo que tiene en el área de trabajo.

     Por ejemplo, si alguien tiene permiso para contribuir en el área de trabajo, puede cambiar su permiso a un tipo de registro específico a Ver. Sin embargo, si tienen permiso de visualización en el espacio de trabajo, no se les puede otorgar permiso de contribución a ningún tipo de registro.

* No es posible eliminar el acceso a un tipo de registro para las personas en el espacio de trabajo. Todos los usuarios siempre tienen al menos permiso de visualización en todos los tipos de registro si tienen al menos permisos de visualización en el espacio de trabajo.

* Puede compartir un tipo de registro internamente con las siguientes entidades:

  Usuarios de Workfront, grupos, equipos, empresas y roles de trabajo
* No puede compartir tipos de registros externamente con usuarios fuera de Workfront.
* Para otorgar un usuario que no tiene permisos espacio de trabajo superiores a Ver permisos a un tipo de registro, primero debe compartir el espacio de trabajo con ellos con un permiso superior al Ver. Los permisos más altos para el espacio de trabajo se aplicarán a los tipos de registro.

## Permisos de uso compartido a un tipo de registro

Puede ajustar los permisos a tipos de registro individuales de una espacio de trabajo si tiene Administrar permiso al espacio de trabajo.

{{step1-to-planning}}

1. Abra la espacio de trabajo cuyos tipos de registros desee compartir y, a continuación, haga clic en un tipo de registro tarjeta.

   Se abre la página de tipo de registro.

1. En la pestaña de cualquier vista, haga clic **en Compartir** en la esquina superior derecha del tipo de registro.

   Se abre el **cuadro Compartir** .

   ![Permisos para tipos de registro con permisos heredados en](assets/permissions-for-record-types-with-inherited-permissions-on.png)

1. (Opcional) En el área **Que tiene acceso**, la opción **Todos los que están en el área de trabajo pueden ver** está seleccionada de forma predeterminada.  Todos los usuarios que tengan permisos de Vista o superiores en el espacio de trabajo pueden ver el tipo de registro.

1. (Opcional) Haga clic en el número de usuarios en la opción **Permisos heredados** para ver los usuarios, equipos, grupos, empresas o roles de trabajo que heredan los permisos del área de trabajo.

   >[!TIP]
   >
   >No puede quitar entidades individuales del lista Permisos heredados.


1. (opcional y condicional) Si desea compartir el tipo de registro con entidades específicas y concederles un acceso al tipo de registro diferente del que ya tienen para el espacio de trabajo, haga lo siguiente:

   1. Seleccione **Deshabilitar** en el **menú desplegable Permisos** heredados.

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
   >* Puede conceder a los usuarios un permiso menor al tipo de registro si tienen permisos Contribute al espacio de trabajo.
   > Para obtener más información, consulte [Información general sobre los permisos de uso compartido en Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

1. Para conceder a los usuarios que no tienen permisos para el espacio de trabajo acceso a vista un tipo de registro, en el **campo Conceder acceso a este vista** , inicio escriba el nombre de una usuario, una grupo, equipo, compañía o función de trabajo y, a continuación, haga clic en él cuando se muestre en el lista.

   La entidad seleccionada se agrega al tipo de registro y al espacio de trabajo con **Ver** permisos.

   Los administradores del sistema siempre reciben permisos de administración para registrar los tipos compartidos con ellos, y hay una indicación de que un usuario es un administrador del sistema.

1. (Opcional) Haga clic en **Copiar vincular** para copiar un vincular al tipo de registro en su portapapeles y compartirlo con otras personas.
1. Haga clic en **Guardar**.

   El tipo de registro ahora se comparte con otros usuarios.

1. Comparta el vínculo copiado con otros usuarios. Los usuarios que reciban el vincular deben ser usuarios activos e iniciar sesión en Workfront para poder acceder al Página de tipo de registro y mostrarlo en el vista seleccionado. Debe tener permisos sobre el tipo de registro para poder vista él.

## Quitar permisos a un tipo de registro.

Puede quitar los permisos de los usuarios de un tipo de registro. Sin embargo, conservarán al menos el acceso de visualización al espacio de trabajo, que les otorga permisos para ver al menos el tipo de registro. Debe quitar su acceso de la espacio de trabajo si desea que no tengan permisos para los tipos de registro del espacio de trabajo.

{{step1-to-planning}}

1. Abra la espacio de trabajo cuyos tipos de registro desea dejar de compartir y, a continuación, haga clic en un tipo de registro tarjeta. Se abre la página de tipo de registro.

1. En la pestaña de cualquier vista, haga clic **en Compartir** en la esquina superior derecha del tipo de registro.

   Se abre el **cuadro Compartir** .
1. Busque el usuario, grupo, equipo, compañía o función trabajo cuyos permisos desea eliminar, expanda el menú desplegable de permisos a la derecha de su nombre y haga clic en **Quitar**. <!--check the screen shot below - the UI text for View might not be accurate-->

   ![Quitar opción en el menú desplegable Uso compartido de tipos de registro](assets/remove-option-on-record-type-sharing-drop-down.png)

1. Haga clic en **Guardar**.

   Las personas ya no tienen los permisos indicados para el tipo de registro. Sin embargo, todavía tienen permisos para el espacio de trabajo, a menos que también los elimine de espacio de trabajo permisos.

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

