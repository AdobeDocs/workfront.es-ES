---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Desactivar roles
description: Como administrador de  [!DNL Adobe Workfront] o usuario con acceso administrativo a los roles, puede desactivar los roles que queden obsoletos en su sistema. Cuando desactiva un rol en lugar de eliminarlo, puede conservar la información histórica asociada a él.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 934cef1a-8157-45db-b000-24a08a94dd18
source-git-commit: 439303273239549bb326c171be44eea321f5bb5f
workflow-type: tm+mt
source-wordcount: '661'
ht-degree: 1%

---

# Desactivar funciones del puesto

Como administrador de [!DNL Adobe Workfront] o usuario con acceso administrativo a los roles, puede desactivar los roles que queden obsoletos en su sistema. Cuando desactiva un rol en lugar de eliminarlo, puede conservar la información histórica asociada a él.

También puede reactivar los roles que se han desactivado anteriormente.

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

## Impacto de la desactivación de funciones del puesto

Si desactiva un rol, ya no se mostrará en las siguientes áreas:

* El campo de escritura anticipada [!UICONTROL Asignaciones] (para tareas, tareas de plantilla, problemas, aprobaciones y reglas de enrutamiento)
* Los campos [!UICONTROL Asignaciones] en listas e informes
* Perfiles de usuario

  >[!NOTE]
  >
  >Cuando se agrega una función nueva a un usuario, no aparece la función de trabajo desactivada. Pero continúa mostrándose en los campos [!UICONTROL Rol principal] y [!UICONTROL Otros roles] si el usuario estaba asociado con el rol antes de que se desactivara.

* Cuadro de diálogo [!UICONTROL Compartir] para objetos, incluida la asignación de plantillas de diseño
* Campos de escritura anticipada en formularios personalizados
* El campo [!UICONTROL Miembros del grupo] en [!UICONTROL Grupos de recursos]
* El campo [!UICONTROL Rol] de una pantalla de edición de [!UICONTROL Tarifa de facturación] cuando un usuario anula las tarifas de facturación de los proyectos
* Cuadro de diálogo [!UICONTROL Agregar asignación al Panel Kanban] en un proyecto
* El campo [!UICONTROL Rol] de un plan o una iniciativa cuando alguien está usando [!DNL Adobe Workfront Scenario Planner].

  [!DNL Scenario Planner] solo está disponible en la nueva experiencia [!DNL Adobe Workfront] y requiere una licencia adicional. Para obtener información acerca de [!DNL Workfront Scenario Planner], vea [La [!DNL Scenario Planner] descripción general](../../../scenario-planner/scenario-planner-overview.md).

>[!TIP]
>
>Los roles desactivados siempre se muestran en los filtros de listas, informes y otras herramientas, como [!UICONTROL Distribuidor de cargas de trabajo].

## Consideraciones antes de desactivar un rol

Es mejor desactivar, en lugar de eliminar, los roles que se vuelven obsoletos para que pueda mantener toda la información histórica asociada con los roles que puede haber utilizado en el pasado.

>[!NOTE]
>
>Cualquier trabajo asignado al rol antes de la desactivación permanece asignado.

Le recomendamos que haga lo siguiente antes de desactivar un rol que no utilice:

* Genere informes para cualquier objeto que esté asignado al rol que planea desactivar y reasigne a un rol activo. Para obtener información sobre cómo generar informes, consulte [Crear un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

  >[!TIP]
  >
  >Puede crear un informe para filtrar por cualquier tarea o problema en el que se asigne la función desactivada. A continuación, utilice el informe para reasignar las tareas o problemas pendientes a un rol activo.

* Haga un inventario de todos los procesos de aprobación, las rutas de aprobación actuales y las reglas de ruta u otros objetos asignados a la función que planea desactivar y reasignarlos a una función activa.

  >[!TIP]
  >
  >Al utilizar colas de solicitudes, si desactiva una función asignada como el usuario asignado por defecto en una regla de enrutamiento, la función se mantiene y las solicitudes se siguen enrutando a la función desactivada. Se recomienda actualizar las reglas de enrutamiento con funciones activas antes de desactivar el equipo.

  Para obtener información sobre la creación de procesos de aprobación y reglas de enrutamiento, consulte los siguientes artículos:

   * [Crear un proceso de aprobación para los elementos de trabajo](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)
   * [Crear reglas de enrutamiento](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)

## Desactivar un rol

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en&#x200B; **[!UICONTROL Funciones del puesto].**
1. (Opcional) En el menú desplegable **[!UICONTROL Filtro]**, seleccione **[!UICONTROL Activo]** para mostrar solo los roles activos.
1. Haga clic en el nombre de la función que desea desactivar.
1. En el menú desplegable **[!UICONTROL Está activo]**, seleccione **[!UICONTROL No]**.

   ![](assets/deactivate-job-role-edit-role-box-nwe.png)

1. Haga clic en **[!UICONTROL Guardar cambios]**.

   La función está desactivada y ya no se puede asignar al trabajo, asociado a plantillas de diseño, etc. Para obtener información acerca de todos los usos de los roles en [!DNL Workfront], vea [Descripción general del rol](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).
