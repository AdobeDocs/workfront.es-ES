---
product-area: reporting
keywords: usuario, delegación, informe, delegado, aprobación
navigation-topic: create-and-manage-reports
title: Creación de un informe de delegación de usuario
description: Creación de un informe de delegación de usuario
author: Nolan
feature: Reports and Dashboards
exl-id: c860574b-0488-499e-8d36-d0f3f85aac2d
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 1%

---

# Creación de un informe de delegación de usuario

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: consider moving this to the Custom&nbsp;View, Filter, Grouping Samples section as an example of a report)</p>
-->

En Adobe Workfront, los usuarios pueden delegar aprobaciones de proyectos, tareas y problemas a otros usuarios para asegurarse de que se administran sus aprobaciones cuando están fuera de la oficina. Los usuarios con una licencia de planificación pueden crear un informe de delegación de usuarios para ver lo siguiente:

* Quién ha delegado sus aprobaciones de tareas, problemas y proyectos a otro usuario
* Qué usuarios han delegado aprobaciones de tareas, problemas y proyectos a ellos asignados

* Las fechas de inicio y finalización de las delegaciones

Para obtener más información sobre la delegación de aprobaciones, consulte [Delegar solicitud de aprobación](../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">DRAFTED: To learn more about delegating work, see <a href="../../../workfront-basics/manage-your-account-and-profile/manage-time-off/personal-time-off.md" class="MCXref xref">Log personal time off and delegate your work</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">DRAFTED: To learn how to manage delegated work in Home, see [future link here].</p>
-->

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Editar acceso a filtros, vistas y agrupaciones</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos para los elementos cuyas aprobaciones se han delegado y para los usuarios implicados en la delegación</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Creación de un informe de delegación de usuarios

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y luego haga clic en **Informes**.

1. Haga clic en **Nuevo informe** y, a continuación, seleccione **Delegación de usuario**.\
   ![](assets/classic-new-report-user-delegation-350x644.png)

   Los campos siguientes se muestran en este informe de forma predeterminada:

   | Campo | Descripción |
   |---|---|
   | **De usuario** | Este es el usuario que está delegando sus aprobaciones de tareas, problemas y proyectos a otro usuario. |
   | **Para el usuario** | Usuario al que se han delegado las aprobaciones de tareas, problemas y proyectos. |
   | **Iniciar** | Este es el comienzo del tiempo fuera de la oficina para el usuario que ha realizado las delegaciones. |
   | **Fin** | Este es el final del tiempo de Fuera de la oficina para el usuario que ha realizado las delegaciones. |

   {style="table-layout:auto"}

1. (Opcional) En Report Builder, modifique lo siguiente:

   * Columnas
   * Agrupaciones
   * Filtros
   * Gráfico

   Para obtener más información acerca de estas características, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Cuando termine de crear el informe, haga clic en **Guardar + Cerrar**.

1. Escriba un nombre nuevo en el campo **Nombre del informe** y haga clic en **Guardar informe**.

   Se muestra el informe.
