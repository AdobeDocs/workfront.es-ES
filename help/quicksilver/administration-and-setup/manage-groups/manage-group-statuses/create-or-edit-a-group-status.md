---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Crear o editar un estado de grupo
description: Como administrador de grupo, puede crear estados personalizados para un grupo que administre. Esto ayuda a eliminar la necesidad de decenas de estados personalizados en toda la compañía y permite una mayor autonomía en las jerarquías de su grupo.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 75018e0e-ff74-4afb-9a99-34bbb39b6e14
source-git-commit: 0afd578ebaa55d911c04a1d08fbcadddc1d05bbc
workflow-type: tm+mt
source-wordcount: '1345'
ht-degree: 1%

---

# Crear o editar un estado de grupo

Como administrador de grupo, puede crear estados personalizados para un grupo que administre. Esto ayuda a eliminar la necesidad de decenas de estados personalizados en toda la compañía y permite una mayor autonomía en las jerarquías de su grupo.

También puede editar un estado de nivel de sistema para un grupo que administre si un administrador de Workfront ha desbloqueado el estado. Para obtener más información, consulte [Estados bloqueados y desbloqueados en el nivel del sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md).

Si hay grupos por encima de su grupo, sus administradores también pueden hacer estas cosas por su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

>[!NOTE]
>
>Los estados de grupo personalizados no se pueden mostrar en un proyecto cuando se visualiza el proyecto en una vista Agile. Solo los estados de bloqueo predeterminados y personalizados están visibles al ver un proyecto en una vista Agile. Para obtener información sobre cómo personalizar una vista Agile para un proyecto, consulte la sección [Creación o personalización de una vista de Agile](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) en el artículo [Creación o edición de vistas en Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

Para obtener información general sobre los estados, consulte [Resumen de estados](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Workfront*</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Debe ser administrador de grupo del grupo o de Workfront. Para obtener más información, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupo</a> y <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Si necesita saber qué plan o tipo de licencia tiene, póngase en contacto con su administrador de Workfront.

## Creación o edición de un estado para un grupo

1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Grupos** ![](assets/groups-icon.png).

1. Haga clic en el nombre del grupo en el que desea crear o personalizar estados.
1. En el panel izquierdo, haga clic en **Estados**.

   Si el grupo que está visualizando es de nivel superior, la lista que se muestra incluye lo siguiente:

   * Estados bloqueados en el nivel del sistema.
   * Ya se han creado estados personalizados para el grupo.

   Además, si el grupo que está visualizando es un subgrupo, la lista también incluye:

   * Estados bloqueados que pertenecen a los grupos por encima del subgrupo.
   * Estados desbloqueados que pertenecían a los grupos por encima del subgrupo cuando se creó.

     Después de crear un subgrupo, los estados desbloqueados creados en los grupos por encima de él no se incluyen en la lista de estados del subgrupo. Sin embargo, si alguien bloquea uno de ellos más adelante, se incluye en la lista de estado del subgrupo. Para obtener más información, consulte [Cómo heredan los grupos los estados](../../../administration-and-setup/manage-groups/manage-group-statuses/how-groups-inherit-statuses.md).

1. Seleccione la pestaña del tipo de objeto (**Proyecto**, **Tareas**, o **Problemas**) que desee asociar con el estado.

1. (Condicional) Si el estado es un estado de problema, asegúrese de que **Lista maestra** está seleccionado.

   ![](assets/master-list.png)

   Para obtener información sobre cómo personalizar los demás tipos de problemas (Informe de errores, Orden de cambio, Problema, Solicitud), consulte [Personalizar tipos de problemas predeterminados](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).

1. (Condicional) Para crear un nuevo estado, haga clic en **Agregar nuevo estado**.

   O

   Para editar un estado existente, pase el ratón sobre el estado que desea editar y, a continuación, haga clic en **Editar** que se muestra en el extremo derecho.

   ![](assets/group-statuses-edit.jpg)

   >[!NOTE]
   >Puede editar un estado para su grupo solo si:
   >      
   >* Usted administra el grupo para el que se creó el estado
   >* Un administrador de Workfront desbloqueó el estado en el sistema
   >* Un administrador de grupo de un grupo por encima de su grupo desbloqueó el estado
   >      
   >      
   >Al editar un estado existente, solo puede cambiar su nombre, descripción y color.
   >
   >Cuando edita un estado bloqueado, los cambios afectan a todos los subgrupos que heredaron el estado del grupo.
   >   
   >Por el contrario, la edición del estado de desbloqueado no afecta a los subgrupos que heredaron el estado del grupo.

1. Especifique la siguiente información.

   Si está editando un estado, solo se pueden cambiar los 3 primeros ajustes.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nombre de estado</td> 
      <td> <p>Escriba un nombre para el estado. Este campo es obligatorio.</p> <p>Cuando cree un nombre de estado, tenga en cuenta que otros usuarios del sistema pueden crear un estado con el mismo nombre. Se recomienda utilizar un nombre único para evitar confusiones al seleccionar estados en Workfront.</p><p>Si existen estados duplicados, el administrador del grupo debe actualizar los nombres para diferenciar entre ellos. El único indicador de unicidad del sistema es la clave de estado.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descripción</td> 
      <td>(Opcional) Escriba una descripción del estado. Esto comunica su propósito a quienes lo utilizan.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Color</td> 
      <td> <p>Personalice el color del estado haciendo clic en el campo de color y seleccionando un color en el panel de muestras. También puede introducir un número hexadecimal en el campo.</p> <p>El color del estado se muestra en la esquina superior derecha de Workfront cuando un usuario ve el objeto.</p> <p> <img src="assets/status-color.png"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Igual que</td> 
      <td> <p>Seleccione una de las opciones de la lista que mejor describa la función del estado. Por ejemplo, si el nombre del estado es Listo, la opción con la que se equipara debe ser Completo.</p> <p>Cada estado debe coincidir con una de estas opciones, ya que esto determina cómo funciona el estado.</p> <p>Esta opción no se puede modificar una vez creado el estado.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Clave</td> 
      <td> <p>Si está creando un nuevo estado, escriba un código o una abreviatura para el estado o utilice el que se ha generado. Esta clave debe ser única en Workfront, ya que puede utilizarse para la creación de informes. Si intenta especificar una clave que ya está en uso en el sistema, el campo se vuelve rojo.</p> <p>Podría resultar útil utilizar una abreviatura que sea reconocible para quienes la utilicen.</p> <p>Esta opción no se puede modificar una vez creado el estado.</p> <p>No se puede cambiar el código de clave para los estados Planificación, Actual y Finalizado. Esto es importante si está creando un informe en modo de texto.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ocultar estado</td> 
      <td> <p>(Solo estados de proyecto y tarea)</p> <p>Active esta opción si desea que el estado se oculte a los usuarios. Cuando está desactivado (la configuración predeterminada), todos los subgrupos por debajo del grupo pueden utilizar el estado.</p> <p>Sugerencia: Para ocultar el estado de un problema, desactive los cuatro tipos de problemas (Informe de errores, Orden de cambio, Problema, Solicitud).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bloquear para todos los grupos</td> 
      <td> 
       <p>Si deja esta opción habilitada, los usuarios del grupo y sus subgrupos pueden ver y utilizar el estado y los administradores del grupo no pueden personalizarlo para subgrupos inferiores.</p> 
       <p>Cuando esta opción está desactivada, los administradores de grupos pueden personalizar el estado de los subgrupos inferiores.</p> 
       <p><b>NOTA</b>: Puede utilizar los estados bloqueado y desbloqueado en un proceso de aprobación de grupo. Si crea un proceso de aprobación de grupo con un estado de grupo desbloqueado, los usuarios pueden adjuntar el proceso de aprobación a cualquier proyecto, tarea o problema asociado con el grupo.</p> 
       <p>Para obtener más información sobre los estados de bloqueo, consulte <a href="../../../administration-and-setup/manage-groups/manage-group-statuses/lock-or-unlock-a-custom-group-status.md" class="MCXref xref">Estados de grupo bloqueados y desbloqueados</a>.</p> 
       </td> 
     </tr>
    </tbody> 
   </table>

1. Haga clic en **Guardar**.

   El estado ya está disponible para todos los proyectos asociados con su grupo o subgrupo. Si lo ha bloqueado, está disponible para su uso en subgrupos inferiores.

   Puede configurar el estado para que sea un estado predeterminado para el grupo. Para obtener más información, consulte [Usar un estado personalizado como estado predeterminado para un grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/use-custom-statuses-as-default-statuses-group.md).

## Crear un estado personalizado para varios grupos

Si es administrador de Workfront, puede crear un estado personalizado para varios grupos creando un estado para todo el sistema y ocultando ese estado a los grupos que no lo necesiten.

Si es administrador de un grupo (o de Workfront), puede crear un estado personalizado para varios subgrupos dentro de una jerarquía de grupo que administre creando un estado para un grupo de nivel superior y ocultando ese estado a cualquier subgrupo inferior que no lo necesite.

1. Si es administrador de Workfront, cree un estado de desbloqueo en todo el sistema como se describe en [Creación o edición de un estado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
1. En el cuadro de la esquina superior derecha, elimine **Estados del sistema**, empiece a escribir el nombre del grupo en el que desea ocultar el estado y, a continuación, haga clic en el nombre cuando aparezca.
1. Pase el ratón sobre el estado que quiera ocultar del grupo y haga clic en **Editar** cuando aparezca.

   ![](assets/hover-click-edit.jpg)

1. Habilite la **Ocultar estado** opción que aparece.

   ![](assets/hide-group-status.png)

1. Haga clic en **Guardar**.

   El estado aparece atenuado y ya no es visible para todos los usuarios de ese grupo.

1. Repita los pasos del 3 al 5 para ocultar el estado personalizado de cualquier otro grupo que no lo necesite.

