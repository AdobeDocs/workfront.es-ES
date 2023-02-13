---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Creación y modificación de las plantillas de proyecto de un grupo
description: Cuando visualiza un grupo que administra en el área Grupos, puede ver y trabajar con plantillas de proyecto asociadas al grupo y a cualquiera de sus subgrupos.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f97a12eb-9002-4f11-908a-c68c1e6dc9c9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1284'
ht-degree: 1%

---

# Creación y modificación de las plantillas de proyecto de un grupo

Cuando visualiza un grupo que administra en el área Grupos, puede ver y trabajar con plantillas de proyecto asociadas al grupo y a cualquiera de sus subgrupos.

Si hay algún grupo por encima de su grupo, sus administradores también pueden hacer esto por su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

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
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver acceso o superior en las plantillas que desee ver y trabajar con</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Si necesita saber qué plan o tipo de licencia tiene, póngase en contacto con el administrador de Workfront.

## Ver, trabajar con y crear plantillas para su grupo desde el área Grupos

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Grupos** ![](assets/groups-icon.png).

1. Haga clic en el nombre del grupo para el que desea crear o modificar plantillas.
1. En el panel izquierdo, haga clic en **Plantillas** para enumerar las plantillas asociadas al grupo y a cualquier subgrupo que pueda tener.

   Debe tener acceso de visualización a una plantilla para verla en esta lista. Para obtener información sobre este acceso, consulte [Concesión de acceso a plantillas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md).

1. Realice una de las siguientes acciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Agregar una plantilla</td> 
      <td> <p>Haga clic en <strong>Nueva plantilla</strong>y, a continuación, configúrela usando las opciones disponibles. Para obtener información sobre estas opciones, consulte <a href="../../../manage-work/projects/create-and-manage-templates/create-template.md" class="MCXref xref">Creación de una plantilla de proyecto</a>.</p> <p>La plantilla se asocia automáticamente al grupo.</p> <p>Para obtener información sobre cómo se aplican las preferencias de grupo a las plantillas nuevas, consulte <a href="#how-preferences-apply-to-templates-and-template-tasks" class="MCXref xref">Aplicación de las preferencias a las plantillas y a las tareas de plantilla</a> en este artículo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Editar una o más plantillas</td> 
      <td> <p>Seleccione al menos una plantilla y haga clic en el icono Editar <img src="assets/edit-icon.png">y, a continuación, utilice cualquiera de las opciones disponibles para configurarlo. Para obtener información sobre estas opciones, consulte <a href="../../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Editar plantillas de proyecto</a>.</p> <p>El icono Editar solo está disponible si tiene acceso de edición a todas las plantillas seleccionadas. Para obtener información sobre este acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Concesión de acceso a plantillas</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Eliminar una o más plantillas</td> 
      <td> <p>Seleccione al menos una plantilla y, a continuación, haga clic en el icono Eliminar <img src="assets/delete.png">.</p> <p>Este icono solo está disponible si tiene acceso de edición a todas las plantillas seleccionadas. Para obtener información sobre este acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Concesión de acceso a plantillas</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Compartir una o más plantillas</td> 
      <td> <p>Seleccione al menos una plantilla y haga clic en el icono Compartir <img src="assets/share-icon.png">y, a continuación, haga clic en una de las siguientes opciones del menú desplegable:</p> 
       <ul> 
        <li> <p><strong>Plantilla</strong>: En el <strong>Acceso a plantilla</strong> que se muestra, agregue nombres para especificar quién desea tener acceso a la plantilla misma.</p> <p>Para obtener más información, consulte la sección <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md#share" class="MCXref xref">Compartir una plantilla</a> en el artículo <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md" class="MCXref xref">Compartir plantillas de proyecto</a>.</p> </li> 
        <li><strong>Proyecto</strong>: En el <strong>Acceso a proyectos</strong> que se muestra, agregue nombres para especificar quién desea tener acceso a los proyectos creados a partir de la plantilla</li> 
       </ul> <p>El icono Compartir solo está disponible si tiene acceso Compartir a todas las plantillas que seleccione. Para obtener información sobre este acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Concesión de acceso a plantillas</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exportación de la lista de plantillas</td> 
      <td>Haga clic en <strong>Exportar</strong> <img src="assets/export.png">y, a continuación, seleccione el formato de archivo que desee para la lista exportada.</td> 
     </tr> 
    </tbody> 
   </table>

## Aplicación de las preferencias a las plantillas y a las tareas de plantilla {#how-preferences-apply-to-templates-and-template-tasks}

Cuando crea una plantilla de proyecto, la configuración que se muestra en las tablas siguientes se configura automáticamente mediante una preferencia de proyecto o tarea correlacionada.

