---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Eliminar roles
description: Puede eliminar los puestos que ya no utilice su organización. Le recomendamos que no elimine los roles si se han asociado con elementos de trabajo en el pasado. Para conservar toda la información histórica acerca de las asignaciones de trabajo, se recomienda desactivar roles, en lugar de eliminarlos cuando queden obsoletos. Para obtener información sobre la desactivación de funciones, consulte Desactivar funciones del puesto.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b0e81d76-5227-4fda-9a58-68fbce3f5b94
source-git-commit: 439303273239549bb326c171be44eea321f5bb5f
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 1%

---

# Eliminar funciones del puesto

Puede eliminar los puestos que ya no utilice su organización. Le recomendamos que no elimine los roles si se han asociado con elementos de trabajo en el pasado.

Para conservar toda la información histórica acerca de las asignaciones de trabajo, se recomienda desactivar roles, en lugar de eliminarlos cuando queden obsoletos. Para obtener información sobre cómo desactivar roles, consulte [Desactivar roles](../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td>
   <p>Nuevo: [!UICONTROL Standard]</p>
   <p>O</p>
   <p>Actual: [!UICONTROL plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>Acceso administrativo a los roles</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Eliminar un rol

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved from create and manage job roles)</p>
-->

{{step-1-to-setup}}

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
