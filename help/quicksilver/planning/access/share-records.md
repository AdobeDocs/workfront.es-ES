---
title: Compartir registros
description: Puede compartir registros con el botón Compartir para aumentar la colaboración en Adobe Workfront Planning.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: e6fc6def1553df3faa8e1200f7ec2ca2bb97eb04
workflow-type: tm+mt
source-wordcount: '1620'
ht-degree: 7%

---


<!--update metadata with real information at release-->

# Compartir registros

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Puede ajustar los permisos de las personas a los registros individuales de un tipo de registro.

Puede compartir un registro de Adobe Workfront Planning de las siguientes maneras:

* Compartir un vínculo al registro.

  Para obtener más información, vea [Compartir registros mediante un vínculo](/help/quicksilver/planning/records/share-records.md).

* Comparta todos los registros de un área de trabajo con otros usuarios compartiendo el área de trabajo y el tipo de registro.

  Para obtener más información, consulte los siguientes artículos:

   * [Compartir un espacio de trabajo](/help/quicksilver/planning/access/share-workspaces.md)

   * [Compartir un tipo de registro](/help/quicksilver/planning/access/share-record-types.md)

* Compartir un registro con la opción **Compartir**.

  Este artículo describe cómo puede compartir un registro con otras personas mediante la opción **Compartir**.

>[!IMPORTANT]
>
>Los usuarios con acceso a un espacio de trabajo obtienen automáticamente al menos permisos de visualización para todos los registros del espacio de trabajo.
>Al compartir vistas, los usuarios no conceden permisos a los registros. Sólo los espacios de trabajo compartidos pueden conceder permisos a los usuarios para tipos de registro y registros.
>
>Para obtener información general sobre cómo compartir objetos en Workfront Planning, consulte también [Información general sobre los permisos de uso compartido en Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).


## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<!--at GA, check that the Workfront plans article linked below has Planning info-->

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
   <td role="rowheader"><p>Configuración de nivel de acceso</p></td> 
   <td> <p>No hay controles de nivel de acceso para Adobe Workfront Planning</p>   
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

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones al compartir registros

<!--maybe use the Share record types as example here and touch on the same points: help/quicksilver/planning/access/share-record-types.md; in addition to using Lilit's information-->

<!--checking on the below with Lilit-->

* Puede compartir registros con las siguientes entidades: personas, grupos, equipos, empresas o roles.
* Cuando comparte un área de trabajo con los usuarios, también reciben los mismos permisos para los registros del área de trabajo de forma predeterminada.
* Cuando se quita una entidad de un espacio de trabajo, todos los permisos de uso compartido se quitan de los tipos de registro y de todos los registros que contiene.
* El acceso de un usuario al registro se determina mediante la combinación de las tres opciones siguientes:

   * Sus permisos se heredan del tipo de registro y del espacio de trabajo
   * Permisos agregados individualmente en el cuadro de diálogo de uso compartido de registros
   * Los siguientes permisos:

      * **Todos los usuarios del área de trabajo pueden ver**: esto hace que el registro sea visible para todos los usuarios del área de trabajo <!-- is this OK to say "workspace? should it be "record"??-->
      * **Solo las personas invitadas pueden acceder**: Esta opción está seleccionada de forma predeterminada y permite restringir el acceso al registro a personas específicas.

* Puede conceder los siguientes niveles de permisos a un registro:

   * Ver
   * Administrar

* Al compartir un registro con un usuario, se agregan con el mismo permiso que tienen en el tipo de registro de forma predeterminada.

  Por ejemplo:

   * Si tienen permisos de visualización en el tipo de registro, obtienen permisos de visualización en el registro
   * Si tiene permisos de tipo Contribuir o Administrar en el tipo de registro, obtiene permisos de Administración en el registro

* Como administrador del espacio de trabajo, puede compartir un registro con un usuario que no forme parte del espacio de trabajo. En este caso, aparece una advertencia junto a la entidad añadida que indica que no tienen acceso al espacio de trabajo. Puede continuar agregando el usuario al registro que también lo agregará al espacio de trabajo o dejar de agregarlo al registro que tampoco lo agregará al espacio de trabajo.

