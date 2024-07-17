---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Crear y modificar las plantillas de proyecto de un grupo
description: Cuando vea un grupo que administra en el área de Grupos, puede ver y trabajar con plantillas de proyecto asociadas al grupo y a cualquiera de sus subgrupos.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f97a12eb-9002-4f11-908a-c68c1e6dc9c9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1284'
ht-degree: 1%

---

# Crear y modificar las plantillas de proyecto de un grupo

Cuando vea un grupo que administra en el área de Grupos, puede ver y trabajar con plantillas de proyecto asociadas al grupo y a cualquiera de sus subgrupos.

Si hay grupos por encima de su grupo, sus administradores también pueden hacer estas cosas por su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

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
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver el acceso o superior a las plantillas que desea ver y con las que desea trabajar</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Si necesita saber qué plan o tipo de licencia tiene, póngase en contacto con su administrador de Workfront.

## Vea, trabaje con y cree plantillas para su grupo desde el área de Grupos

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y, a continuación, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Grupos** ![](assets/groups-icon.png).

1. Haga clic en el nombre del grupo para el que desea crear o modificar plantillas.
1. En el panel izquierdo, haga clic en **Plantillas** para ver una lista de las plantillas asociadas con el grupo y con los subgrupos que pueda tener.

   Debe tener acceso de visualización a una plantilla para verla en esta lista. Para obtener información sobre este acceso, consulte [Conceder acceso a las plantillas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md).

1. Realice una de las siguientes acciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Añadir una plantilla</td> 
      <td> <p>Haga clic en <strong>Nueva plantilla</strong> y, a continuación, configúrela con las opciones disponibles. Para obtener información acerca de estas opciones, vea <a href="../../../manage-work/projects/create-and-manage-templates/create-template.md" class="MCXref xref">Crear una plantilla de proyecto</a>.</p> <p>La plantilla se asocia automáticamente al grupo.</p> <p>Para obtener información sobre cómo se aplican las preferencias de grupo a las nuevas plantillas, consulte <a href="#how-preferences-apply-to-templates-and-template-tasks" class="MCXref xref">Cómo se aplican las preferencias a las plantillas y tareas de plantilla</a> en este artículo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Editar una o más plantillas</td> 
      <td> <p>Seleccione al menos una plantilla, haga clic en el icono Editar <img src="assets/edit-icon.png"> y, a continuación, utilice cualquiera de las opciones disponibles para configurarla. Para obtener información acerca de estas opciones, vea <a href="../../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Editar plantillas de proyecto</a>.</p> <p>El icono Editar solo está disponible si tiene acceso de edición a todas las plantillas seleccionadas. Para obtener información sobre este acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Conceder acceso a las plantillas</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Eliminar una o más plantillas</td> 
      <td> <p>Seleccione al menos una plantilla y luego haga clic en el icono Eliminar <img src="assets/delete.png">.</p> <p>Este icono solo está disponible si tiene acceso de edición a todas las plantillas seleccionadas. Para obtener información sobre este acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Conceder acceso a las plantillas</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Compartir una o más plantillas</td> 
      <td> <p>Seleccione al menos una plantilla, haga clic en el icono Compartir <img src="assets/share-icon.png"> y, a continuación, haga clic en una de las siguientes opciones del menú desplegable:</p> 
       <ul> 
        <li> <p><strong>Plantilla</strong>: en el cuadro <strong>Acceso a plantillas</strong> que aparece, agregue nombres para especificar a quién desea tener acceso a la propia plantilla.</p> <p>Para obtener más información, vea la sección <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md#share" class="MCXref xref">Compartir una plantilla</a> en el artículo <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md" class="MCXref xref">Compartir plantillas de proyecto</a>.</p> </li> 
        <li><strong>Proyecto</strong>: en el cuadro <strong>Acceso al proyecto</strong> que aparece, agregue nombres para especificar a quién desea tener acceso a los proyectos creados a partir de la plantilla</li> 
       </ul> <p>El icono Compartir solo está disponible si tiene acceso de uso compartido a todas las plantillas que seleccione. Para obtener información sobre este acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Conceder acceso a las plantillas</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exportar la lista de plantillas</td> 
      <td>Haga clic en <strong>Exportar</strong> <img src="assets/export.png"> y, a continuación, seleccione el formato de archivo que desee para la lista exportada.</td> 
     </tr> 
    </tbody> 
   </table>

## Cómo se aplican las preferencias a las plantillas y tareas de plantilla {#how-preferences-apply-to-templates-and-template-tasks}

Al crear una plantilla de proyecto, la configuración que se muestra en las tablas siguientes se establece automáticamente mediante una preferencia de proyecto o tarea relacionada.

