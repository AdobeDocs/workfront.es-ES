---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Reordenar estados de grupo
description: Como administrador de grupo, puede cambiar el orden de los estados de proyecto, tarea y problema de un grupo que administre.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 0cdb4d10-7792-4140-8dec-ef805f668f90
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 7%

---

# Reordenar estados de grupo

Como administrador de grupo, puede cambiar el orden de los estados de proyecto, tarea y problema de un grupo que administre.

<!--
The system version of this snippet mentions a single group because a sysadmin call also reorder statuses there. Group admin version of this article is still needed.
-->

![](assets/statuses.png)

Si hay grupos por encima del grupo que administra, sus administradores también pueden hacerlo en su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

>[!NOTE]
>
>* Un administrador de Workfront puede reordenar los estados en el nivel del sistema. Esto no afecta al orden de los estados dentro de los grupos.
>
>  Sin embargo, los estados de un grupo de nivel superior recién creado heredan el orden de los estados de nivel del sistema. (Un nuevo subgrupo hereda el orden de los estados del grupo que se encuentra un nivel por encima).
>
>* Puede reordenar los estados bloqueados. Para obtener información acerca de los estados bloqueados, vea [Crear o editar un estado de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

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
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Nuevo: estándar</p>
       <p>O</p>
       <p>Actual: plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>Debe ser administrador de grupo del grupo o administrador del sistema.</td>
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
     <p>Al día</p> 
     <p>Inactivo</p> 
     <p> En espera </p> 
     <p> Planificación </p> 
     <p> Completar </p> 
     <p> Solicitud </p> 
     <p> Aprobado </p> 
     <p> Rechazado </p> 
     <p> Idea </p> 
   </td> 
   <td> 
     <p>Nuevo</p> 
     <p>En curso</p> 
     <p>Completar</p> 
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

## Reordenar los estados de las tareas y proyectos de un grupo que administra

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Grupos** y, a continuación, haga clic en el nombre del grupo.
1. En el panel izquierdo, haga clic en **Estados**.
1. Sobre la lista Estados que se muestra, haga clic en la ficha **Proyectos** o **Tareas**.

1. Arrastre y suelte los estados en el orden que desee.

   El nuevo orden de estado se guarda automáticamente.

1. Para probar el nuevo orden de estado, vaya a una tarea o proyecto asociado al grupo, haga clic en el estado en la esquina superior derecha y asegúrese de que los estados que se muestran están en el orden configurado.

## Reordenar estados para problemas

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Grupos** y, a continuación, haga clic en el nombre del grupo.
1. En el panel izquierdo, haga clic en **Estados**.
1. Haga clic en la ficha **Problemas**.
1. (Opcional) Seleccione un tipo de problema (**Informe de errores**, **Pedido de cambio**, **Problema** o **Solicitud**).

   >[!NOTE]
   >
   >* No se puede personalizar el orden de los estados de la lista maestra.
   >* Le recomendamos que ordene los estados para cada tipo de problema de la misma manera. Para obtener más información sobre los tipos de problemas, consulte [Configurar tipos de solicitudes](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Arrastre y suelte los estados en el orden que desee.

   El nuevo orden de estado se guarda automáticamente.

1. Para probar el nuevo orden de estado, vaya a un problema asociado con el grupo, haga clic en el estado en la esquina superior derecha y asegúrese de que los estados que se muestran están en el orden configurado.