* Cuando comparte un registro con usuarios que tienen permisos de Administración en el espacio de trabajo, también obtienen permisos de Administración en el registro de forma predeterminada. El permiso Ver aparece atenuado.

* Si no tiene permisos para agregar personas al espacio de trabajo, solo verá y agregará usuarios, equipos, grupos, funciones y empresas que ya se hayan agregado al espacio de trabajo. No se puede añadir ninguna otra entidad que no forme parte del espacio de trabajo.

* Puede deshabilitar los permisos heredados para un único registro, en cuyo caso puede concederles permisos para registros individuales o pueden obtener permisos si pertenecen a **Todos los usuarios del área de trabajo pueden ver** opción. <!-- is this OK to say "workspace? should it be "record"??-->

* Si se aplican varios permisos de uso compartido para el mismo usuario, recibe el permiso más alto de esos permisos.

  Por ejemplo, si un registro se comparte con un usuario con permisos de visualización y su grupo con acceso de administración, obtiene permisos de administración en el registro.

<!--Too granular??

If the inheritance has not been disabled, the user gets the maximum of inherited+individual+wildcard access 

If the inherited permissions are disabled, the user gets the maximum of wildcard+individual permissions -->

* Si un campo de fórmula o un campo de búsqueda de un registro conectado se basa en un campo de un registro en el que no tiene permisos, verá el cálculo correcto de los factores del registro a los que no puede tener acceso de otro modo.

<!-- not sure if any of the Share record types points might match here - ask Lilit??-->


## Compartir permisos de registros

Puede ajustar los permisos a los registros individuales si tiene permiso de administración en el espacio de trabajo.

{{step1-to-planning}}

1. Abra el espacio de trabajo cuyos registros desee compartir.
1. Haga clic en el tipo de registro cuyos registros desee compartir.

1. Realice una de las siguientes acciones:

   * En la vista de tabla, pase el ratón sobre el nombre de un registro, haga clic en el menú **Más** ![Menú más](assets/more-menu.png) y, a continuación, haga clic en **Compartir**.
   * En cualquier vista, haga clic en el nombre de un registro y, a continuación, haga clic en **Compartir** en la esquina superior derecha de la página de detalles del registro.

   Se abre el cuadro **Compartir**.

   ![Permisos para registros con permisos heredados en](assets/permissions-for-records-with-inherited-permissions-on.png)

1. (Opcional) En el área **Que tiene acceso**, la opción **Todos los que están en el área de trabajo pueden ver** está seleccionada de forma predeterminada.  Todos los usuarios que tengan permisos de Vista o superiores en el espacio de trabajo y tipo de registro pueden ver el registro.

1. (Opcional) Haga clic en el número de usuarios en la opción **Permisos heredados** para ver los usuarios, equipos, grupos, empresas o roles de trabajo que heredan los permisos del área de trabajo.

   >[!TIP]
   >
   >No se pueden quitar entidades individuales de la lista Permisos heredados.

