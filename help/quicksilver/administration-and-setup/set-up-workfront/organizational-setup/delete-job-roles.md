---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Eliminar funciones del puesto
description: Puede eliminar los puestos que ya no utilice su organización. Le recomendamos que no elimine los roles si se han asociado con elementos de trabajo en el pasado. Para conservar toda la información histórica acerca de las asignaciones de trabajo, se recomienda desactivar roles, en lugar de eliminarlos cuando queden obsoletos. Para obtener información sobre la desactivación de funciones, consulte Desactivar funciones del puesto.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b0e81d76-5227-4fda-9a58-68fbce3f5b94
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 0%

---

# Eliminar funciones del puesto

Puede eliminar los puestos que ya no utilice su organización. Le recomendamos que no elimine los roles si se han asociado con elementos de trabajo en el pasado.

Para conservar toda la información histórica acerca de las asignaciones de trabajo, se recomienda desactivar roles, en lugar de eliminarlos cuando queden obsoletos. Para obtener información sobre cómo desactivar roles, consulte [Desactivar roles](../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).

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
   <td> <p>Acceso administrativo a las funciones del puesto</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte al administrador de [!DNL Workfront] si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de [!DNL Workfront] puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

## Eliminar un rol

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved from create and manage job roles)</p>
-->

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront] y, a continuación, haga clic en **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. Haga clic en **[!UICONTROL Roles].**
1. Seleccione el rol que desea eliminar y haga clic en **[!UICONTROL Eliminar].**
1. Si hay algún objeto (usuarios, tareas o problemas) asignado a la función del puesto, realice una de las siguientes acciones:

   * **Reemplazar el rol con un rol diferente:** Seleccione el nuevo rol en la lista desplegable.

     Todas las asignaciones de recursos actuales y anteriores asociadas con el rol eliminado se transfieren al rol seleccionado.

     Los usuarios que solo tienen un rol asignado se reasignan al rol que seleccione; los usuarios que tienen un rol secundario asignado a ellos no se reasignan al rol que seleccione.

   * **Eliminar el rol y su asignación de recursos:** Seleccione **[!UICONTROL Ninguno]** en la lista desplegable.

     >[!IMPORTANT]
     >
     >Al eliminar un rol, se eliminan todas las asignaciones de recursos actuales y pasadas relacionadas con ese rol en todos los proyectos.

     &#x200B;Por ejemplo, si una tarea o un problema se asigna solo a ese rol, la tarea o el problema se anula después de eliminar el rol.

1. Haga Clic En **[!UICONTROL Sí, Eliminarlo]**.
