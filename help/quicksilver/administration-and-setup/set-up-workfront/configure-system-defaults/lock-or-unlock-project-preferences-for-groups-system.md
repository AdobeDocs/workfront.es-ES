---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Bloquear o desbloquear las preferencias de proyecto de todos los grupos del sistema
description: Es posible que los grupos de su organización necesiten una preferencia de proyecto configurada de forma diferente para sus flujos de trabajo únicos. Puede desbloquear la preferencia de todos los grupos de la organización para que puedan configurarla ellos mismos.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f5a94eaf-ebb8-424b-80ff-ba40cc985a6e
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 96%

---

# Bloquear o desbloquear las preferencias de proyecto de todos los grupos del sistema

Es posible que los grupos de su organización necesiten una preferencia de proyecto configurada de forma diferente para sus flujos de trabajo únicos. Puede desbloquear la preferencia de todos los grupos de la organización para que puedan configurarla ellos mismos.

Cuando una preferencia está desbloqueada y el administrador de grupos la modifica, los proyectos asociados al grupo adquieren la configuración de dicha preferencia desde la configuración a nivel de grupo en lugar de hacerlo desde la configuración a nivel de sistema.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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
   <td><p>Nuevo: [!UICONTROL Standard]</p>
   O
   <p>Actual: [!UICONTROL Plan]</p>
   </td> 
  </tr>
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td>
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Acerca de las preferencias bloqueadas y desbloqueadas

Bloquear una preferencia de proyecto, tarea o problema que haya configurado a nivel del sistema garantiza que todos utilicen la misma configuración para esa preferencia. Aunque puede volver a configurar una preferencia que haya bloqueado, los administradores de grupos no podrán volver a configurarla para sus grupos.

Por el contrario, si se desbloquean las preferencias de un proyecto, tarea o problema, los administradores de grupos tendrán más flexibilidad para administrar el modo en que sus grupos trabajan con esos elementos. Cuando una preferencia está desbloqueada, los administradores de grupos pueden volver a configurarla para sus grupos.

Si un campo no tiene un conmutador de bloqueo/desbloqueo, no se puede desbloquear para que los administradores de grupos configuren las opciones a nivel de grupo. La configuración solo está disponible a nivel del sistema.

Para obtener instrucciones sobre el bloqueo o desbloqueo de una preferencia de proyecto, tarea o problema a nivel de sistema, consulte [Configurar las preferencias de tareas y problemas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>Después de que un administrador de [!DNL Workfront] desbloquee una preferencia a nivel del sistema, cualquier administrador de grupos puede configurarla y después bloquearla para asegurarse de que todos los miembros de su grupo y de los subgrupos que se muestran a continuación usan la misma configuración. Esto es equivalente a la posibilidad que un administrador de [!DNL Workfront] tiene para configurar y bloquear una preferencia para todas las personas del sistema. Para obtener más información, consulte [Configurar las preferencias de proyecto para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) y [Bloquear o desbloquear una preferencia de proyecto, tarea o problema para subgrupos](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

## Desbloquear una preferencia de proyecto para que los grupos puedan configurarla

{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Preferencias del proyecto]** y, a continuación, haga clic en **[!UICONTROL Proyectos]**.

1. Realice una de las siguientes acciones:

   * Si desea que los administradores de grupo puedan configurar una preferencia para sus grupos, desbloquéela ![Desbloquear opción](assets/unlock-toggle-button.png).
   * Si desea que todos los grupos utilicen su configuración para una preferencia, asegúrese de que esté bloqueada (es el valor predeterminado).

     >[!IMPORTANT]
     >
     >Le recomendamos que se comunique con los administradores y usuarios de los grupos de todo el sistema para asegurarse de tener en cuenta todas las necesidades a la hora de configurar una preferencia bloqueada. Cuando la bloquea, su configuración se hereda por todos los grupos del sistema. Y si la preferencia ha estado desbloqueada durante algún tiempo, su configuración reemplaza aquellas que los administradores de grupo puedan haber realizado.

1. Haga clic en **[!UICONTROL Guardar]**.
