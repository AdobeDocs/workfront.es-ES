---
title: Conceder acceso al Scenario Planner
description: Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para definir el acceso de un usuario al Scenario Planner.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4343f0ff-2f78-4556-801f-db9d94f80c95
source-git-commit: c887569d59c7751210671cab97c492ee1752fffc
workflow-type: tm+mt
source-wordcount: '697'
ht-degree: 0%

---

# Conceder acceso al Scenario Planner

Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para definir el acceso de un usuario al Scenario Planner, tal como se explica en [Información general sobre los niveles de acceso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Además del acceso a Scenario Planner, un usuario con un nivel de acceso que no sea administrador del sistema también debe tener acceso a los datos financieros para ver cualquier información financiera que contenga un plan, como presupuestos, costes y tasas de función del puesto. Para obtener más información, consulte [Conceder acceso a datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>plan Adobe Workfront*</p> </td> 
   <td>Empresa o superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Revise o superior. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref" data-mc-variable-override="">Resumen de licencias</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td> <p>Debe adquirir una licencia adicional para el planificador de escenarios de Adobe Workfront a fin de acceder a la funcionalidad descrita en este artículo.</p> <p>Para obtener información sobre cómo obtener el Scenario Planner de Workfront, consulte <a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref" data-mc-variable-override="">Acceso necesario para usar el Scenario Planner</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nivel de acceso*</td> 
   <td> <p>Ver el acceso o superior al Scenario Planner</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Permisos de objeto</p> </td> 
   <td> <p>Ver permisos o superiores de un plan</p> <p>Para obtener información sobre cómo solicitar acceso adicional a un plan, consulte <a href="../../../scenario-planner/request-access-to-plan.md" class="MCXref xref" data-mc-variable-override="">Solicitar acceso a un plan en el Scenario Planner</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

+++

## Configurar el acceso de los usuarios al Scenario Planner mediante un nivel de acceso personalizado

1. Comience a crear o editar el nivel de acceso, tal como se explica en [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Haga clic en la opción a la derecha de **Planificador de escenarios** que desee usar para este nivel de acceso.

   >[!NOTE]
   >
   >El tipo de licencia de solicitud o externa no permite el acceso de visualización o edición al Scenario Planner.

1. (Opcional) Para establecer la configuración de acceso para otros objetos y áreas en el nivel de acceso en el que está trabajando, continúe con uno de los artículos enumerados en [Configurar el acceso a Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Conceder acceso a las tareas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) y [Conceder acceso a los datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Cuando termine, haga clic en **Guardar**.

## Acceso a Scenario Planner por tipo de licencia

Para obtener información acerca de lo que los usuarios de cada nivel de acceso pueden hacer con el Scenario Planner, vea la sección [Área del Scenario Planner](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#scenario) en el artículo [Funcionalidad disponible para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Acceso al Scenario Planner por configuración de nivel de acceso

La siguiente información puede ayudarle a comprender cómo utilizar la configuración de Nivel de acceso para controlar el acceso de los usuarios a la información en el Scenario Planner de Workfront.

* [Sin acceso](#no-access)
* [Ver acceso](#view-access)
* [Editar acceso](#edit-access)

### Sin acceso {#no-access}

Un usuario sin acceso al Scenario Planner no puede ver el icono de escenarios en el menú principal cuando se añade a su plantilla de diseño, ni ver los planes e iniciativas que se comparten con él. Si el vínculo a un plan se comparte con un usuario que no tiene acceso al Scenario Planner, el usuario no podrá ver ni editar el plan.

### Ver acceso {#view-access}

Los usuarios con acceso de Vista al Planificador de escenarios pueden hacer lo siguiente:

* Vea el icono Escenarios en el menú principal ![](assets/esp-icon-in-main-menu.png), aunque el área Planes está vacía a menos que el usuario haga clic en un vínculo de plan compartido por otro usuario.
* Ver un plan cuando otro usuario comparta el vínculo con él.

  Esto incluye cualquier información sobre el rol en el plan.

  También incluye las tasas de funciones del puesto e información sobre los costes del plan si el usuario destinatario también tiene acceso a los datos financieros. Para obtener más información, consulte [Conceder acceso a datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

### Editar acceso {#edit-access}

Los usuarios con acceso de edición en el Scenario Planner pueden hacer lo siguiente:

* Consulte el icono Escenarios en el menú principal ![](assets/esp-icon-in-main-menu.png) y utilícelo para acceder a los datos del plan.
* Cree planes.
* Ver, editar y eliminar los planes que crean.
* Ver, editar y eliminar los planes de otros usuarios a los que acceden mediante un vínculo compartido.

  Esto incluye cualquier información sobre el rol de un plan.

  También incluye tasas de funciones del puesto e información de costes en el plan si el usuario destinatario tiene acceso a los datos financieros. Para obtener más información, consulte [Conceder acceso a datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
