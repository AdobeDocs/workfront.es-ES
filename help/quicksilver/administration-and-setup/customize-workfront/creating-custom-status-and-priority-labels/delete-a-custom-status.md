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

Si el estado es bloqueado o desbloqueado, determina si el estado se elimina para todos los grupos del sistema:

* Cuando se elimina un estado del sistema que está bloqueado actualmente, el estado se elimina para todos los grupos del sistema, independientemente de si el grupo le ha cambiado el nombre.
* Por el contrario, cuando se elimina un estado del sistema que está desbloqueado actualmente, el estado permanece para todos los grupos del sistema.


>[!NOTE]
>
>No puede eliminar lo siguiente:
>
>* Estado del sistema bloqueado o desbloqueado utilizado en un proceso de aprobación del sistema que está actualmente pendiente de aprobación para al menos un objeto del sistema.
>
>  Sin embargo, puede eliminar un estado de sistema desbloqueado utilizado en un proceso de aprobación de un solo uso o de nivel de grupo que esté pendiente de aprobación en ese momento.
>
>  Puede ejecutar un informe para buscar los objetos, resolver las aprobaciones pendientes y, a continuación, intentar de nuevo eliminar el estado. Para obtener instrucciones, vea [Enumerar objetos con procesos de aprobación pendientes que utilizan un estado determinado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/list-objects-pending-approval-certain-status.md).
>
>* Estados utilizados en los procesos de aprobación que están actualmente pendientes de aprobación para al menos un objeto del sistema.

Para obtener instrucciones sobre cómo eliminar un estado de grupo, consulte [Eliminar un estado de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/delete-a-group-status.md).

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
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Eliminar un estado de sistema personalizado

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y, a continuación, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Preferencias de proyecto** > **Estados**.

1. Para eliminar el estado en todo el sistema (incluidos los grupos individuales), pasa el ratón sobre el estado, haz clic en **Editar** y asegúrate de que la opción **Bloquear para todos los grupos** está seleccionada. Haga clic en **Guardar**.

   O

   Para eliminar el estado del sistema pero conservarlo para grupos individuales, pasa el ratón sobre el estado, haz clic en **Editar** y, a continuación, asegúrate de que la opción **Bloquear para todos los grupos** no esté seleccionada. Haga clic en **Guardar**.

1. Pase el ratón sobre el estado que quiera eliminar y luego haga clic en **Eliminar**.
1. En el mensaje que aparece, haga clic en **Eliminar estado**.
1. En el cuadro **Eliminar estado** que se muestra, seleccione un estado en el campo denominado **Establecer todos los proyectos actualmente con este estado en**.

   Los proyectos que utilizaban el estado que está eliminando se establecen en el estado que seleccione.

   Los estados solo están disponibles en la lista desplegable si coinciden con el mismo estado que el estado que está eliminando.

   Por ejemplo, si elimina un estado que es igual a Actual, solo se pueden seleccionar los estados que también son iguales a Actual.

1. Haga clic en **Eliminar estado**.
