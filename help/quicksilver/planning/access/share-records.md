---
title: Compartir registros
description: Puede compartir registros con el botón Compartir para aumentar la colaboración en Adobe Workfront Planning.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 9ffad1aa-3c96-40fa-9c62-7a3e00699f18
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/NTytTWD-zq3PVhXn4n-GHinvQxna1wfnAXjaeYBgTEY
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: c33c023ab33a3b0c8369e6fae091d0ec877aa4e2
workflow-type: tm+mt
source-wordcount: 1720
ht-degree: 7%

---

<!--update metadata with real information at release-->

# Compartir registros

<!--
this will NOT be available in Preview ever - find a way to add this in this article that is prominent
-->

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>\
<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Puede ajustar los permisos de las personas a los registros individuales de un tipo de registro en Adobe Workfront Planning.

Puede compartir un registro de Adobe Workfront Planning de las siguientes maneras:

* Compartir un vínculo al registro.

  Para obtener más información, vea [Compartir registros mediante un vínculo](/help/quicksilver/planning/records/share-records.md).

* Comparta todos los registros de un área de trabajo con otros usuarios compartiendo el área de trabajo y el tipo de registro.

  Para obtener más información, consulte los siguientes artículos:

   * [Compartir un espacio de trabajo](/help/quicksilver/planning/access/share-workspaces.md)

   * [Compartir un tipo de registro](/help/quicksilver/planning/access/share-record-types.md)

* Compartir un registro individual o compartir varios registros de forma masiva mediante la opción **Compartir**.

  Este artículo describe cómo puede compartir registros con otras personas mediante la opción **Compartir**.

