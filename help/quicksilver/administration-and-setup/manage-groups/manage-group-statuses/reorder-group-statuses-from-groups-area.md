---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Reordenar estados de grupos
description: Como administrador de grupo, puede cambiar el orden de los estados de proyecto, tarea y problema de un grupo que administra.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 0cdb4d10-7792-4140-8dec-ef805f668f90
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 6%

---

# Reordenar estados de grupos

Como administrador de grupo, puede cambiar el orden de los estados de proyecto, tarea y problema de un grupo que administra.

<!--
The system version of this snippet mentions a single group because a sysadmin call also reorder statuses there. Group admin version of this article is still needed.
-->

![](assets/statuses.png)

Si hay algún grupo por encima del grupo que administra, sus administradores también pueden hacerlo por su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

>[!NOTE]
>
>* Un administrador de Workfront puede reordenar los estados a nivel del sistema. Esto no afecta al orden de los estados dentro de los grupos.
>
>  Sin embargo, los estados de un grupo de nivel superior creado recientemente heredan el orden de los estados de nivel del sistema. (Un nuevo subgrupo hereda el orden de los estados del grupo un nivel superior).
>
>* Puede reordenar los estados bloqueados. Para obtener información sobre los estados bloqueados, consulte [Crear o editar un estado de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
>


## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront* </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConditions-wf-groups.groups"> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Debe ser administrador de grupo del grupo o administrador de Workfront. Para obtener más información, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupo</a> y <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Si necesita saber qué plan o tipo de licencia tiene, póngase en contacto con el administrador de Workfront.

## Orden predeterminado de los estados

De forma predeterminada, los estados se muestran en el siguiente orden:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th width="33.33%">Proyecto</th> 
   <th width="33.33%">Tarea</th> 
   <th width="33.33%">Problema</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
     <p>Al día</p> 
     <p>Inactivo</p> 
     <p> En espera </p> 
     <p> Planificación </p> 
     <p> Finalizadas </p> 
     <p> Solicitado </p> 
     <p> Aprobado </p> 
     <p> Rechazado </p> 
     <p> Idea </p> 
   </td> 
   <td> 
     <p>Nuevo</p> 
     <p>En curso</p> 
     <p>Finalizadas</p> 
   </td> 
   <td> 
     <p>Nuevo</p> 
     <p>En curso</p> 
     <p>Vuelto a abrir</p> 
     <p>Esperando comentarios</p> 
     <p>En espera</p> 
     <p>No se puede duplicar</p> 
     <p>Cerrado</p> 
     <p>Resuelto</p> 
     <p>Verificación completa</p> 
     <p>No se puede resolver</p> 
   </td> 
  </tr> 
 </tbody> 
</table>

## Reordenar estados para tareas y proyectos en un grupo que administra

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Grupos** y, a continuación, haga clic en el nombre del grupo.
1. En el panel izquierdo, haga clic en **Estados**.
1. Sobre la lista Estados que se muestra, haga clic en el botón **Proyectos** o **Tareas** pestaña .

1. Arrastre y suelte los estados en el orden que desee.

   El nuevo orden de estado se guarda automáticamente.

1. Para probar el nuevo orden de estado, vaya a una tarea o proyecto asociado al grupo, haga clic en el estado en la esquina superior derecha y asegúrese de que los estados que se muestran estén en el orden configurado.

## Reordenar estados por problemas

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Grupos** y, a continuación, haga clic en el nombre del grupo.
1. En el panel izquierdo, haga clic en **Estados**.
1. Haga clic en el **Problemas** pestaña .
1. (Opcional) Seleccione un tipo de problema (**Informe de errores**, **Cambiar orden**, **Problema** o **Solicitud**).

   >[!NOTE]
   >
   >* No se puede personalizar el orden de los estados de la lista maestra.
   >* Le recomendamos que ordene los estados de cada tipo de problema del mismo modo. Para obtener más información sobre los tipos de problemas, consulte [Configurar tipos de solicitud](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).


1. Arrastre y suelte los estados en el orden que desee.

   El nuevo orden de estado se guarda automáticamente.

1. Para probar el nuevo orden de estado, vaya a un problema asociado con el grupo, haga clic en el estado en la esquina superior derecha y asegúrese de que los estados que se muestran estén en el orden configurado.
