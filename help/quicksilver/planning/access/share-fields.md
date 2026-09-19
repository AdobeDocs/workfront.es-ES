---
title: Compartir campos de planificación de Workfront
description: Puede compartir el campo de un registro de Workfront Planning con otros usuarios para garantizar la colaboración al utilizar Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: ac94936cc4dc9dc4f2d56b3f1221f71a405c5c65
workflow-type: tm+mt
source-wordcount: '1335'
ht-degree: 4%
---

# Compartir campos de Workfront Planning

{{planning-important-intro}}

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después del lanzamiento en Vista previa, las mismas funciones también están disponibles mensualmente en el entorno de producción para los clientes que habilitaron lanzamientos rápidos. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


Puede compartir el campo de un registro de Workfront Planning con otros usuarios para garantizar la colaboración al utilizar Adobe Workfront Planning.

El uso compartido de campos permite a los administradores del espacio de trabajo controlar el acceso a un campo individual. Cada campo de un tipo de registro tiene su propio cuadro de diálogo de uso compartido, donde el acceso se puede establecer en Sin acceso, Ver valores de campo o Administrar valores de campo.

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
<p>Cualquier Workfront o flujo de trabajo con un paquete de Planning</p> 
O
<p>Cualquier Workfront Planning como paquete de producto independiente</p> 
 </tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Cualquiera</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de planificación de Adobe</p></td> 
   <td><p>Cualquiera</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuración de nivel de acceso</p></td> 
   <td> <p>Debe agregar un tipo de licencia de flujo de trabajo y de Planning al nivel de acceso cuando tenga un flujo de trabajo y un paquete de Planning a la vez</p>   
</td> 
  </tr>  
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td><p>Administre permisos en un campo para cambiar los valores del campo</p>  
   <p>Permisos de contribución o superiores a un tipo de registro para heredar los permisos de administración en el campo</p>  
   </td> 
  </tr>
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones sobre el uso compartido de campos

* Puede compartir campos con usuarios, funciones del puesto, grupos, equipos o empresas.
* Solo puede compartir campos desde la vista de tabla de un tipo de registro.
* No puede compartir los siguientes tipos de campos:

  * Campos del sistema (por ejemplo, Creado por, ID de registro)
  * Campos principales
  * Campos de búsqueda. Siempre heredan los permisos de los campos de objeto de origen.
* El acceso a un campo se obtiene combinando las siguientes configuraciones:

  * **Permisos heredados**: De forma predeterminada, un campo hereda el mismo acceso que alguien tiene en el tipo de registro. Puede desactivar los permisos heredados y proporcionar a los usuarios un acceso al campo menor que el que tienen para el tipo de registro.
  * Las **personas con acceso al tipo de registro pueden ver** o **Solo las personas invitadas pueden tener acceso a la selección**. Puede permitir que todos los usuarios con permisos en el espacio de trabajo vean el campo o conceder permisos solo a entidades individuales.

  Si se aplican varias reglas a la misma persona, reciben el permiso más alto disponible de una de las reglas.

* Para que un campo sea de solo lectura para todos los usuarios de un espacio de trabajo, asegúrese de que exista la siguiente configuración:

  * Desactivar permisos heredados
  * Mantener la configuración **Todos los que tengan acceso al tipo de registro pueden ver**
  * No agregue entidades individuales.

* Según los permisos de tipo de registro, los usuarios pueden recibir los siguientes permisos de campo:

  * Ver permisos de tipo de registro: otorga a un usuario permisos para ver valores de campo
  * Los permisos de tipo Contribuir o Administrar registro otorgan a un usuario permisos para administrar valores de campo

