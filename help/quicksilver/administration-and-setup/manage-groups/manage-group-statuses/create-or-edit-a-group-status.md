---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Crear o editar un estado de grupo
description: Como administrador de grupos, puede crear estados personalizados para un grupo que administra. Esto ayuda a eliminar la necesidad de decenas de estados personalizados de toda la compañía y permite una mayor autonomía en las jerarquías de grupo.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 75018e0e-ff74-4afb-9a99-34bbb39b6e14
source-git-commit: 027d636e8256c6a12d552af736884f6f27886114
workflow-type: tm+mt
source-wordcount: '1313'
ht-degree: 1%

---

# Crear o editar un estado de grupo

Como administrador de grupos, puede crear estados personalizados para un grupo que administra. Esto ayuda a eliminar la necesidad de decenas de estados personalizados de toda la compañía y permite una mayor autonomía en las jerarquías de grupo.

También puede editar un estado de sistema para un grupo que administra si un administrador de Workfront ha desbloqueado el estado. Para obtener más información, consulte [Estados de nivel de sistema bloqueados y desbloqueados](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md).

Si hay algún grupo por encima de su grupo, sus administradores también pueden hacer esto por su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

>[!NOTE]
>
>Los estados de grupo personalizados no se pueden mostrar en un proyecto al visualizarlo en una vista ágil. Solo están visibles los estados de bloqueo predeterminados y personalizados al ver un proyecto en una vista ágil. Para obtener información sobre la personalización de una vista ágil para un proyecto, consulte la sección [Creación o personalización de una vista Águila](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) en el artículo [Información general sobre las vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

Para obtener información general sobre los estados, consulte [Resumen de los estados](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Workfront*</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Debe ser administrador de grupo del grupo o administrador de Workfront. Para obtener más información, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupo</a> y <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Si necesita saber qué plan o tipo de licencia tiene, póngase en contacto con el administrador de Workfront.

## Crear o editar un estado para un grupo

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Grupos** ![](assets/groups-icon.png).

1. Haga clic en el nombre del grupo en el que desea crear o personalizar estados.
1. En el panel izquierdo, haga clic en **Estados**.

   Si el grupo que está viendo es un grupo de nivel superior, la lista que se muestra incluye lo siguiente:

   * Estados bloqueados a nivel de sistema.
   * Estados personalizados ya creados para el grupo.

   Además, si el grupo que está viendo es un subgrupo, la lista también incluye:

   * Estados bloqueados que pertenecen a los grupos situados encima del subgrupo.
   * Estados desbloqueados que pertenecían a los grupos superiores al subgrupo cuando se creó.

      Después de crear un subgrupo, los estados desbloqueados que se crean en los grupos superiores no se incluyen en la lista de estado del subgrupo. Sin embargo, si alguien bloquea uno de ellos más adelante, se incluye en la lista de estado del subgrupo. Para obtener más información, consulte [Cómo heredan los estados los grupos](../../../administration-and-setup/manage-groups/manage-group-statuses/how-groups-inherit-statuses.md).


1. Seleccione la pestaña del tipo de objeto (**Proyecto**, **Tareas** o **Problemas**) que desea asociar al estado.

1. (Condicional) Si el estado es un estado de problema, asegúrese de que **Lista maestra** está seleccionado.

   ![](assets/master-list.png)

   Para obtener información sobre la personalización de otros tipos de problemas (Informe de errores, Orden de cambio, Problema, Solicitud), consulte [Personalización de tipos de problemas predeterminados](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).

1. (Condicional) Para crear un nuevo estado, haga clic en **Agregar un nuevo estado**.

   O

   Para editar un estado existente, pase el ratón sobre el estado que desee editar y luego haga clic en el **Editar** que se muestra en el extremo derecho.

   ![](assets/group-statuses-edit.jpg)

   >[!NOTE]
   >Puede editar un estado para su grupo solo si:
   >      
   >* Administra el grupo para el que se creó el estado
   >* Un administrador de Workfront desbloqueó el estado en el sistema
   >* Un administrador de grupo de un grupo por encima del grupo desbloqueó el estado

   >      
   >      
   >Cuando edita un estado existente, solo puede cambiar su nombre, descripción y color.
   >
   >Cuando edita un estado bloqueado, los cambios afectan a todos los subgrupos que heredaron el estado de su grupo.
   >   
   >Por el contrario, la edición de un estado desbloqueado no afecta a los subgrupos que heredaron el estado de su grupo.

1. Especifique la siguiente información.

   Si está editando un estado, solo se pueden cambiar las 3 primeras configuraciones.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nombre de estado</td> 
      <td> <p>Escriba un nombre para el estado. Este campo es obligatorio.</p> <p>Cuando cree un nombre de estado, tenga en cuenta que otros usuarios del sistema pueden crear un estado con el mismo nombre. Se recomienda utilizar un nombre único para evitar confusiones al seleccionar estados en Workfront.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descripción</td> 
      <td>(Opcional) Escriba una descripción del estado. Esto comunica su propósito a quienes lo utilizan.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Color</td> 
      <td> <p>Personalice el color del estado haciendo clic en el campo de color y seleccionando un color en el panel de muestra. También puede introducir un número hexadecimal en el campo .</p> <p>El color del estado se muestra en la esquina superior derecha de Workfront cuando un usuario ve el objeto.</p> <p> <img src="assets/status-color.png"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Igual que</td> 
      <td> <p>Seleccione una de las opciones de la lista que mejor describa la función del estado. Por ejemplo, si el nombre del estado es Listo, la opción con la que se equipara debe ser Completada.</p> <p>Cada estado debe coincidir con una de estas opciones porque esto determina cómo funciona el estado.</p> <p>Esta opción no se puede modificar una vez creado el estado.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Clave</td> 
      <td> <p>Si está creando un nuevo estado, escriba un código o abreviatura para el estado o use el que se ha generado para usted. Esta clave debe ser única en Workfront, ya que se puede utilizar para generar informes. Si intenta especificar una clave que ya se está utilizando en el sistema, el campo se vuelve rojo.</p> <p>Podría resultar útil utilizar una abreviatura reconocible para quienes la utilicen.</p> <p>Esta opción no se puede modificar una vez creado el estado.</p> <p>No se puede cambiar el código clave para los estados Planificación, Actual y Completado. Esto es importante si está creando un informe en modo de texto.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ocultar estado</td> 
      <td> <p>(Estados de proyecto y tarea únicamente)</p> <p>Active esta opción si desea que el estado esté oculto para los usuarios. Cuando está desactivado (la configuración predeterminada), todos los subgrupos debajo del grupo pueden utilizar el estado .</p> <p>Sugerencia: Puede ocultar el estado de un problema desactivando los 4 tipos de problemas (informe de errores, orden de cambio, problema, solicitud).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bloquear para todos los grupos</td> 
      <td> 
       <p>Si deja esta opción activada, los usuarios del grupo y de sus subgrupos pueden ver y utilizar el estado y los administradores de grupos no pueden personalizarlo para subgrupos inferiores.</p> 
       <p>Cuando esta opción está desactivada, los administradores de grupos pueden personalizar el estado de los subgrupos inferiores.</p> 
       <p><b>NOTA</b>: Puede utilizar los estados bloqueado y desbloqueado en un proceso de aprobación de grupo. Si crea un proceso de aprobación de grupo con un estado de grupo desbloqueado, los usuarios pueden adjuntar el proceso de aprobación a cualquier proyecto, tarea o problema asociado al grupo.</p> 
       <p>Para obtener más información sobre los estados de bloqueo, consulte <a href="../../../administration-and-setup/manage-groups/manage-group-statuses/lock-or-unlock-a-custom-group-status.md" class="MCXref xref">Estados de grupo bloqueados y desbloqueados</a>.</p> 
       </td> 
     </tr>
    </tbody> 
   </table>

1. Haga clic en **Guardar**.

   El estado ahora está disponible para todos los proyectos asociados con su grupo o subgrupo. Si la bloqueó, estará disponible para cualquier subgrupo inferior.

   Puede configurar el estado para que sea el estado predeterminado del grupo. Para obtener más información, consulte [Usar un estado personalizado como estado predeterminado para un grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/use-custom-statuses-as-default-statuses-group.md).

## Crear un estado personalizado para varios grupos

Si es administrador de Workfront, puede crear un estado personalizado para varios grupos creando un estado para todo el sistema y, a continuación, ocultándolo de cualquier grupo que no lo necesite.

Si es un administrador de grupo (o un administrador de Workfront), puede crear un estado personalizado para varios subgrupos dentro de una jerarquía de grupo que administra creando un estado para un grupo de nivel superior y, a continuación, ocultando ese estado de cualquier subgrupo inferior que no lo necesite.

1. Si es administrador de Workfront, cree un estado de desbloqueo de todo el sistema como se describe en [Crear o editar un estado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
1. En el cuadro de la esquina superior derecha, elimine **Estados del sistema**, empiece a escribir el nombre de un grupo en el que desee ocultar el estado y, a continuación, haga clic en el nombre cuando aparezca.
1. Pase el ratón sobre el estado que quiera ocultar en el grupo y haga clic en **Editar** cuando aparezca.

   ![](assets/hover-click-edit.jpg)

1. Active la variable **Ocultar estado** que aparece.

   ![](assets/hide-group-status.png)

1. Haga clic en **Guardar**.

   El estado está tenue y ya no es visible para todos los usuarios de ese grupo.

1. Repita los pasos del 3 al 5 para ocultar el estado personalizado de cualquier otro grupo que no lo necesite.