>[!IMPORTANT]
>
>* Los usuarios con acceso a un espacio de trabajo obtienen automáticamente al menos permisos de visualización para todos los registros del espacio de trabajo.
>* Al compartir vistas, los usuarios no conceden permisos a los registros. Sólo los espacios de trabajo compartidos pueden conceder permisos a los usuarios para tipos de registro y registros.
>
>Para obtener información general sobre cómo compartir objetos en Workfront Planning, consulte también [Información general sobre los permisos de uso compartido en Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<!--
at GA, check that the Workfront plans article linked below has Planning info
-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
   <td role="rowheader"><p>Paquete de Adobe Workfront</p></td> 
   <td> 
<p>Cualquier paquete de Workfront y Planning</p> 
O
<p>Cualquier paquete de flujo de trabajo y planificación</p> 
 </tr>

<tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Cualquiera</p> 
   <p><b>NOTA</b></p>
   <p>Solo se pueden conceder permisos de administración a los registros a las personas con una licencia Standard. Todas las demás licencias solo pueden tener permisos de visualización y la opción Administrar aparece atenuada para ellas.</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>  <p>Administrar permisos para un espacio de trabajo, un tipo de registro y el registro</p>  
   <p><b>IMPORTANTE</b></p>
   <p>Solo los usuarios con permisos de Administración de un espacio de trabajo pueden compartir un registro</p></td> 
  </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> A los usuarios con una licencia Light o Contributor se les debe asignar una plantilla de diseño que incluya Planning.
   <p>Los usuarios estándar y los administradores del sistema tienen las áreas de Planning habilitadas de forma predeterminada.</p></div></li></ul>
</td>
  </tr>

</tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones al compartir registros

<!--
maybe use the Share record types as example here and touch on the same points: help/quicksilver/planning/access/share-record-types.md; in addition to using Lilit's information
-->

<!--checking on the below with Lilit-->

* Puede compartir registros con las siguientes entidades: personas, grupos, equipos, empresas o roles.
* Si restringe los permisos a un registro, los usuarios ya no verán ese registro y los valores de sus campos de búsqueda en ningún lugar del sistema donde se muestre ese registro.
* Workfront comprueba los permisos de registro en conexiones de hasta 5 registros de profundidad, lo que garantiza que los usuarios solo vean los registros compartidos con ellos.
* Puede conceder los siguientes niveles de permisos a un registro:

   * Ver
   * Administrar
* Cuando comparte un espacio de trabajo y un tipo de registro con los usuarios, también reciben los mismos permisos para los registros del espacio de trabajo de forma predeterminada.
Cuando los usuarios tienen permisos de contribución para un espacio de trabajo o tipo de registro, reciben permisos de administración para los registros de ese tipo de registro.
* Cuando se quita una entidad de un espacio de trabajo, todos los permisos de uso compartido se quitan de los tipos de registro y de todos los registros que contiene.
* No se puede compartir un registro con un usuario que no tenga permisos para el área de trabajo o el tipo de registro.

  Si comparte un registro con alguien que no está en el área de trabajo, se agregará automáticamente al área de trabajo.
* El acceso de un usuario al registro se determina mediante la combinación de las tres opciones siguientes:

   * Sus permisos se heredan del tipo de registro y del espacio de trabajo
   * Permisos agregados individualmente en el cuadro para compartir registros
   * **Todos los usuarios del área de trabajo pueden ver**.

     Esto hace que todos los usuarios del espacio de trabajo puedan ver el registro

     <!--
      Cannot do this on a record: 
      * **Only invited people can access**: This is selected by default and allows restricting access to the record to specific people. 
      -->

* Al compartir un registro con un usuario, se agregan con el mismo permiso que tienen en el tipo de registro de forma predeterminada.

  Por ejemplo:

   * Si tienen permisos de visualización en el tipo de registro, obtienen permisos de visualización en el registro
   * Si tiene permisos de tipo Contribuir o Administrar en el tipo de registro, obtiene permisos de Administración en el registro

* Cuando un usuario tiene permisos de Administrar o Contribuir en el espacio de trabajo y el tipo de registro y los añade a los permisos de registro, los permisos de Vista aparecen atenuados. Conservan los mismos permisos para el registro que para el tipo de registro y no se les pueden conceder permisos inferiores para el registro.

* Puede deshabilitar los permisos heredados para un único registro, en cuyo caso puede conceder a determinados usuarios permisos para registros individuales o pueden obtener permisos si pertenecen al área de trabajo, debido a la opción **Todos los usuarios del área de trabajo pueden ver**.

* Si se aplican varios permisos de uso compartido para el mismo usuario, recibirá el nivel más alto de esos permisos.

  Por ejemplo, si un registro se comparte con un usuario con permisos de visualización y su grupo con acceso de administración, recibirá permisos de administración en el registro.

* Si un campo de fórmula o un campo de búsqueda de un registro conectado se basa en un campo de un registro en el que no tiene permisos, verá el cálculo correcto de los factores del registro a los que no puede tener acceso de otro modo.

  <!--
   Not possible: 
   * As a workspace manager, you can share a record with a user that does not have permissions to the record type or the workspace. In this case, there is a warning next to the added entity notifying you that they don't have access to the workspace or the record type.  You can continue adding the user to the record which will also add them to the record type and workspace, or cancel the sharing.
   -->

  <!--
   ensure this is this way, because in devtest the warning only shows record type, but logged a bug to add "workspace" to the warning too
   -->

<!--
Lilit is checking on this, it is not working correctly
-->

<!--
   check on this: I cannot disable inherited permissions when this setting is ON and this documented in a TIP below: When they have View permissions to the workspace or the record type, they retain View permissions to the records. You can grant them Manage permissions to the record by disabling Inherited permissions and selecting the Only invited people can access setting.
   -->

<!-- 
   not sure what this means, confusing, hiding for now: * If you don't have permissions to add people to the workspace, you will only see and add users, teams, groups, roles, and companies that are already added to the workspace. You cannot add any other entity that is not already part of the workspace.
   -->

<!--
   Too granular??
   If the inheritance has not been disabled, the user gets the maximum of inherited+individual+wildcard access 
   If the inherited permissions are disabled, the user gets the maximum of wildcard+individual permissions 
   -->

<!--
   not sure if any of the Share record types points might match here - ask Lilit??
   -->

## Compartir registros

Como administrador del espacio de trabajo, puede ajustar permisos a registros individuales.

{{step1-to-planning}}

1. Abra el espacio de trabajo y, a continuación, el tipo de registro cuyos registros desee compartir.

1. Realice una de las siguientes acciones:

   * En la vista de tabla, pase el ratón sobre el nombre de un registro, haga clic en el menú **Más** ![Menú más](assets/more-menu.png) y, a continuación, haga clic en **Compartir**.
   * En la vista de tabla, seleccione uno o varios registros y, a continuación, haga clic en **Compartir** en la barra de herramientas azul situada en la parte inferior de la lista.
   * En cualquier vista, haga clic en el nombre de un registro y, a continuación, haga clic en **Compartir** en la esquina superior derecha de la página de detalles del registro.

   Se abre el cuadro **Compartir**.

   ![Permisos para registros con permisos heredados en](assets/permissions-for-records-with-inherited-permissions-on.png)

   >[!WARNING]
   >
   >No puede compartir permisos a registros que se agregan en diferentes espacios de trabajo. Cuando comparte registros de forma masiva, todos los registros deben crearse en el mismo espacio de trabajo.

1. (Opcional) En el área **Que tiene acceso**, la opción **Todos los que están en el área de trabajo pueden ver** está seleccionada de forma predeterminada.  Todos los usuarios que tienen **View** o permisos superiores en el área de trabajo y el tipo de registro tienen los mismos permisos para el registro.

1. (Opcional) Haga clic en los avatares de los usuarios en la opción **Permisos heredados de** para ver los usuarios, equipos, grupos, empresas o roles de trabajo que heredan los permisos del área de trabajo. <!--logged bug to move "Permissions" to lowercase-->

   Los permisos del usuario para el tipo de registro se muestran cuando expande los permisos heredados.

   >[!TIP]
   >
   >No se pueden quitar entidades individuales de la lista de permisos heredados. Se muestran los usuarios de equipos, grupos, empresas o funciones del puesto en lugar de las entidades con las que estaban asociados cuando se compartió el espacio de trabajo y el tipo de registro con ellos.

1. (Opcional y condicional) Si desea compartir el registro con entidades específicas y otorgarles un acceso al tipo de registro diferente del que ya tienen para el espacio de trabajo, haga lo siguiente:

   1. Anule la selección de la opción **Activado** de **Permisos heredados**. Está seleccionada de forma predeterminada.

      La opción cambia a **Desactivado**.

      >[!TIP]
      >
      >Los administradores de Workspace y los creadores de registros siguen teniendo permisos de administración para el tipo de registro y el registro.

      <!-- 
      This is no longer possible for a record: 
      (Optional) Select **Only invited people can access** from the **Who has access** area. You must indicate individual users, groups, teams, or companies to share the records with. 
      >[!TIP]
      >
      >You cannot disable or enable Inherited permissions when this setting is selected.
      -->

   1. En el campo **Conceder acceso a este registro**, agregue los usuarios, equipos, grupos, empresas o roles de trabajo a los que desea conceder un nivel de permiso diferente del que tienen para el área de trabajo o el tipo de registro.

      Cuando comparte un registro con un usuario, su función de trabajo principal y su correo electrónico también se muestran en el campo. Debe tener activada la configuración Ver información de contacto para el objeto Usuarios en su nivel de acceso para poder ver el correo electrónico del usuario.

   1. Elija uno de los siguientes niveles de permisos:

      * Ver
      * Administrar

      >[!IMPORTANT]
      >
      >* Si los usuarios tienen permisos de tipo Contribuir o Administrar en el espacio de trabajo y el tipo de registro, puede concederles permisos de Administración en el registro. El permiso Ver aparece atenuado.
      >* No puede conceder a los usuarios un permiso inferior al registro si tienen Contribute o superior al tipo de registro.
      >Para obtener más información, consulte [Información general sobre los permisos de uso compartido en Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).
      >* No puede conceder permisos a usuarios que no están en el espacio de trabajo. Los usuarios que no tienen permisos de acceso al espacio de trabajo y tipo de registro no pueden acceder a ninguno de los registros.

   <!--   
   Not possible:
   1. To give users who do not have permissions to the workspace access to view a record, in the **Grant access to this view** field, start typing the name of a user, a group, team, company, or job role, then click it when it displays in the list. 
      The entity you selected is added to the record and also to the record type and the workspace with **View** permissions. 
      System administrators always receive Manage permissions to records shared with them, and there is an indication that a user is a System administrator.
   -->

1. (Opcional) Haga clic en **Copiar vínculo** para copiar un vínculo al registro en el portapapeles y compartirlo con otros usuarios. El vínculo abre la página de detalles del registro.
1. Haga clic en **Guardar**.

   El registro ahora se comparte con otros usuarios.

   Los usuarios con los que compartió el registro reciben una notificación en la aplicación y por correo electrónico sobre la concesión de permisos para el registro.

   <!--
   not possible anymore: 
   * The record
   * The record type, if they never had permissions before
   * The workspace, if they had not had permissions to the workspace before the record was shared with them.
   -->

   Para obtener más información, consulte [Notificaciones de Adobe Workfront Planning: índice de artículo](/help/quicksilver/planning/notifications/notifications-information.md).


1. (Opcional) Comparta el vínculo copiado con otros usuarios.

   Los usuarios que reciban el vínculo deben ser usuarios activos e iniciar sesión en Workfront para poder acceder a la página de tipo de registro y mostrarla en la vista seleccionada.

   Deben tener permisos sobre el tipo de registro para poder verlo.

   Para obtener más información, vea también [Compartir registros mediante un vínculo](/help/quicksilver/planning/records/share-records.md).


## Eliminación de permisos de un registro

Puede quitar los permisos de los usuarios de un registro. Sin embargo, conservarán al menos los permisos de Vista en el espacio de trabajo, que también les otorga al menos permisos de Vista en el tipo de registro.

Debe quitar su acceso al espacio de trabajo si desea que no tengan permisos para los tipos de registros o registros del espacio de trabajo.

No puede quitar un usuario de los permisos heredados.

{{step1-to-planning}}

1. Abra el espacio de trabajo cuyos registros desee dejar de compartir y, a continuación, haga clic en una tarjeta de tipo de registro. Se abre la página de tipo de registro.
1. Realice una de las siguientes acciones:

   * En la vista de tabla, pase el ratón sobre el nombre de un registro, haga clic en el menú **Más** ![Menú más](assets/more-menu.png) y, a continuación, haga clic en **Compartir**.
   * En la vista de tabla, seleccione uno o varios registros y, a continuación, haga clic en **Compartir** en la barra de herramientas azul situada en la parte inferior de la lista.

     Debe seleccionar registros creados en el mismo espacio de trabajo.
   * En cualquier vista, haga clic en el nombre de un registro y, a continuación, haga clic en **Compartir** en la esquina superior derecha de la página de detalles del registro.

   Se abre el cuadro **Compartir**.
1. Busque el usuario, grupo, equipo, empresa o función de trabajo cuyos permisos desee quitar, expanda el menú desplegable de permisos a la derecha de su nombre y, a continuación, haga clic en **Quitar**.

   ![Quitar permisos en el registro](assets/remove-option-on-record-sharing-drop-down.png)

1. Haga clic en **Guardar**.

   Las personas ya no tienen los permisos indicados para el registro. Sin embargo, aún tienen permisos para el tipo de registro y el espacio de trabajo, a menos que también los quite de esos permisos.

   No hay notificación para los usuarios que se han eliminado del acceso al registro de que ya no tienen estos permisos.
