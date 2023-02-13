---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Bloquear o desbloquear las preferencias del proyecto para todos los grupos del sistema
description: Los grupos de su organización pueden necesitar una preferencia de proyecto configurada de forma diferente para sus flujos de trabajo únicos. Puede desbloquear la preferencia de todos los grupos en toda la organización para que puedan configurarla por su cuenta.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f5a94eaf-ebb8-424b-80ff-ba40cc985a6e
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 0%

---

# Bloquear o desbloquear las preferencias del proyecto para todos los grupos del sistema

Los grupos de su organización pueden necesitar una preferencia de proyecto configurada de forma diferente para sus flujos de trabajo únicos. Puede desbloquear la preferencia de todos los grupos en toda la organización para que puedan configurarla por su cuenta.

Cuando se desbloquea una preferencia y el administrador del grupo la modifica, los proyectos asociados al grupo adquieren la configuración de dicha preferencia desde la configuración de nivel de grupo en lugar de desde la configuración de nivel de sistema.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser [!DNL Workfront] administrador.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Acerca de las preferencias bloqueadas y desbloqueadas

Bloquear un proyecto, tarea o preferencia de problema que haya configurado a nivel de sistema garantiza que todos usen la misma configuración para esa preferencia. Aunque aún puede volver a configurar una preferencia que bloquee, los administradores de grupos no podrán reconfigurarla para sus grupos.

Por el contrario, al desbloquear un proyecto, una tarea o una preferencia de problemas, los administradores de grupos pueden disponer de más flexibilidad para administrar la forma en que sus grupos trabajan con esos elementos. Cuando se desbloquea una preferencia, los administradores del grupo pueden volver a configurarla para sus grupos.

Para obtener instrucciones sobre cómo bloquear o desbloquear un proyecto, una tarea o una preferencia de emisión a nivel de sistema, consulte [Configurar las preferencias de problemas y tareas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>Después de un [!DNL Workfront] administrador desbloquea una preferencia a nivel de sistema, cualquier administrador de grupo puede configurarla y luego bloquearla para asegurarse de que todos los miembros de su grupo y los subgrupos siguientes usen la misma configuración. Esto es paralelo a la capacidad de que una [!DNL Workfront] El administrador debe configurar y bloquear una preferencia para todos los miembros del sistema. Para obtener más información, consulte [Configuración de las preferencias de un proyecto para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) y [Bloquear o desbloquear un proyecto, tarea o preferencia de problemas para subgrupos](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

## Desbloquear preferencias de proyecto para que los grupos puedan configurarlo

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. Haga clic en **[!UICONTROL Preferencias de proyecto]** y haga clic en **[!UICONTROL Proyectos]**.

1. Realice una de las siguientes acciones:

   * Si desea que los administradores del grupo puedan configurar una preferencia para sus grupos, desbloquéela ![](assets/unlock-toggle-button.png).
   * Si desea que todos los grupos utilicen la configuración para una preferencia, asegúrese de que esté bloqueada (este es el valor predeterminado).

      >[!IMPORTANT]
      >
      >Le recomendamos que se comunique con los administradores y usuarios en grupos de todo el sistema para asegurarse de que todas las necesidades se tienen en cuenta de la forma en que configura una preferencia bloqueada. Cuando lo bloquea, la configuración para él la heredan todos los grupos del sistema. Y si la preferencia se ha desbloqueado durante cualquier periodo de tiempo, la configuración sustituye a las que pueden haber realizado los administradores del grupo.

1. Haga clic en **[!UICONTROL Guardar]**.