* Solo los propietarios y administradores del espacio de trabajo pueden ajustar los permisos de campo. Los administradores de Workspace siempre conservan el acceso de Administración a todos los campos y esto no se puede reducir.
* El uso compartido de campos controla el acceso a los valores, no la configuración de los campos. Solo los administradores de espacio de trabajo pueden cambiar la configuración de un campo.
* Agregar a alguien a la lista de uso compartido de un campo no les concede acceso de tipo de registro o de espacio de trabajo. Si no tienen ese acceso, un icono de advertencia indica que el permiso solo surtirá efecto una vez que se añadan al tipo de registro.
* Los campos con permisos restringidos se aplican en todas partes donde se muestra el campo. Esto incluye todas las vistas, páginas de detalles de registro, formularios de solicitud, conexiones y campos de búsqueda, paneles de lienzo, la API y las herramientas de MCP.
* Las vistas públicas siguen siendo totalmente visibles y de solo lectura para cualquier persona que pueda acceder a ellas.
  <!--Not sure if this is right - right now, it allows me to duplicate with the values in the new record - checking with Lilit: * When you duplicate a record, the restricted values are not copied to the new records.-->
* Los cambios de valor de campo restringidos no se registran en el historial de un registro.
* Los cambios de permisos para los campos no almacenan en déclencheur las notificaciones.
* Para los tipos de registro globales, los permisos de campo se aplican a todos los espacios de trabajo secundarios y no se pueden ajustar localmente.

<!--
From Claude: 
Additional permissions for fields - maybe add this to the Overview article for all of the sharing?? - help/quicksilver/planning/access/sharing-permissions-overview.md 

Here's how record type / workspace access maps to field-level access in the document:

Field permission levels (only two, plus none):

No Access – field is completely hidden
View field values – can see the value, can't edit
Manage field values – can view and edit

Default inheritance from record type role

Record type / workspace access    Default field permission
View    View field values
Contribute    Manage field values
Manage (workspace manager)    Manage field values (locked — cannot be reduced)

So by default, a field simply mirrors whatever role someone has on the record type — Viewers get read-only, Contributors and Managers get edit rights. Workspace managers are a special case: whenever they're added to a field's sharing list, "Manage field values" is pre-selected and the "View field values" option is disabled, since their edit access can never be taken away.

Wildcard (fallback) setting
Separate from inheritance, each field has a wildcard default:

Everyone in the workspace can view (default)
Only invited people can access

How the final permission is calculated

If inherited permissions are enabled: a person's access = the highest of (inherited from record type, wildcard, individually granted permission).
If inherited permissions are disabled: a person's access = the highest of (wildcard, individually granted permission) — record type role no longer factors in.
If inheritance is disabled, wildcard is "Only invited people can access," and the person isn't individually added → they get No Access.

Other permission notes

Individually granting access to someone doesn't grant them workspace/record-type access — it just sits inactive (with a warning icon) until they're separately added to the workspace.
For Global Record Types, field permissions are set once and apply to all secondary workspaces; secondary/team workspace managers cannot override them locally.

-->

## Compartir campos

Como administrador del espacio de trabajo, puede ajustar permisos a campos individuales.

{{step1-to-planning}}

1. Abra el espacio de trabajo y, a continuación, el tipo de registro cuyos campos desee compartir.

1. En la vista de tabla, pase el ratón sobre el nombre del encabezado de columna de un campo, haga clic en el menú **Más** ![Menú más](assets/more-menu.png) y, a continuación, haga clic en **Compartir campo**.

   Se abre el cuadro **Compartir**.

1. (Opcional) En el área de **Conceder acceso**, la opción **Todas las personas con acceso al tipo de registro pueden ver** está seleccionada de forma predeterminada. Todos los usuarios que tienen **Ver** o permisos superiores en el área de trabajo y el tipo de registro tienen los mismos permisos en el campo.

1. (Opcional) Haga clic en los avatares de los usuarios en la opción **Permisos heredados de** para ver los usuarios, equipos, grupos, empresas o roles de trabajo que heredan los permisos del área de trabajo.

   Los permisos del usuario para el tipo de registro se muestran cuando expande los permisos heredados.

   >[!TIP]
   >
   >No se pueden quitar entidades individuales de la lista de permisos heredados. Se muestran los usuarios de equipos, grupos, empresas o funciones del puesto en lugar de las entidades con las que estaban asociados cuando se compartió el espacio de trabajo y el tipo de registro con ellos.