>[!NOTE]
>
>Una preferencia de tarea o un proyecto de nivel de grupo o de nivel de sistema afecta a una plantilla de proyecto, en función de si la asoció con un grupo cuando la creó.
>
>Si lo asoció a un grupo, la preferencia de nivel de grupo surtirá efecto. Esto ocurre en los siguientes casos:
>
>* La plantilla se crea desde el área Grupos , tal como se explica en este artículo
>* Especifique un grupo al crear la plantilla con un archivo Kickstart
>* Especifique un grupo al crear la plantilla con la API
>
>Si no asoció la nueva plantilla a un grupo, la preferencia a nivel de sistema surtirá efecto. Esto ocurre cuando se encuentran en los escenarios siguientes. (Si posteriormente asigna un grupo a la plantilla o a la tarea de plantilla, las preferencias del grupo no le afectan).
>
>* La plantilla se crea desde el área Plantillas
>* No se especifica ningún grupo al crear la plantilla con un archivo Kickstart
>* No se especifica ningún grupo al crear la plantilla con la API
>


* [Ajustes de plantilla de proyecto configurados por las preferencias de proyecto y tarea](#project-template-settings-configured-by-project-and-task-preferences)
* [Configuración de tareas de plantilla configurada por las preferencias de tareas](#template-task-settings-configured-by-task-preferences)

### Ajustes de plantilla de proyecto configurados por las preferencias de proyecto y tarea {#project-template-settings-configured-by-project-and-task-preferences}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Método de índice de rendimiento</p> </td> 
   <td> <p>Configurado por la preferencia de proyecto de nivel de grupo "Método de índice de rendimiento" si asocia la nueva plantilla con un grupo o la misma preferencia de proyecto de nivel de sistema si no lo hace.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Tipo de condición</p> </td> 
   <td> <p>Configurado por la preferencia de proyecto de nivel de grupo "Establezca automáticamente la condición del proyecto en función del estado de progreso" si asocia la nueva plantilla con un grupo o la misma preferencia de proyecto de nivel de sistema si no lo hace.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Programar desde</p> </td> 
   <td> <p>Configurado por la preferencia de proyecto de nivel de grupo "Programar desde" si asocia la nueva plantilla con un grupo o la misma preferencia de proyecto de nivel de sistema si no lo hace.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Tiempo de espera del usuario</p> </td> 
   <td> <p>Configurado por la preferencia de proyecto de nivel de grupo "Tiempo de espera del usuario" si asocia la nueva plantilla a un grupo o la misma preferencia de proyecto de nivel de sistema si no lo hace.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Tipo de actualización</p> </td> 
   <td> <p>Configurado por la preferencia de proyecto de nivel de grupo "Las líneas de tiempo del proyecto se vuelven a calcular automáticamente" si asocia la nueva plantilla con un grupo o la misma preferencia de proyecto de nivel de sistema si no lo hace.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Acceso a la configuración de la sección</p> </td> 
   <td> <p>Configurado por las preferencias de tarea de nivel de grupo en la sección "Acceso" si asocia la nueva plantilla con un grupo o la misma preferencia de proyecto de nivel de sistema si no lo hace.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener información sobre las preferencias del proyecto que se enumeran en esta tabla, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Para obtener información sobre la tarea y las preferencias de problema, consulte [Configurar las preferencias de problemas y tareas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>* Si cambia el grupo que está asociado con una plantilla de proyecto existente, la configuración de la plantilla sigue siendo la misma.
>* Si mueve una tarea de plantilla existente a otra plantilla, la siguiente configuración permanece sin cambios en la tarea de plantilla, independientemente del grupo asociado con la nueva plantilla:>
   >   * Tipo de duración
   >   * Tipo de ingresos
   >   * Tipo de costo
>
>  Sin embargo, la tarea de plantilla se ve afectada por la configuración &quot;Cuando a alguien se le asigna una tarea&quot; en la nueva plantilla. Para obtener más información, consulte la sección [Acceso](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#access) en el artículo [Editar plantillas de proyecto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).
>
>* Cuando un administrador guarda un proyecto como plantilla, todos los ajustes de la plantilla se heredan del proyecto, incluido el grupo.
>
>  Cuando un administrador convierte una tarea o un problema en un proyecto mediante una plantilla, todos los ajustes de la plantilla están determinados por lo que ya se ha guardado en la plantilla.

### Configuración de tareas de plantilla configurada por las preferencias de tareas {#template-task-settings-configured-by-task-preferences}

Al crear una tarea de plantilla, algunos de sus ajustes se configuran automáticamente mediante una preferencia de tarea correlacionada. Estos ajustes se enumeran en la siguiente tabla.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Tipo de duración </p> </td> 
   <td> <p>Configurado por la preferencia de tarea de nivel de grupo "Tipo de duración" si asocia la plantilla a un grupo, o la misma tarea de nivel de sistema y preferencia de emisión si no lo hace.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Tipo de ingresos</p> </td> 
   <td> <p>Configurado por la preferencia de tarea de nivel de grupo "Tipo de ingresos" si asocia la plantilla a un grupo, o la misma tarea de nivel de sistema y preferencia de emisión si no lo hace.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Tipo de costo </p> </td> 
   <td> <p> Configurado por la preferencia de tarea de nivel de grupo "Tipo de coste" si asocia la plantilla a un grupo, o la misma tarea de nivel de sistema y preferencia de emisión si no lo hace.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener información sobre las preferencias de tareas que se enumeran en esta tabla, consulte [Configurar las preferencias de problemas y tareas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
