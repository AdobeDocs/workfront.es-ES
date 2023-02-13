---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Eliminar un estado personalizado
description: Puede eliminar un estado de sistema personalizado si ya no resulta útil para su organización.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 73c4eb87-94f6-47bf-b447-eb02a703f7ef
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 1%

---

# Eliminar un estado personalizado

Puede eliminar un estado de sistema personalizado si ya no resulta útil para su organización.

Si el estado está bloqueado o desbloqueado determina si se elimina el estado de todos los grupos del sistema:

* Cuando se elimina un estado del sistema que está bloqueado actualmente, se elimina el estado de todos los grupos del sistema, independientemente de si el grupo lo ha renombrado o no.
* Por el contrario, cuando se elimina un estado del sistema que está actualmente desbloqueado, el estado se mantiene para todos los grupos del sistema.


>[!NOTE]
>
>No puede eliminar lo siguiente:
>
>* Estado del sistema bloqueado o desbloqueado utilizado en un proceso de aprobación del sistema que actualmente está pendiente de aprobación para al menos un objeto del sistema.
>
>  Sin embargo, puede eliminar un estado del sistema desbloqueado que se utilice en un proceso de aprobación de un solo uso o de nivel de grupo que esté pendiente de aprobación.
>
>  Puede ejecutar un informe para buscar los objetos, resolver las aprobaciones pendientes e intentar de nuevo eliminar el estado. Para obtener instrucciones, consulte [Enumerar objetos con procesos de aprobación pendientes con un estado determinado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/list-objects-pending-approval-certain-status.md).
>
>* Estados utilizados en procesos de aprobación que actualmente están pendientes de aprobación para al menos un objeto del sistema.


Para obtener instrucciones sobre la eliminación de un estado de grupo, consulte [Eliminar un estado de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/delete-a-group-status.md).

## Requisitos de acceso

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Eliminar un estado de sistema personalizado

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Preferencias de proyecto** > **Estados**.

1. Para eliminar el estado en todo el sistema (incluso para grupos individuales), pase el ratón sobre el estado y haga clic en **Editar** y, a continuación, asegúrese de que **Bloqueo para todos los grupos** está seleccionado. Haga clic en **Guardar**.

   O

   Para eliminar el estado del sistema pero conservarlo para grupos individuales, pase el ratón sobre el estado y haga clic en **Editar** y, a continuación, asegúrese de que **Bloqueo para todos los grupos** no está seleccionado. Haga clic en **Guardar**.

1. Pase el ratón sobre el estado que quiera eliminar y haga clic en **Eliminar**.
1. En el mensaje que aparece, haga clic en **Eliminar estado**.
1. En el **Eliminar estado** que aparece, seleccione un estado en el campo etiquetado **Defina todos los proyectos que tengan este estado en**.

   Los proyectos que utilizaban el estado que está eliminando se establecen en el estado que seleccione.

   Los estados están disponibles en la lista desplegable solo si coinciden con el mismo estado que el estado que está eliminando.

   Por ejemplo, si está eliminando un estado que coincide con Actual, solo los estados que también se equiparan con Actual estarán disponibles para seleccionarlos.

1. Haga clic en **Eliminar estado**.
