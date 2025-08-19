---
title: Ver y exportar registros de auditoría
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Puede ver todos los registros de auditoría del sistema o los que cumplen determinados criterios de filtrado. También puede exportar registros de auditoría. Los registros de auditoría enumeran los cambios de usuario activados en el sistema durante los últimos 90 días.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b04e8ba5-c3f2-4838-8df1-35e90de5c7bd
source-git-commit: 994518f7abe519180fa6c3eab6b29165475ab4fc
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 19%

---

# Ver y exportar registros de auditoría

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **
-->

Puede ver todos los registros de auditoría del sistema o los que cumplen determinados criterios de filtrado. También puede exportar registros de auditoría.

Los registros de auditoría enumeran los cambios de usuario activados en el sistema durante los últimos 90 días.

Para obtener información acerca de todos los tipos de registros de auditoría y lo que los genera, vea [Registros de auditoría](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

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
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ver registros de auditoría

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Sistema > Registros de auditoría**.
1. En el menú desplegable **Tipo de registro**, seleccione el tipo de registro de auditoría que desea ver.

   **Todos los tipos de registro** está seleccionado de forma predeterminada.

   Para obtener una lista de todos los tipos de registros de auditoría que puede ver y la información que contienen, vea [Registros de auditoría](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

1. (Opcional) Defina cualquiera de los filtros disponibles.

   >[!NOTE]
   >
   >Las opciones del menú desplegable Tipo de acción varían según el registro de auditoría seleccionado.

   ![Registros de auditoría](assets/audit-logs.png)

1. Haga clic en **Aplicar**.
1. (Opcional) Haga clic en **Borrar filtros** para restablecer los cambios realizados en los filtros.

## Exportar registros de auditoría

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Sistema > Seguimiento de cambios > Registros de auditoría**.

1. En el menú desplegable **Tipo de registro**, seleccione un registro de auditoría.

   **Todos los tipos de registro** está seleccionado de forma predeterminada.

1. Defina cualquiera de los filtros disponibles y luego haga clic en **Aplicar**.

   >[!IMPORTANT]
   >
   >No se pueden exportar más de 50 000 registros al mismo tiempo. Workfront exporta registros en función de los filtros configurados, no del número de registros que se muestran en la página. Puede ver el número total de registros filtrados en la esquina inferior derecha de la página.

1. Haga clic en **Exportar**.
