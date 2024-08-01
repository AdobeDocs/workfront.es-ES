---
product-area: resource-management
navigation-topic: resource-pools
title: Asociar conjuntos de recursos a proyectos y plantillas
description: Los conjuntos de recursos son colecciones de usuarios que le ayudan a administrar los recursos en Adobe Workfront.
author: Lisa
feature: Resource Management
exl-id: bbfe8257-ff02-4f06-9763-3f2ae4871c9d
source-git-commit: 36599722aafadcbbc630650a94005fd73b3e517e
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 0%

---

# Asociar conjuntos de recursos a proyectos y plantillas


<!-- drafted for bulk editing projects: keep this in yellow till this releases to ALL customers - May 1, 2023

Also - take out all the references to Preview and Prod at prod final
-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->


<!--
<p>The sections about how to add resource pools to templates, projects are duplicated from the articles listed in those sections (Editing Projects, Creating a Template, etc).</p>
<p>***I decided to keep these steps here, though, because it's hard to parse through those much lunger articles for just updating this one field.)</p>
-->

Los conjuntos de recursos son colecciones de usuarios que le ayudan a administrar los recursos en Adobe Workfront.

Después de crear conjuntos de recursos, puede asociarlos a proyectos o plantillas para poder presupuestar posteriormente los recursos en los proyectos.

Se recomienda crear los conjuntos de recursos por adelantado, asociarlos a proyectos y presupuestar los recursos antes de que comience el proyecto.

Para obtener información acerca de los conjuntos de recursos, vea [Resumen de los conjuntos de recursos](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

Para obtener información acerca de cómo crear conjuntos de recursos, vea [Crear conjuntos de recursos](../../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Administración de recursos que incluye acceso a Administrar conjuntos de recursos</p> <p>Editar el acceso a Proyectos, Plantillas y Usuarios</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para los proyectos, plantillas y usuarios con los que asocia los conjuntos de recursos</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Asociar conjuntos de recursos a un proyecto o plantilla

Puede asociar conjuntos de recursos a una plantilla del mismo modo que asocia conjuntos de recursos a un proyecto. Este artículo describe cómo asociar conjuntos de recursos a proyectos.

1. Vaya a un proyecto y haga clic en el icono **Más** ![](assets/more-icon.png)junto al nombre del proyecto; a continuación, haga clic en **Editar**.

1. Haga clic en **Configuración del proyecto**.

1. Empiece a escribir el nombre de un conjunto de recursos en el campo **Conjuntos de recursos** y selecciónelo en la lista cuando aparezca.\
   Puede asociar varios conjuntos de recursos a un proyecto o plantilla.

   ![](assets/nwe-project-settings-in-edit-project-box-350x380.png)

1. Haga clic en **Guardar**.

Para obtener más información sobre cómo editar un proyecto y asociarlo a conjuntos de recursos, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

Para obtener más información sobre cómo editar una plantilla y asociarla a conjuntos de recursos, consulte [Editar plantillas de proyecto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Asociar conjuntos de recursos con varios proyectos o plantillas de forma masiva

Puede editar varios proyectos o plantillas de forma masiva y asociar los mismos conjuntos de recursos a todos ellos al mismo tiempo.

Puede asociar conjuntos de recursos con plantillas de la misma manera que asocia conjuntos de recursos con proyectos.

Para asociar conjuntos de recursos a varios proyectos de forma masiva:

1. Ir a una lista de proyectos.
1. Seleccione varios proyectos y, a continuación, haga clic en el icono **Editar** ![](assets/edit-icon.png) en la parte superior de la lista.

1. Haga clic en **Configuración**.
1. Empiece a escribir el nombre de un conjunto de recursos en el campo **Conjuntos de recursos** y selecciónelo en la lista cuando aparezca.\
   Puede asociar varios conjuntos de recursos con los proyectos o las plantillas.

   >[!NOTE]
   >
   >* Cuando edita las plantillas de forma masiva, solo aparecen en este campo los conjuntos de recursos que son comunes a todas las plantillas seleccionadas. Si las plantillas seleccionadas no tienen conjuntos de recursos compartidos, este campo está vacío. Los conjuntos de recursos que especifique aquí sobrescriben los conjuntos de recursos individuales de los proyectos o plantillas.
   >
   >* Cuando edita proyectos por lotes, aparece el indicador &quot;Varios valores&quot; si los proyectos seleccionados tienen diferentes conjuntos de recursos. Si agrega conjuntos de recursos de forma masiva a los proyectos, todos los conjuntos se agregarán al proyecto seleccionado y se sobrescribirán los conjuntos de recursos originales.

   ![agregar_conjuntos_de_recursos_a_varios_proyectos.png](assets/add-resource-pools-to-multiple-projects-350x358.png)

1. Haga clic en **Guardar cambios**.\
   Cuando los conjuntos de recursos están asociados a sus proyectos o a sus plantillas, puede presupuestar las asignaciones de usuarios para sus proyectos dentro del Planificador de recursos.\
   Para obtener más información sobre el Planificador de recursos, consulte [Resumen del Planificador de recursos](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

Para obtener más información sobre cómo editar proyectos en lotes, consulte la sección &quot;Editar proyectos en lotes&quot; en [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

Para obtener más información acerca de cómo editar plantillas en lotes, consulte la sección &quot;Editar plantillas en lotes&quot; en [Editar plantillas de proyecto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).
