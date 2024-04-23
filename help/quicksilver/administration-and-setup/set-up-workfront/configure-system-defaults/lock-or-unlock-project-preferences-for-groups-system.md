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
source-git-commit: 3e97df265df83965d094d8723fe76043ff4af80e
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---

# Bloquear o desbloquear las preferencias de proyecto de todos los grupos del sistema

Es posible que los grupos de su organización necesiten una preferencia de proyecto configurada de forma diferente para sus flujos de trabajo únicos. Puede desbloquear la preferencia de todos los grupos de la organización para que puedan configurarla ellos mismos.

Cuando una preferencia está desbloqueada y el administrador del grupo la modifica, los proyectos asociados con el grupo adquieren la configuración de dicha preferencia desde la configuración de nivel de grupo en lugar de desde la configuración de nivel de sistema.

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
   <td> <p>Debe ser un [!DNL Workfront] administrador.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo [!DNL Workfront] El administrador puede modificar su nivel de acceso. Consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Acerca de las preferencias bloqueadas y desbloqueadas

Bloquear una preferencia de proyecto, tarea o problema que haya configurado en el sistema garantiza que todos utilicen la misma configuración para esa preferencia. Aunque puede volver a configurar una preferencia que haya bloqueado, los administradores de grupos no podrán volver a configurarla para sus grupos.

Por el contrario, si se desbloquean las preferencias de un proyecto, tarea o problema, los administradores de grupos tendrán más flexibilidad para administrar el modo en que sus grupos trabajan con esos elementos. Cuando una preferencia está desbloqueada, los administradores de grupos pueden volver a configurarla para sus grupos.

Si un campo no tiene la opción de bloqueo/desbloqueo, no se puede desbloquear para que los administradores de grupo configuren las opciones en el nivel de grupo. La configuración solo está disponible en el sistema.

Para obtener instrucciones sobre cómo bloquear o desbloquear un proyecto, una tarea o una preferencia de problema en el nivel del sistema, consulte [Configurar las preferencias de tareas y problemas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>Después de un [!DNL Workfront] Un administrador desbloquea una preferencia en el sistema. Cualquier administrador de grupo puede configurarla y, a continuación, bloquearla para garantizar que todos los miembros de su grupo y de los subgrupos siguientes utilicen la misma configuración. Esto es paralelo a la capacidad de que un [!DNL Workfront] El administrador de debe configurar y bloquear una preferencia para todos los usuarios del sistema. Para obtener más información, consulte [Configurar las preferencias de proyecto de un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) y [Bloquear o desbloquear una preferencia de proyecto, tarea o problema para subgrupos](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

## Desbloquear una preferencia de proyecto para que los grupos puedan configurarla

1. Haga clic en **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront], luego haga clic en **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. Clic **[!UICONTROL Preferencias de proyecto]**, luego haga clic en **[!UICONTROL Proyectos]**.

1. Realice una de las siguientes acciones:

   * Si desea que los administradores de grupo puedan configurar una preferencia para sus grupos, desbloquéela ![](assets/unlock-toggle-button.png).
   * Si desea que todos los grupos utilicen su configuración para una preferencia, asegúrese de que esté bloqueada (este es el valor predeterminado).

     >[!IMPORTANT]
     >
     >Le recomendamos que se comunique con los administradores y usuarios de los grupos de todo el sistema para asegurarse de que todas las necesidades se tienen en cuenta de la forma en que configura una preferencia bloqueada. Cuando lo bloquea, la configuración para él la heredan todos los grupos del sistema. Y si la preferencia se ha desbloqueado durante cualquier período de tiempo, la configuración reemplaza las que los administradores del grupo puedan haber realizado.

1. Haga clic en **[!UICONTROL Guardar]**.
