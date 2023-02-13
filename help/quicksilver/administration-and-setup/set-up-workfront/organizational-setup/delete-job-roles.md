---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Eliminar funciones de trabajo
description: Puede eliminar las funciones de trabajo que su organización ya no utilice. Se recomienda no eliminar las funciones de trabajo si se han asociado con elementos de trabajo en el pasado. Para conservar toda la información histórica sobre las asignaciones de trabajo, se recomienda desactivar las funciones en lugar de eliminarlas cuando queden obsoletas. Para obtener información sobre la desactivación de funciones, consulte Desactivación de funciones de trabajo.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b0e81d76-5227-4fda-9a58-68fbce3f5b94
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 0%

---

# Eliminar funciones de trabajo

Puede eliminar las funciones de trabajo que su organización ya no utilice. Se recomienda no eliminar las funciones de trabajo si se han asociado con elementos de trabajo en el pasado.

Para conservar toda la información histórica sobre las asignaciones de trabajo, se recomienda desactivar las funciones en lugar de eliminarlas cuando queden obsoletas. Para obtener información sobre la desactivación de funciones, consulte [Desactivar funciones de trabajo](../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso administrativo a las funciones de trabajo</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Eliminar una función de trabajo

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved from create and manage job roles)</p>
-->

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. Haga clic en **[!UICONTROL Funciones del trabajo].**
1. Seleccione la función de trabajo que desea eliminar y haga clic en **[!UICONTROL Eliminar].**
1. Si hay algún objeto (usuarios, tareas, problemas) asignado a la función de trabajo, realice una de las siguientes acciones:

   * **Reemplace la función de trabajo con otra función de trabajo:** Seleccione la nueva función de trabajo en la lista desplegable.

      Todas las asignaciones de recursos actuales y anteriores que estén asociadas con la función de trabajo eliminada se transfieren a la función de trabajo seleccionada.

      Los usuarios que solo tienen una función de trabajo asignada se asignan a la función de trabajo seleccionada; los usuarios que tengan una función de trabajo secundaria asignada no se reasignarán a la función de trabajo seleccionada.

   * **Elimine la función de trabajo y su asignación de recursos:** Select **[!UICONTROL Ninguna]** en la lista desplegable.

      >[!IMPORTANT]
      >
      >Al eliminar una función de trabajo, se eliminan todas las asignaciones de recursos actuales y anteriores relacionadas con esa función de trabajo para todos los proyectos.

      &#x200B; Por ejemplo, si una tarea o un problema está asignado solo a esa función de trabajo, la tarea o el problema no se asignan después de que se elimine la función de trabajo.

1. Haga clic en  **[!UICONTROL Sí, Eliminarlo]**.
