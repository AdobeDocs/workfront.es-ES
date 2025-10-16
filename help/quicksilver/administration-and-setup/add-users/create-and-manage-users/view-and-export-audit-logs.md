---
title: Ver y exportar registros de auditoría
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Puede ver todos los registros de auditoría del sistema o los que cumplen determinados criterios de filtrado. También puede exportar registros de auditoría. Los registros de auditoría enumeran los cambios de usuario activados en el sistema durante los últimos 90 días.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: b04e8ba5-c3f2-4838-8df1-35e90de5c7bd
source-git-commit: c8987d036e1c1324618cb53ebcbb8fd7e4bcc6a4
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 10%

---

# Ver y exportar registros de auditoría

<!--Audited: 08/2025-->

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **
-->

Puede ver todos los registros de auditoría del sistema o los que cumplen determinados criterios de filtrado. También puede exportar registros de auditoría a un archivo CSV.

Los registros de auditoría enumeran los cambios de usuario activados en el sistema durante los últimos 90 días.

Para obtener información acerca de todos los tipos de registros de auditoría y lo que los genera, vea [Resumen de los registros de auditoría](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p>
       <p>Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td><p>Administrador del sistema</p></td>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td><p>System Administrator</p></td>
  </tr> 
 </tbody> 
</table>-->

## Ver registros de auditoría

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Sistema > Registros de auditoría**.
1. En la lista desplegable **Tipo de acción**, seleccione el tipo de auditoría que desea ver.

   >[!NOTE]
   >
   >Las opciones del menú desplegable Tipo de acción varían según el registro de auditoría seleccionado.

1. En el menú desplegable **Tipo de registro**, seleccione el tipo de registro de auditoría que desea ver.

   **Todos los tipos de registro** está seleccionado de forma predeterminada.

   Para obtener una lista de todos los tipos de registros de auditoría que puede ver y la información que contienen, vea [Resumen de los registros de auditoría](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

1. (Opcional) Defina cualquiera de los filtros disponibles para los siguientes campos:

   * **Usuarios**: escriba el nombre del usuario que realizó el cambio.
   * **Desde**: fecha de inicio del lapso de tiempo en que se realizó el cambio.
   * **Para**: Fecha de finalización del lapso de tiempo en que se realizó el cambio.

   ![Registros de auditoría](assets/audit-logs.png)

1. Haga clic en **Aplicar**.
1. (Opcional) Haga clic en **Borrar** para restablecer los cambios realizados en los filtros.

## Exportar registros de auditoría

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Sistema** > **Registros de auditoría**.

1. En el menú desplegable **Tipo de registro**, seleccione un registro de auditoría.

   **Todos los tipos de registro** está seleccionado de forma predeterminada.

1. Defina cualquiera de los filtros disponibles y luego haga clic en **Aplicar**.

   >[!IMPORTANT]
   >
   >No se pueden exportar más de 50 000 registros al mismo tiempo. Workfront exporta registros en función de los filtros configurados, no del número de registros que se muestran en la página. Puede ver el número total de registros filtrados en la esquina inferior derecha de la página.

1. Haga clic en **Exportar**.

   Se abrirá el cuadro Guardar archivo y podrá guardar el archivo exportado en el equipo.

   Los registros de auditoría solo se pueden guardar en formato CSV.

   Termine de guardar el archivo exportado. Ahora puede encontrarlo en el equipo y compartirlo con otros usuarios.
