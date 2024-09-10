---
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Reordenar los estados de grupo y de nivel de sistema
description: Como administrador de Workfront, puede cambiar el orden de los estados de proyectos, tareas y problemas para todos los miembros del sistema o para un solo grupo.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6fee45a6-1a55-4351-8b08-88244c742ed5
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 6%

---

# Reordenar los estados de grupo y de nivel del sistema

Como administrador de Workfront, puede cambiar el orden de los estados de proyectos, tareas y problemas para todos los miembros del sistema o para un solo grupo.

<!--The system version of this snippet mentions a single group because a sysadmin call also reorder statuses there. Group admin version of this article is still needed.-->

![](assets/statuses.png)

>[!NOTE]
>
>* Reordenar los estados en el nivel del sistema no afecta al orden de los estados dentro de los grupos.
>
>  Sin embargo, los estados de un grupo de nivel superior recién creado heredan el orden de los estados de nivel del sistema. (Un nuevo subgrupo hereda el orden de los estados del grupo que se encuentra un nivel por encima).
>
>* Puede reordenar los estados bloqueados. Para obtener información acerca de los estados bloqueados, vea [Crear o editar un estado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
>* Los administradores de grupo también pueden reordenar los estados utilizados en sus grupos. Para obtener más información, vea [Reordenar estados de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/reorder-group-statuses-from-groups-area.md).
>

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
     <p>Nuevo: estándar</p>
     <p>o</p>
     <p>Actual: plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL Administrador del sistema]</td>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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
    <ul> 
     <li>Al día</li> 
     <li>Inactivo</li> 
     <li> En espera </li> 
     <li> Planificación </li> 
     <li> Completar </li> 
     <li> Solicitud </li> 
     <li> Aprobado </li> 
     <li> Rechazado </li> 
     <li> Idea </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>Nuevo</li> 
     <li>En curso</li> 
     <li>Completar</li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>Nuevo</li> 
     <li>En curso</li> 
     <li>Vuelto a abrir</li> 
     <li>Esperando comentarios</li> 
     <li>En espera</li> 
     <li>No se puede duplicar</li> 
     <li>Cerrado</li> 
     <li>Resuelto</li> 
     <li>Verificación completa</li> 
     <li>No se puede resolver</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Reordenar estados para tareas y proyectos de todo el sistema o para un grupo

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Preferencias de proyecto > Estados**.
1. (Condicional) Si va a reordenar los estados de un grupo, empiece a escribir el nombre del grupo en el cuadro de la esquina superior derecha y, a continuación, haga clic en el nombre cuando aparezca.

   ![](assets/system-statuses-in-upper-rt-corner-group.jpg)

1. Sobre la lista Estados que se muestra, haga clic en la ficha **Proyectos** o **Tareas**.

1. Arrastre y suelte los estados en el orden que desee.

   El nuevo orden de estado se guarda automáticamente.

1. Para probar el nuevo orden de estado, vaya a una tarea o proyecto, haga clic en el estado en la esquina superior derecha y asegúrese de que los estados que se muestran están en el orden configurado.

## Reordenar estados para problemas

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y, a continuación, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. Haga clic en **Preferencias de proyecto > Estados.**
1. (Condicional) Si va a reordenar los estados de un grupo, empiece a escribir el nombre del grupo en el cuadro de la esquina superior derecha y, a continuación, haga clic en el nombre cuando aparezca.

   ![](assets/issue-statuses-group-name.png)

1. Haga clic en la ficha **Problemas**.
1. (Opcional) Seleccione un tipo de problema (**Informe de errores**, **Pedido de cambio**, **Problema** o **Solicitud**).

   >[!NOTE]
   >
   >* No se puede personalizar el orden de los estados de la lista maestra.
   >* Le recomendamos que ordene los estados para cada tipo de problema de la misma manera. Para obtener más información sobre los tipos de problemas, consulte [Configurar tipos de solicitudes](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Arrastre y suelte los estados en el orden que desee.

   El nuevo orden de estado se guarda automáticamente.

1. Para probar el nuevo orden de estado, vaya a un problema, haga clic en el estado en la esquina superior derecha y asegúrese de que los estados que se muestran estén en el orden configurado.
