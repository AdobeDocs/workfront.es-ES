---
product-area: resource-management
navigation-topic: resource-planning
title: Localizar el planificador de recursos
description: '(Esto salió de este artículo: borrador de ese contenido en el artículo cuando se publique: /Content/Resource Mgmt/Resource Planning/get-started-resource-planner.html)'
author: Alina
feature: Resource Management
exl-id: 0de749df-5af9-4124-8539-06b82dca2ec4
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---

# Localizar el planificador de recursos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This came off this article: draft that content in the article when this comes live: /Content/Resource Mgmt/Resource Planning/get-started-resource-planner.html)</p>
-->

Puede utilizar el planificador de recursos para administrar la asignación de recursos a los proyectos. Puede acceder al Planificador de recursos para varios proyectos al mismo tiempo o para un proyecto, desde el área Caso de negocio del proyecto.

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Pro y superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Revisar o superior<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        (this seems to be the case in NWE only, not classic. Waiting on Vazgen's response for this)
      </MadCap:conditionalText>
     --></p> <p>Planificar o posterior para localizar el Planificador de recursos en el área global</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Ver acceso o superior a Administración de recursos</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos para proyectos y usuarios </p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Asegúrese de que todos los requisitos previos para acceder y trabajar con el planificador de recursos se cumplan antes de empezar a utilizarlo. De este modo, debe asegurarse de que el planificador de recursos muestre la información correcta antes de comenzar a presupuestar los recursos.

Para obtener información sobre los requisitos previos del planificador de recursos, consulte [Introducción a la planificación de recursos](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

## Localizar el planificador de recursos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this was moved from the get-started-resource-planner article)</p>
-->

Puede ubicar el Planificador de recursos en dos áreas de Workfront, en función de si desea presupuestar los recursos para varios proyectos o solo para un proyecto.

* [Usar el planificador de recursos para varios proyectos](#use-the-resource-planner-for-multiple-projects)
* [Uso del planificador de recursos para un proyecto](#use-the-resource-planner-for-one-project)

### Usar el planificador de recursos para varios proyectos {#use-the-resource-planner-for-multiple-projects}

Al utilizar el Planificador de recursos para varios proyectos, los números de asignación de los recursos representan números de varios proyectos.

Para acceder a la sección Planificador del área Recursos:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Haga clic en **Recurso**. El Planificador se muestra de forma predeterminada.  Para obtener información sobre la presupuestación de recursos en el planificador de recursos, consulte el artículo [Recursos presupuestarios en el planificador de recursos utilizando las vistas Proyecto y Función](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

   ![](assets/qs-resource-management-area-with-planner-as-default-350x152.png)

1. Pase el ratón sobre el panel izquierdo y haga clic en **Grupos de recursos**.\
   Para obtener información sobre la creación de grupos de recursos, consulte [Crear grupos de recursos](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

### Uso del planificador de recursos para un proyecto {#use-the-resource-planner-for-one-project}

Al utilizar el Planificador de recursos para un proyecto, los números de asignación de los recursos representan números para el proyecto seleccionado.

1. Vaya a un proyecto para el que desee presupuestar recursos.
1. Haga clic en **Caso empresarial** en el panel izquierdo.
1. Desplácese hasta el **Presupuestación de recursos** del caso empresarial.
1. Haga clic en **Editar presupuesto de recursos** para agregar grupos de recursos al proyecto y comenzar a presupuestar los recursos.

   >[!TIP]
   >
   >Solo puede agregar un grupo de recursos en el área de Presupuestación de recursos del caso empresarial cuando el proyecto no tiene ningún grupo de recursos asociado a él. Cuando el proyecto ya tiene un grupo de recursos, los usuarios del grupo y sus funciones de trabajo se muestran en el área de presupuestación de recursos de forma predeterminada.

   ![](assets/resource-budgeting-area-on-project-350x70.png)

   Para obtener información sobre la presupuestación de recursos para un proyecto, consulte el artículo [Recursos presupuestarios en el caso empresarial](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).
