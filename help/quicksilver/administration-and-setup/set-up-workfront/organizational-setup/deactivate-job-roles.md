---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Desactivar roles
description: Como administrador o usurario de  [!DNL Adobe Workfront]  con acceso administrativo a las funciones, puede desactivar las que queden obsoletas en su sistema. Cuando desactiva una función en lugar de eliminarla, puede conservar la información histórica asociada a ella.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 934cef1a-8157-45db-b000-24a08a94dd18
source-git-commit: 15063d937a5ba9b5285c66a0987e8deea6cc6d74
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 98%

---

# Desactivar funciones

Como administrador o usurario de [!DNL Adobe Workfront] con acceso administrativo a las funciones, puede desactivar las que queden obsoletas en su sistema. Cuando desactiva una función en lugar de eliminarla, puede conservar la información histórica asociada a ella.

También puede reactivar las funciones que se han desactivado anteriormente.

## Requisitos de acceso

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquete</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licencia</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>Acceso administrativo a los roles</td>
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Impacto de la desactivación de funciones

Si desactiva una función, ya no se mostrará en las siguientes áreas:

* El campo de escritura anticipada [!UICONTROL Asignaciones] (para tareas, tareas de plantilla, problemas, aprobaciones y reglas de enrutamiento)
* Los campos [!UICONTROL Asignaciones] en listas e informes
* Perfiles de usuario

  >[!NOTE]
  >
  >Cuando se añade una función nueva a un usuario, no aparece una función desactivada. Pero continúa mostrándose en los campos [!UICONTROL Función principal] y [!UICONTROL Otras funciones] si el usuario estaba asociado con la función antes de que se desactivara.

* Cuadro de diálogo [!UICONTROL Compartir] para objetos, incluida la asignación de plantillas de diseño
* Campos de escritura anticipada en formularios personalizados
* El campo [!UICONTROL Miembros del grupo] en [!UICONTROL Conjuntos de recursos]
* El campo [!UICONTROL Función] de una pantalla de edición de [!UICONTROL Tarifa de facturación] cuando un usuario anula las tarifas de facturación de los proyectos
* Cuadro de diálogo [!UICONTROL Añadir asignación al tablero Kanban] en un proyecto
* El campo [!UICONTROL Función] de un plan o una iniciativa cuando alguien está usando [!DNL Adobe Workfront Scenario Planner].

  El [!DNL Scenario Planner] solo está disponible en la nueva experiencia de [!DNL Adobe Workfront] y requiere una licencia adicional. Para obtener información sobre el [!DNL Workfront Scenario Planner], consulte [Información general sobre el  [!DNL Scenario Planner] &#x200B;](../../../scenario-planner/scenario-planner-overview.md).

>[!TIP]
>
>Las funciones desactivadas siempre se muestran en los filtros de listas, informes y otras herramientas, como el [!UICONTROL Distribuidor de cargas de trabajo].

## Consideraciones antes de desactivar una función

Es mejor desactivar en lugar de eliminar funciones que se vuelven obsoletas para que pueda mantener toda la información histórica asociada con ellas que puede haber utilizado en el pasado.

>[!NOTE]
>
>Cualquier trabajo asignado a la función antes de la desactivación permanece asignado.

Le recomendamos que haga lo siguiente antes de desactivar una función que no utilice:

* Genere informes para cualquier objeto que esté asignado a la función que tiene previsto desactivar y reasígnelas a una función activa. Para obtener información sobre cómo generar informes, consulte [Crear un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

  >[!TIP]
  >
  >Puede crear un informe para filtrar las tareas o problemas en los que esté asignada la función desactivada. A continuación, utilice el informe para reasignar las tareas o problemas pendientes a una función activa.

* Haga un inventario de todos los procesos de aprobación, las rutas de aprobación actuales y las reglas de enrutamiento u otros objetos asignados a la función que tiene previsto desactivar y reasignarlos a una función activa.

  >[!TIP]
  >
  >Al utilizar colas de solicitudes, si desactiva una función asignada como el usuario asignado de forma predeterminada en una regla de enrutamiento, la función se mantiene y las solicitudes se siguen enrutando a la función desactivada. Se recomienda actualizar las reglas de enrutamiento con funciones activas antes de desactivar el equipo.

  Para obtener información sobre la creación de procesos de aprobación y las reglas de enrutamiento, consulte los siguientes artículos:

   * [Crear un proceso de aprobación para los elementos de trabajo](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)
   * [Crear reglas de enrutamiento](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)

## Desactivar una función

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **[!UICONTROL Funciones].**
1. (Opcional) En el menú desplegable **[!UICONTROL Filtro]**, seleccione **[!UICONTROL Activo]** para mostrar solo las funciones activas.
1. Haga clic en el nombre de la función que desea desactivar.
1. En el menú desplegable **[!UICONTROL Está activo]**, seleccione **[!UICONTROL No]**.

   ![Desactivar rol](assets/deactivate-job-role-edit-role-box-nwe.png)

1. Haga clic en **[!UICONTROL Guardar cambios]**.

   La función está desactivada y ya no se puede asignar al trabajo, asociado con plantillas de diseño, etc. Para obtener información sobre todos los usos de las funciones en [!DNL Workfront], consulte [Información general sobre una función](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).
