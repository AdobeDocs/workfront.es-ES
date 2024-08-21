---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-groups
title: Mover un grupo
description: Puede mover un grupo a otro grupo que administre.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f5227454-457d-40d3-865c-c2551471d83e
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 1%

---

# Mover un grupo

Puede mover un grupo a otro grupo que administre.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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

+++

## Mover un grupo a otro grupo

>[!NOTE]
>
>Si los estados del grupo movido están bloqueados, heredará los estados del nuevo grupo principal.
>
>Si los estados del grupo movido son desbloqueados, no heredará los estados de su nuevo grupo padre, ni el nuevo grupo padre adoptará sus estados.
>
>Para obtener más información acerca de los estados de grupo, vea [Crear o editar un estado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) y [Crear o editar un estado de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Grupos** ![](assets/groups-icon.png).

1. Seleccione el grupo de destino al que desea mover el grupo y haga clic en el icono Editar ![](assets/edit-icon.png).
1. En el cuadro **Editar grupo** que aparece, en **Miembros del grupo y Administradores del grupo**, empiece a escribir el nombre del grupo que desea mover y, a continuación, haga clic en él cuando aparezca.
1. Haga clic en **Guardar**.

>[!TIP]
>
>También puede convertir un subgrupo en un grupo de nivel superior. Para obtener instrucciones, vea la sección [Quitar un subgrupo de su grupo principal y convertirlo en un grupo de nivel superior](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) en el artículo [Administrar un subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