1. (Opcional y condicional) Si desea compartir el tipo de registro con entidades específicas y otorgarles un acceso al tipo de registro diferente del que ya tienen para el espacio de trabajo, haga lo siguiente:

   1. Seleccione **Deshabilitar** del menú desplegable **Permisos heredados**.

   >[!TIP]
   >
   >Los administradores de Workspace siguen teniendo permisos de administración para el tipo de registro y el registro.

   1. (Opcional) Seleccione **Solo las personas invitadas pueden acceder a** desde el área de **que tiene acceso a**.

   1. En el campo **Conceder acceso a este tipo de registro**, agregue los usuarios, equipos, grupos, empresas o roles de trabajo a los que desea conceder un nivel de permiso diferente del que tienen para el área de trabajo o el tipo de registro.
   1. Elija uno de los siguientes niveles de permisos:

      * Ver
      * Administrar

      <!--checking on the below with Lilit-->

   >[!IMPORTANT]
   >
   >* Además de los equipos, grupos, empresas y funciones del puesto, solo puede compartir con los usuarios que se han añadido a Adobe Admin Console. No puede agregar usuarios solo de Workfront. Para obtener más información, consulte [Administrar usuarios en Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).
   >* Si los usuarios tienen permisos de tipo Contribuir o Gestionar en el espacio de trabajo y el tipo de registro, mantendrán los permisos de Gestionar en el registro. El permiso Ver aparece atenuado
   >* No puede conceder a los usuarios un permiso inferior al registro si tienen Contribute o superior.
   > Para obtener más información, consulte [Información general sobre los permisos de uso compartido en Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

1. Para que los usuarios que no tengan permisos de acceso al área de trabajo puedan ver un registro, en el campo **Conceder acceso a esta vista**, empiece a escribir el nombre de un usuario, un grupo, un equipo, una empresa o un rol y, a continuación, haga clic en él cuando aparezca en la lista.

   La entidad seleccionada se agrega al registro y al área de trabajo con permisos de **Ver**.

   Los administradores del sistema siempre reciben permisos de administración para los registros compartidos con ellos y existe una indicación de que un usuario es administrador del sistema.

1. (Opcional) Haga clic en **Copiar vínculo** para copiar un vínculo al registro en el portapapeles y compartirlo con otros usuarios. El vínculo abre la página de detalles del registro.
1. Haga clic en **Guardar**.

   El registro ahora se comparte con otros usuarios.
   <!--Checking with Lilit on this: The users you shared the record with receive both an in-app and email notification about having given permissions to the following entities:

   * The record
   * The record type, if they never had permissions before
   * The workspace, if they had not had permissions to the workspace before the record was shared with them. -->

1. Comparta el vínculo copiado con otros usuarios. Los usuarios que reciban el vínculo deben ser usuarios activos e iniciar sesión en Workfront para poder acceder a la página de tipo de registro y mostrarla en la vista seleccionada. Deben tener permisos sobre el tipo de registro para poder verlo. Para obtener más información, vea también [Compartir registros mediante un vínculo](/help/quicksilver/planning/records/share-records.md).

## Quitar permisos a un registro (*************** ESTO SE COPIÓ DE LOS TIPOS DE REGISTRO, DEBE EDITARSE PARA LOS REGISTROS, PERO ESPERE A LA RESPUESTA DE SLACK DE LILIT **********)

Puede quitar los permisos de los usuarios de un registro. Sin embargo, conservarán al menos los permisos de Vista en el espacio de trabajo de registros, que también les otorga al menos permisos de Vista en el tipo de registro. Debe quitar su acceso al espacio de trabajo si desea que no tengan permisos para los tipos de registro del espacio de trabajo.

{{step1-to-planning}}

1. Abra el espacio de trabajo cuyos tipos de registros desee dejar de compartir y, a continuación, haga clic en una tarjeta de tipo de registro. Se abre la página de tipo de registro.

1. En la pestaña de cualquier vista, haga clic en **Compartir** en la esquina superior derecha del tipo de registro.
1. Haga clic en **Compartir el tipo de registro**.

   Se abre el cuadro **Compartir**.
1. Busque el usuario, grupo, equipo, empresa o función de trabajo cuyos permisos desee quitar, expanda el menú desplegable de permisos a la derecha de su nombre y, a continuación, haga clic en **Quitar**. <!--check the screen shot below - the UI text for View might not be accurate-->

   ![Quitar opción en la lista desplegable de uso compartido de tipo de registro](assets/remove-option-on-record-type-sharing-drop-down.png)

1. Haga clic en **Guardar**.

   Las personas ya no tienen los permisos indicados para el tipo de registro. Sin embargo, siguen teniendo permisos en el espacio de trabajo, a menos que también los quite de los permisos del espacio de trabajo.

   A los usuarios a los que se les ha retirado el acceso a la vista no se les notifica de ninguna manera que ya no tienen acceso a ella.
