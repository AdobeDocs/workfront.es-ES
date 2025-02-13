---
product-area: resource-management
navigation-topic: resource-planning
title: Localizar el Planificador de recursos
description: Puede utilizar el Planificador de recursos para administrar la asignación de sus recursos a los proyectos. Puede acceder al Planificador de recursos para varios proyectos al mismo tiempo o para un solo proyecto, desde el área de caso empresarial del proyecto.
author: Lisa
feature: Resource Management
exl-id: 0de749df-5af9-4124-8539-06b82dca2ec4
source-git-commit: a3b2ac192e1f37e0c3d16d059ed96e8d5cadf8be
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 91%

---

# Localizar el Planificador de recursos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This came off this article: draft that content in the article when this comes live: /Content/Resource Mgmt/Resource Planning/get-started-resource-planner.html)</p>
-->

Puede utilizar el Planificador de recursos para administrar la asignación de sus recursos a los proyectos. Puede acceder al Planificador de recursos para varios proyectos al mismo tiempo o para un solo proyecto, desde el área de caso empresarial del proyecto.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td><p>Nuevo: cualquiera</p>
       <p>o</p>
       <p>Actual: pro o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Nuevo: Claro o superior;</br>
          Estándar para localizar el Planificador de recursos en el menú principal</p>
       <p>o</p>
       <p>Actual: revisión o superior;</br>
       Planifique la ubicación del Planificador de recursos en el menú principal</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de visualización o superior a la Administración de recursos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de visualización para proyectos y usuarios </p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Asegúrese de que se cumplen todos los requisitos previos para acceder al Planificador de recursos y trabajar con él antes de empezar a utilizarlo. De este modo, se asegura de que el Planificador de recursos muestra la información correcta antes de empezar a presupuestar los recursos.

Para obtener información sobre los requisitos previos del Planificador de recursos, consulte [Introducción a la planificación de recursos](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

## Localizar el Planificador de recursos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this was moved from the get-started-resource-planner article)</p>
-->

Puede ubicar el Planificador de recursos en dos áreas de Workfront, en función de si desea presupuestar los recursos para varios proyectos o para un solo proyecto.

* [Utilizar el Planificador de recursos para varios proyectos](#use-the-resource-planner-for-multiple-projects)
* [Utilizar el Planificador de recursos para un proyecto](#use-the-resource-planner-for-one-project)

### Utilizar el Planificador de recursos para varios proyectos {#use-the-resource-planner-for-multiple-projects}

Cuando se utiliza el Planificador de recursos para varios proyectos, los números de asignación de los recursos representan números en varios proyectos.

Para acceder a la sección Planificador del área de Recursos:

{{step1-to-resourcing}}

Se muestra el Planificador de forma predeterminada.  Para obtener información sobre el presupuesto de recursos en el Planificador de recursos, consulte el artículo [Presupuesto de recursos en el Planificador de recursos mediante las vistas de proyecto y función](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

![Planificador de recursos predeterminado](assets/qs-resource-management-area-with-planner-as-default-350x152.png)

1. Haga clic en **Conjuntos de recursos** en el panel izquierdo.
Para obtener información sobre la creación de conjuntos de recursos, consulte [Crear conjuntos de recursos](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

### Utilizar el Planificador de recursos para un proyecto {#use-the-resource-planner-for-one-project}

Cuando se utiliza el Planificador de recursos para un proyecto, los números de asignación de los recursos representan números para el proyecto seleccionado.

1. Vaya al proyecto para el que desea presupuestar recursos.
1. Haga clic en **Caso empresarial** en el panel de la izquierda.
1. Desplácese hasta la sección **Presupuestación de recursos** del caso comercial.
1. Haga clic en **Editar presupuesto de recursos** para añadir conjuntos de recursos al proyecto y comenzar a presupuestar los recursos.

   >[!TIP]
   >
   >Solo puede añadir un conjunto de recursos en el área de Presupuestación de recursos del caso empresarial cuando el proyecto no tiene conjuntos de recursos asociados. Cuando el proyecto ya tiene un conjunto de recursos, los usuarios del grupo y sus funciones de trabajo se muestran en el área de Presupuestación de recursos de forma predeterminada.

   ![Presupuestación de recursos](assets/resource-budgeting-area-on-project-350x70.png)

   Para obtener información sobre el presupuesto de recursos de un proyecto, consulte el artículo [Presupuesto de recursos en el caso comercial](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).
