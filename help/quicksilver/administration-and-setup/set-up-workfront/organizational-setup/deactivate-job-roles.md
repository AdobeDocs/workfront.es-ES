---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Desactivar funciones de trabajo
description: Como [!DNL Adobe Workfront] o un usuario con acceso administrativo a Funciones de trabajo, puede desactivar las funciones de trabajo que queden obsoletas en su sistema. Al desactivar una función de trabajo en lugar de eliminarla, puede conservar cualquier información histórica asociada a ella.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 934cef1a-8157-45db-b000-24a08a94dd18
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 0%

---

# Desactivar funciones de trabajo

Como [!DNL Adobe Workfront] o un usuario con acceso administrativo a Funciones de trabajo, puede desactivar las funciones de trabajo que queden obsoletas en su sistema. Al desactivar una función de trabajo en lugar de eliminarla, puede conservar cualquier información histórica asociada a ella.

También puede reactivar las funciones de trabajo que se hayan desactivado anteriormente.

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de [!UICONTROL Adobe Workfront]*</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia [!UICONTROL Adobe Workfront]*</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso administrativo a las funciones de trabajo</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## El impacto de la desactivación de funciones de trabajo

Si desactiva una función de trabajo, ya no se muestra en las siguientes áreas:

* La variable [!UICONTROL Asignaciones] campo typeforward (para tareas, tareas de plantilla, problemas, aprobaciones y reglas de enrutamiento)
* La variable [!UICONTROL Asignaciones] campos en listas e informes
* Perfiles de usuario

   >[!NOTE]
   >
   >Cuando agrega una función nueva a un usuario, no se muestra una función de trabajo desactivada. Pero sigue mostrándose en la variable [!UICONTROL Función principal] y [!UICONTROL Otras funciones] si el usuario estaba asociado con la función de trabajo antes de desactivarla.

* La variable [!UICONTROL Uso compartido] cuadro de diálogo para objetos, incluida la asignación de plantilla de diseño
* Campos Typeforward en formularios personalizados
* La variable [!UICONTROL Miembros del grupo] en [!UICONTROL Grupos de recursos]
* La variable [!UICONTROL Función del trabajo] campo de [!UICONTROL Tasa de facturación] editar pantalla cuando un usuario anula las tasas de facturación de los proyectos
* La variable [!UICONTROL Agregar asignación a un tablero kanban] cuadro de diálogo de un proyecto
* La variable [!UICONTROL Función del trabajo] campo de un plan o una iniciativa cuando alguien está utilizando la variable [!DNL Adobe Workfront Scenario Planner].

   La variable [!DNL Scenario Planner] solo está disponible en el nuevo [!DNL Adobe Workfront] experiencia y requiere una licencia adicional. Para obtener información sobre la variable [!DNL Workfront Scenario Planner], consulte [La variable [!DNL Scenario Planner] información general](../../../scenario-planner/scenario-planner-overview.md).

>[!TIP]
>
>Los roles desactivados siempre se muestran en filtros de listas, informes y otras herramientas, como la variable [!DNL Workload Balancer].

## Consideraciones antes de desactivar una función de trabajo

Es mejor desactivar en lugar de eliminar las funciones de trabajo que quedan obsoletas, de modo que pueda conservar toda la información histórica asociada a las funciones que haya utilizado en el pasado.

>[!NOTE]
>
>Cualquier trabajo asignado a la función de trabajo antes de la desactivación permanece asignado.

Le recomendamos que haga lo siguiente antes de desactivar una función de trabajo no utilizada:

* Genere informes para cualquier objeto que esté asignado a la función que desea desactivar y reasignarlo a una función de trabajo activa. Para obtener información sobre la creación de informes, consulte [Crear un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

   >[!TIP]
   >
   >Puede crear un informe para filtrar por cualquier tarea o problema al que se le asigne la función desactivada. A continuación, utilice el informe para reasignar tareas o problemas pendientes a una función activa.

* Realice un inventario de todos los procesos de aprobación, las rutas de aprobación actuales y las reglas de enrutamiento u otros objetos asignados a la función de trabajo que desea desactivar y reasignarlos a una función activa.

   >[!TIP]
   >
   >Cuando se utilizan colas de solicitud, si se desactiva una función de trabajo asignada como usuario asignado predeterminado en una regla de enrutamiento, la función permanece y las solicitudes siguen enrutadas a la función desactivada. Se recomienda actualizar las reglas de enrutamiento con funciones activas antes de desactivar el equipo.

   Para obtener información sobre la creación de procesos de aprobación y reglas de enrutamiento, consulte los siguientes artículos:

   * [Creación de un proceso de aprobación para elementos de trabajo](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)
   * [Crear reglas de enrutamiento](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)

## Desactivar una función de trabajo

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en &#x200B; **[!UICONTROL Funciones del trabajo].**
1. (Opcional) En la **[!UICONTROL Filtro]** menú desplegable, seleccione **[!UICONTROL Activo]** para mostrar solo los roles de trabajo activos.
1. Haga clic en el nombre de la función de trabajo que desea desactivar.
1. En el **[!UICONTROL Está activo]** menú desplegable, seleccione **[!UICONTROL No]**.

   ![](assets/deactivate-job-role-edit-role-box-nwe.png)

1. Haga clic en **[!UICONTROL Guardar cambios]**.

   La función de trabajo está desactivada y ya no se puede asignar a trabajo, está asociada a plantillas de diseño, etc. Para obtener información sobre todos los usos de las funciones de trabajo en [!DNL Workfront], consulte [Información general sobre la función de trabajo](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).