1. (Opcional y condicional) Si desea compartir el campo con entidades específicas y otorgarles un acceso al campo diferente al que ya tienen para el tipo de registro, haga lo siguiente:

   1. Anule la selección de la opción **Activado** de **Permisos heredados**. Está seleccionada de forma predeterminada.

      La opción cambia a **Desactivado**.

      >[!TIP]
      >
      >Los administradores de Workspace siguen teniendo permisos de administración en el tipo de registro y el campo.

   1. (Opcional) Haga clic en el menú desplegable **Todas las personas con acceso al tipo de registro pueden ver** y seleccione **Solo las personas invitadas pueden acceder**.

      >[!IMPORTANT]
      >
      >Este cambio, junto con la desactivación de **Permisos heredados**, quita el acceso a todas las personas que pueden ver el tipo de registro y dar acceso únicamente a las personas designadas. Los administradores y gestores de Workspace siempre tendrán acceso a todos los campos.


   1. En el cuadro **Conceder acceso**, agregue los usuarios, equipos, grupos, empresas o roles de trabajo a los que desee conceder un nivel de permiso diferente del que tienen para el área de trabajo o el tipo de registro.

      Cuando comparte un campo con un usuario, su función de trabajo principal y su correo electrónico también se muestran en el campo. Debe tener activada la configuración Ver información de contacto para el objeto Usuarios en su nivel de acceso para poder ver el correo electrónico del usuario.

   1. Elija uno de los siguientes niveles de permisos:

      * Ver valores de campo
      * Administrar valores de campo

      >[!IMPORTANT]
      >
      ><!-- * If users have Contribute or Manage permissions to the workspace and the record type, you can give them Manage permissions to the field. The View permission is dimmed.-->
      >* No puede conceder a los usuarios un permiso inferior al campo si tienen Contribute o superior al tipo de registro.
      >
      >* No puede conceder permisos a usuarios que no están en el espacio de trabajo. Los usuarios que no tienen permisos de acceso al espacio de trabajo y tipo de registro no pueden acceder a ninguno de los campos. Podrán acceder a los campos cuando obtengan permisos para el espacio de trabajo y los tipos de registro.

1. Haga clic en **Guardar**.

   El campo ahora se comparte con otros usuarios.

   <!--
    Not possible for fields: 
    The users you shared the field with receive both an in-app and email notification about having been given permissions to the field.
    For information, see [Adobe Workfront Planning notifications: article index](/help/quicksilver/planning/notifications/notifications-information.md).
    -->

## Eliminación de permisos de un campo

Puede quitar los permisos de los usuarios de un campo. Sin embargo, conservarán al menos los permisos de Vista en el espacio de trabajo y el tipo de registro, lo que también les otorga al menos permisos de Vista en el campo.

Debe quitar su acceso al espacio de trabajo si desea que no tengan permisos para los tipos de registros o campos del espacio de trabajo.

No puede quitar un usuario de los permisos heredados.

{{step1-to-planning}}

1. Abra el espacio de trabajo cuyos campos desee dejar de compartir y, a continuación, haga clic en una tarjeta de tipo de registro. Se abre la página de tipo de registro.
1. En la vista de tabla, pase el ratón sobre el nombre del encabezado de columna de un campo, haga clic en el menú **Más** ![Menú más](assets/more-menu.png) y, a continuación, haga clic en **Compartir campo**.

   Se abre el cuadro **Compartir**.
1. Busque el usuario, grupo, equipo, empresa o función de trabajo cuyos permisos desee quitar, expanda el menú desplegable de permisos a la derecha de su nombre y, a continuación, haga clic en **Quitar**.

1. Haga clic en **Guardar**.

   Las personas ya no tienen los permisos indicados en el campo. Sin embargo, aún tienen permisos para el tipo de registro y el espacio de trabajo, a menos que también los quite de esos permisos.

   No hay notificación para los usuarios que se han eliminado del acceso al campo de que ya no tienen estos permisos.
