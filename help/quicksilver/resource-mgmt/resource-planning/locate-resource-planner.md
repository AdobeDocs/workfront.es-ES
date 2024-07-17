---
product-area: resource-management
navigation-topic: resource-planning
title: Busque el Planificador de recursos
description: "(Esto salió de este artículo: redactar ese contenido en el artículo cuando esto se publique: /Content/Resource Mgmt/Resource Planning/get-started-resource-planner.html)"
author: Alina
feature: Resource Management
exl-id: 0de749df-5af9-4124-8539-06b82dca2ec4
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---

# Busque el Planificador de recursos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This came off this article: draft that content in the article when this comes live: /Content/Resource Mgmt/Resource Planning/get-started-resource-planner.html)</p>
-->

Puede utilizar el Planificador de recursos para administrar la asignación de sus recursos a los proyectos. Puede acceder al Planificador de recursos para varios proyectos al mismo tiempo o para un solo proyecto, desde el área de Caso comercial del proyecto.

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Pro y superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Revisar o superior<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        (this seems to be the case in NWE only, not classic. Waiting on Vazgen's response for this)
      </MadCap:conditionalText>
     --></p> <p>Planifique o superior para localizar el Planificador de recursos en el área global</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Ver acceso o superior a Administración de recursos</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos para proyectos y usuarios </p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Asegúrese de que se cumplan todos los requisitos previos para acceder al Planificador de recursos y trabajar con él antes de empezar a utilizarlo. De este modo, se asegura de que el Planificador de recursos muestra la información correcta antes de empezar a presupuestar los recursos.

Para obtener información acerca de los requisitos previos del Planificador de recursos, consulte [Introducción a la planificación de recursos](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

## Busque el Planificador de recursos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this was moved from the get-started-resource-planner article)</p>
-->

Puede ubicar el Planificador de recursos en dos áreas de Workfront, en función de si desea presupuestar los recursos para varios proyectos o para un solo proyecto.

* [Usar el Planificador de recursos para varios proyectos](#use-the-resource-planner-for-multiple-projects)
* [Utilizar el Planificador de recursos para un proyecto](#use-the-resource-planner-for-one-project)

### Utilizar el Planificador de recursos para varios proyectos {#use-the-resource-planner-for-multiple-projects}

Al utilizar el Planificador de recursos para varios proyectos, los números de asignación de los recursos representan números en varios proyectos.

Para acceder a la sección Planificador del área de Recursos:

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Haga clic en **Recursos**. Se muestra el Planificador de forma predeterminada.  Para obtener información sobre cómo presupuestar recursos en el Planificador de recursos, consulte el artículo [Recursos presupuestarios en el Planificador de recursos mediante las vistas de proyecto y función](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

   ![](assets/qs-resource-management-area-with-planner-as-default-350x152.png)

1. Pase el ratón sobre el panel izquierdo y haga clic en **Conjuntos de recursos**.\
   Para obtener información acerca de cómo crear conjuntos de recursos, vea [Crear conjuntos de recursos](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

### Utilizar el Planificador de recursos para un proyecto {#use-the-resource-planner-for-one-project}

Al utilizar el Planificador de recursos para un proyecto, los números de asignación de los recursos representan números para el proyecto seleccionado.

1. Vaya al proyecto para el que desea presupuestar recursos.
1. Haga clic en **Caso comercial** en el panel izquierdo.
1. Desplácese a la sección **Presupuestación de recursos** del caso comercial.
1. Haga clic en **Editar presupuesto de recursos** para agregar conjuntos de recursos al proyecto y comenzar a presupuestar los recursos.

   >[!TIP]
   >
   >Solo puede agregar un conjunto de recursos en el área de Presupuestación de recursos del caso empresarial cuando el proyecto no tiene conjuntos de recursos asociados. Cuando el proyecto ya tiene un conjunto de recursos, los usuarios del grupo y sus funciones de trabajo se muestran en el área de Presupuestación de recursos de forma predeterminada.

   ![](assets/resource-budgeting-area-on-project-350x70.png)

   Para obtener información acerca de cómo presupuestar recursos para un proyecto, vea el artículo [Recursos de presupuesto en el caso comercial](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).
