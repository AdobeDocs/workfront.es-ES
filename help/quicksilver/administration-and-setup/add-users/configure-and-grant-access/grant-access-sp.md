---
title: Conceder acceso al Planificador de escenarios
description: Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para definir el acceso de un usuario al Planificador de escenarios.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4343f0ff-2f78-4556-801f-db9d94f80c95
source-git-commit: 2a83e5a415ff254cf5525d6f44ecb0e447e7e70a
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 97%

---

# Conceder acceso al Planificador de escenarios

Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para definir el acceso de un usuario al Planificador de escenarios, tal como se explica en la [Información general sobre los niveles de acceso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Además del acceso al Planificador de escenarios, un usuario con un nivel de acceso que no sea administrador del sistema también debe tener acceso a los datos financieros para ver cualquier información financiera que contenga un plan, como presupuestos, costes y tarifas de función. Para obtener más información, consulte [Conceder acceso a datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>paquete de Adobe Workfront</p> </td> 
   <td>Business o superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
   <p>Ligero o superior</p>
   <p>Revisión o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Producto</td> 
   <td> <p>Debe adquirir una licencia adicional para Adobe Workfront Scenario Planner.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de visualización o superior al planificador de escenarios</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Permisos de objeto</p> </td> 
   <td> <p>Permisos de visualización o superiores para un plan</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar el acceso del usuario al Planificador de escenarios mediante un nivel de acceso personalizado

1. Comience a crear o editar el nivel de acceso, tal como se explica en [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Haga clic en la opción a la derecha del **Planificador de escenarios** que desee usar para este nivel de acceso.

   >[!NOTE]
   >
   >El tipo de licencia de solicitud o externa no permite el acceso de visualización o edición en el Planificador de escenarios.

1. (Opcional) Para establecer la configuración de acceso para otros objetos y áreas del nivel de acceso en el que está trabajando, continúe con uno de los artículos enumerados en [Configurar el acceso a Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Conceder acceso a las tareas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) y [Conceder acceso a los datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Cuando termine, haga clic en **Guardar**.

## Acceso al Planificador de escenarios por tipo de licencia

Para obtener información sobre lo que los usuarios de cada nivel de acceso pueden hacer con el Planificador de escenarios, consulte la sección [Área del Planificador de escenarios](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#scenario) en el artículo [Funcionalidad disponible para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Acceso al Planificador de escenarios por configuración de nivel de acceso

La siguiente información puede ayudarle a comprender cómo utilizar la configuración del nivel de acceso para controlar el acceso de los usuarios a la información en el Planificador de escenarios de Workfront.

* [Sin acceso](#no-access)
* [Acceso de visualización](#view-access)
* [Acceso de edición](#edit-access)

### Sin acceso {#no-access}

Un usuario sin acceso al Planificador de escenarios no puede ver el icono de escenarios en el menú principal cuando se añade a su plantilla de diseño, ni ver los planes e iniciativas que se comparten con él. Si el vínculo a un plan se comparte con un usuario que no tiene acceso al Planificador de escenarios, el usuario no podrá ver ni editar el plan.

### Acceso de visualización {#view-access}

Los usuarios con acceso de visualización al Planificador de escenarios pueden hacer lo siguiente:

* Ver el icono Escenarios en el menú principal de ![](assets/esp-icon-in-main-menu.png), aunque el área Planes está vacía a menos que el usuario haga clic en un vínculo de plan compartido por otro usuario.
* Ver un plan cuando otro usuario comparta el vínculo con él.

  Esto incluye cualquier información sobre la función en el plan.

  También incluye las tarifas de las funciones e información sobre los costes del plan si el usuario destinatario también tiene acceso a los datos financieros. Para obtener más información, consulte [Conceder acceso a los datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

### Acceso de edición {#edit-access}

Los usuarios con acceso de edición al Planificador de escenarios pueden hacer lo siguiente:

* Consulte el icono Escenarios en el menú principal de ![](assets/esp-icon-in-main-menu.png) y utilícelo para acceder a los datos del plan.
* Cree planes.
* Ver, editar y eliminar los planes que han creado.
* Ver, editar y eliminar los planes de otros usuarios a los que acceden mediante un vínculo compartido.

  Esto incluye cualquier información sobre una función en un plan.

  También incluye las tarifas de las funciones y la información sobre los costes del plan si el usuario destinatario tiene acceso a los datos financieros. Para obtener más información, consulte [Conceder acceso a los datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