>[!NOTE]
>
>Las preferencias de proyecto o tarea de nivel de grupo o de nivel de sistema afectan a una plantilla de proyecto, dependiendo de si la ha asociado a un grupo cuando la creó.
>
>Si lo asoció a un grupo, la preferencia de nivel de grupo surte efecto. Esto ocurre en los siguientes casos:
>
>* La plantilla se crea desde el área Grupos, como se explica en este artículo
>* Especifique un grupo al crear la plantilla mediante un archivo de KickStart
>* Especifique un grupo al crear la plantilla mediante la API
>
>Si no ha asociado la nueva plantilla con un grupo, la preferencia de nivel de sistema tiene efecto. Esto ocurre en los casos siguientes. (Si posteriormente asigna un grupo a la plantilla o tarea de plantilla, las preferencias del grupo no le afectan).
>
>* La plantilla se crea desde el área Plantillas
>* No se especifica un grupo al crear la plantilla mediante un archivo de KickStart
>* No se especifica un grupo al crear la plantilla mediante la API
>

* [Configuración de plantillas de proyecto configurada por preferencias de proyecto y tarea](#project-template-settings-configured-by-project-and-task-preferences)
* [Configuración de tarea de plantilla configurada por preferencias de tarea](#template-task-settings-configured-by-task-preferences)

### Configuración de plantillas de proyecto configurada por preferencias de proyecto y tarea {#project-template-settings-configured-by-project-and-task-preferences}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Método de índice de rendimiento</p> </td> 
   <td> <p>Configurado por la preferencia de proyecto de nivel de grupo "Método de índice de rendimiento" si asocia la nueva plantilla con un grupo, o la misma preferencia de proyecto de nivel de sistema si no lo hace.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Tipo de condición</p> </td> 
   <td> <p>Configurado por la preferencia de proyecto de nivel de grupo "Establecer automáticamente la condición del proyecto en función del estado de progreso" si asocia la nueva plantilla a un grupo o la misma preferencia de proyecto de nivel de sistema si no lo hace.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Programar desde</p> </td> 
   <td> <p>Configurado por la preferencia de proyecto de nivel de grupo "Programar desde" si asocia la nueva plantilla con un grupo, o la misma preferencia de proyecto de nivel de sistema si no lo hace.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Tiempo libre del usuario</p> </td> 
   <td> <p>Configurado por la preferencia de proyecto de nivel de grupo "Tiempo libre del usuario" si asocia la nueva plantilla con un grupo, o la misma preferencia de proyecto de nivel de sistema si no lo hace.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Tipo de actualización</p> </td> 
   <td> <p>Configurado por la preferencia de proyecto de nivel de grupo "Las escalas de tiempo del proyecto se volverán a calcular automáticamente" si asocia la nueva plantilla con un grupo o la misma preferencia de proyecto de nivel de sistema si no lo hace.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Configuración de sección de acceso</p> </td> 
   <td> <p>Configurado por las preferencias de tareas de nivel de grupo en la sección "Acceso" si asocia la nueva plantilla a un grupo o la misma preferencia de proyecto de nivel de sistema si no lo hace.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener información acerca de las preferencias de proyecto enumeradas en esta tabla, vea [Configurar preferencias de proyecto para todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Para obtener información sobre la preferencia de tareas y problemas, consulte [Configurar las preferencias de tareas y problemas en todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>* Si cambia el grupo asociado a una plantilla de proyecto existente, la configuración de la plantilla será la misma.
>* Si mueve una tarea de plantilla existente a otra plantilla, la siguiente configuración permanece sin cambios en la tarea de plantilla, independientemente del grupo asociado a la nueva plantilla:>
>   * Tipo de duración
>   * Tipo de ingresos
>   * Tipo de costo
>
>  Sin embargo, la tarea de plantilla se ve afectada por la configuración &quot;Cuando se asigna a alguien a una tarea&quot; en la nueva plantilla. Para obtener más información, consulte la sección [Acceso](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#access) en el artículo [Editar plantillas de proyecto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).
>
>* Cuando un administrador guarda un proyecto como plantilla, todos los ajustes de la plantilla se heredan del proyecto, incluido el grupo.
>
>  Cuando un administrador convierte una tarea o un problema en un proyecto mediante una plantilla, todos los ajustes de la plantilla están determinados por lo que ya se ha guardado en la plantilla.
>

### Configuración de tarea de plantilla configurada por preferencias de tarea {#template-task-settings-configured-by-task-preferences}

Al crear una tarea de plantilla, algunos de sus ajustes se configuran automáticamente mediante una preferencia de tarea de correlación. Esta configuración se enumera en la tabla siguiente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Tipo de duración </p> </td> 
   <td> <p>Configurado por la preferencia de tarea de nivel de grupo "Tipo de duración" si asocia la plantilla a un grupo, o la misma preferencia de tarea y problema de nivel de sistema si no lo hace.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Tipo de ingresos</p> </td> 
   <td> <p>Configurado por la preferencia de tarea de nivel de grupo "Tipo de ingresos" si asocia la plantilla a un grupo, o la misma preferencia de tarea y problema de nivel de sistema si no lo hace.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Tipo de costo </p> </td> 
   <td> <p> Configurado por la preferencia de tarea de nivel de grupo "Tipo de coste" si asocia la plantilla a un grupo, o la misma preferencia de tarea y problema de nivel de sistema si no lo hace.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener información acerca de las preferencias de tareas que se enumeran en esta tabla, consulte [Configurar las preferencias de tareas y problemas en todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
