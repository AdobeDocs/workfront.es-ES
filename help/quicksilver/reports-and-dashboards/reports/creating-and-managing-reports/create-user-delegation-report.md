---
product-area: reporting
keywords: usuario, delegación, informe, delegar, aprobación
navigation-topic: create-and-manage-reports
title: Creación de un informe de delegación de usuario
description: Crear un informe de delegación de usuarios
author: Nolan
feature: Reports and Dashboards
exl-id: c860574b-0488-499e-8d36-d0f3f85aac2d
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 90%

---

# Crear un informe de delegación de usuarios

<!--Audited: 10/2024-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: consider moving this to the Custom&nbsp;View, Filter, Grouping Samples section as an example of a report)</p>
-->

En Adobe Workfront, los usuarios pueden delegar aprobaciones de proyectos, tareas y problemas a otros usuarios para asegurarse de que se administran sus aprobaciones cuando están fuera de la oficina. Los usuarios con una licencia Plan pueden crear un informe de delegación de usuarios para ver lo siguiente:

* Quién ha delegado sus aprobaciones de tareas, problemas y proyectos a otro usuario
* Qué usuarios tienen asignadas aprobaciones delegadas de tareas, problemas y proyectos

* Las fechas de inicio y finalización de las delegaciones

Para obtener más información sobre la delegación de aprobaciones, consulte [Delegar solicitud de aprobación](../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">DRAFTED: To learn more about delegating work, see <a href="../../../workfront-basics/manage-your-account-and-profile/manage-time-off/personal-time-off.md" class="MCXref xref">Log personal time off and delegate your work</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">DRAFTED: To learn how to manage delegated work in Home, see [future link here].</p>
-->

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
      <p>Estándar</p>
      <p>Plan</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuración de nivel de acceso</td> 
   <td> <p>Acceso de Edición a informes, paneles de control y calendarios</p> <p>Acceso de edición a filtros, vistas y agrupaciones</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
 <td> <p>Permisos de visualización para los elementos cuyas aprobaciones se han delegado y para los usuarios implicados en la delegación</p></td>  
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Crear un informe de delegación de usuarios

1. Haga clic en el icono **Menú principal** ![Menú principal](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y, a continuación, haga clic en **Informes**.

1. Haga clic en **Nuevo informe** y, a continuación, seleccione **Delegación de usuarios**.

   ![Nueva delegación de usuario de informe](assets/classic-new-report-user-delegation-350x644.png)

   Los campos siguientes se muestran en este informe de forma predeterminada:

   | Campo | Descripción |
   |---|---|
   | **Del usuario** | Es el usuario que va a delegar sus aprobaciones de tareas, problemas y proyectos a otro usuario. |
   | **Para el usuario** | Es el usuario al que se delegan las aprobaciones de tareas, problemas y proyectos. |
   | **Fecha de inicio** | Es el comienzo del tiempo fuera de la oficina para el usuario que ha realizado las delegaciones. |
   | **Fecha de finalización** | Es el final del tiempo fuera de la oficina para el usuario que ha realizado las delegaciones. |

   {style="table-layout:auto"}

1. (Opcional) En Report Builder, modifique lo siguiente:

   * Columnas (vista)
   * Agrupaciones
   * Filtros
   * Gráfico

   Para obtener más información sobre estas características, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Cuando termine de crear el informe, haga clic en **Guardar + Cerrar**.

   Se muestra el informe.
