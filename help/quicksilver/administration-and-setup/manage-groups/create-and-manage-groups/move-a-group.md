---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-groups
title: Mover un grupo
description: Puede mover un grupo debajo de otro grupo que administre.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f5227454-457d-40d3-865c-c2551471d83e
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 84%

---

# Mover un grupo

Puede mover un grupo debajo de otro grupo que administre.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
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

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Mover un grupo debajo de otro grupo

>[!NOTE]
>
>Si los estados del grupo movido están bloqueados, heredará los estados del nuevo grupo principal.
>
>Si se desbloquean los estados del grupo movido, no heredará los estados de su nuevo grupo principal, ni el nuevo grupo principal adoptará sus estados.
>
>Para obtener más información acerca de los estados de grupo, consulte [Crear o editar un estado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) y [Crear o editar un estado de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Grupos** ![Grupos](assets/groups-icon.png).

1. Seleccione el grupo de destino al que desea mover el grupo y haga clic en el icono Editar ![icono Editar](assets/edit-icon.png).
1. En el cuadro **Editar grupo** que aparece, debajo de **Miembros del grupo y Administradores del grupo**, empiece a escribir el nombre del grupo que desea mover y, a continuación, haga clic en él cuando aparezca.
1. Haga clic en **Guardar**.

>[!TIP]
>
>También puede convertir un subgrupo en un grupo de nivel superior. Para obtener instrucciones, consulte la sección [Quitar un subgrupo de su grupo principal y convertirlo en un grupo de nivel superior](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) en el artículo [Administrar un subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
