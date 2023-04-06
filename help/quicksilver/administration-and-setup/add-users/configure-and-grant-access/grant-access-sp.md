---
title: Conceder acceso al Planificador de escenario
description: Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para definir el acceso de un usuario al Planificador de escenario.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4343f0ff-2f78-4556-801f-db9d94f80c95
source-git-commit: 5469598d57fec1a744ddb44cf2accb94e1f70941
workflow-type: tm+mt
source-wordcount: '687'
ht-degree: 0%

---

# Conceder acceso al Planificador de escenario

Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para definir el acceso de un usuario al Planificador de escenario, tal como se explica en [Información general sobre los niveles de acceso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Además del acceso a Scenario Planner, un usuario con un nivel de acceso de administrador que no sea del sistema también debe tener acceso a los datos financieros para ver cualquier información financiera contenida en un plan, como presupuestos, costos y tasas de rol de trabajo. Para obtener más información, consulte [Concesión de acceso a datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>plan de Adobe Workfront*</p> </td> 
   <td>Negocios o superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Revise o superior. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref" data-mc-variable-override="">Información general sobre licencias heredadas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td> <p>Debe adquirir una licencia adicional para el planificador de escenarios de Adobe Workfront para acceder a las funciones que se describen en este artículo.</p> <p>Para obtener información sobre cómo obtener el planificador de escenarios de Workfront, consulte <a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref" data-mc-variable-override="">Acceso necesario para utilizar el planificador de escenarios</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nivel de acceso*</td> 
   <td> <p>Ver acceso o superior al planificador de escenarios</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Permisos de objeto</p> </td> 
   <td> <p>Ver permisos o superiores de un plan</p> <p>Para obtener información sobre la solicitud de acceso adicional a un plan, consulte <a href="../../../scenario-planner/request-access-to-plan.md" class="MCXref xref" data-mc-variable-override="">Solicitar acceso a un plan en el planificador de escenarios</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Configuración del acceso de los usuarios a Scenario Planner mediante un nivel de acceso personalizado

1. Comience a crear o editar el nivel de acceso, tal como se explica en [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Haga clic en la opción a la derecha de **Planificador de escenario** que desea usar para este nivel de acceso.

   >[!NOTE]
   >
   >El tipo de licencia Solicitud o Externa no permite el acceso de Vista o Edición al Planificador de escenario.

1. (Opcional) Para configurar las opciones de acceso de otros objetos y áreas del nivel de acceso en el que esté trabajando, continúe con uno de los artículos enumerados en [Configuración del acceso a Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Concesión de acceso a tareas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) y [Concesión de acceso a datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Cuando haya terminado, haga clic en **Guardar**.

## Acceso al planificador de escenarios por tipo de licencia

Para obtener información sobre lo que los usuarios de cada nivel de acceso pueden hacer con el planificador de escenarios, consulte la sección [Área de Planificador de escenario](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#scenario) en el artículo [Funcionalidad disponible para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Acceso del planificador de escenarios mediante la configuración del nivel de acceso

La siguiente información puede ayudarle a comprender cómo utilizar la configuración de nivel de acceso para controlar el acceso de los usuarios a la información en el planificador de escenarios de Workfront.

* [Sin acceso](#no-access)
* [Ver acceso](#view-access)
* [Editar acceso](#edit-access)

### Sin acceso {#no-access}

Un usuario sin acceso a Scenario Planner no puede ver el icono Escenarios en el menú principal cuando se agrega a su plantilla de diseño ni ver los planes e iniciativas que se comparten con ellos. Si el vínculo a un plan se comparte con un usuario que no tiene acceso a Scenario Planner, el usuario no puede ver ni editar el plan.

### Ver acceso {#view-access}

Los usuarios con acceso de visualización al planificador de escenarios pueden hacer lo siguiente:

* Consulte el icono Escenarios en el menú principal ![](assets/esp-icon-in-main-menu.png), aunque el área Planes está vacía a menos que el usuario haga clic en un vínculo de plan compartido por otro usuario.
* Ver un plan cuando otro usuario comparte el vínculo con él.

   Esto incluye cualquier información sobre la función de trabajo en el plan.

   También incluye tasas de función del puesto de trabajo e información sobre los costos del plan si el usuario receptor también tiene acceso a datos financieros. Para obtener más información, consulte [Concesión de acceso a datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

### Editar acceso {#edit-access}

Los usuarios con acceso de edición al planificador de escenario pueden hacer lo siguiente:

* Consulte el icono Escenarios en el menú principal ![](assets/esp-icon-in-main-menu.png) y utilícelo para acceder a los datos del plan.
* Cree planes.
* Vea, edite y elimine los planes que creen.
* Vea, edite y elimine los planes de otros usuarios a los que acceden mediante un vínculo compartido.

   Esto incluye cualquier información de rol de trabajo en un plan.

   También incluye tasas de función del puesto de trabajo e información sobre los costos del plan si el usuario destinatario tiene acceso a datos financieros. Para obtener más información, consulte [Concesión de acceso a datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
