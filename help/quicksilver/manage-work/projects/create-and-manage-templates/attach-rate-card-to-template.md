---
content-type: overview
product-area: templates
navigation-topic: financials
title: Adjuntar una tarjeta de tarifa a una plantilla
description: Al asignar una tarjeta de tasa a una plantilla, la tarjeta de tasa se adjunta a todos los proyectos creados a partir de la plantilla.
author: Lisa
feature: Work Management
source-git-commit: ca2effb6674caf3a1b44f675a23758f734332a01
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 10%

---

# Adjuntar una tarjeta de tarifa a una plantilla

{{highlighted-preview-article-level}}

Al asignar una tarjeta de tasa a una plantilla, la tarjeta de tasa se adjunta a todos los proyectos creados a partir de la plantilla. La tarjeta de tarifa se convierte en la predeterminada en el proyecto, pero se puede anular si es necesario.

Para obtener información sobre las tarjetas de tarifas, consulte [Administrar tarjetas de tarifas](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md).

Para obtener información acerca de las plantillas de proyecto, vea [Descripción general de la plantilla de proyecto](/help/quicksilver/manage-work/projects/create-and-manage-templates/project-template-overview.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Paquete de Adobe Workfront</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td>Estándar</td> 
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>Acceso de edición a las plantillas</td> 
  </tr> 
  <tr> 
   <td>Permisos de objeto</td> 
   <td>Administre los permisos de la tarjeta Tarifas con permisos para Editar Tarifas de facturación</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

La tarjeta de tarifas que desee asignar a la plantilla debe crearse en Workfront. Para obtener más información, consulte [Administrar tarjetas de tarifas](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md).

El campo **Tarjeta de tarifa** debe estar habilitado para las plantillas de la plantilla de diseño.

1. En la plantilla de diseño, haga clic en la flecha abajo debajo de **Personalizar lo que ven los usuarios** y, a continuación, haga clic en **Plantilla**.
1. En la sección **Detalles**, seleccione el campo **Tarjeta de tarifa** en el área **Información general**.

   Para obtener más información, consulte [Personalizar la vista de detalles con una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

## Adjuntar una tarjeta de tarifa a una plantilla

{{step1-to-templates}}

1. Cree una plantilla nueva o edite una plantilla existente.
1. En la sección Template Details > Overview > Template association, seleccione una tarjeta de tarifa en el campo **Rate Card**.

   Solo las tarjetas de clasificación para las que tenga permisos están disponibles para elegir.
Puede empezar a escribir el nombre de una tarjeta de tasa para reducir la lista de resultados.

   ![Seleccione una tarifa en la plantilla](assets/select-rate-card-on-template.png)

1. Guarde la plantilla cuando haya terminado de editarla.

   Para obtener más información sobre cómo crear una plantilla, vea [Crear una plantilla de proyecto](/help/quicksilver/manage-work/projects/create-and-manage-templates/create-template.md).

   Para obtener más información sobre cómo editar una plantilla, consulte [Editar plantillas de proyecto](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md).

## Aplicar la plantilla a un proyecto

1. Cree un proyecto con la plantilla.

   Existen varias formas de crear un proyecto a partir de una plantilla. Para obtener más información, consulte estos artículos:

   * [Crear un proyecto a partir de una plantilla](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md)
   * [Convertir una tarea en un proyecto](/help/quicksilver/manage-work/tasks/manage-tasks/convert-task-to-project.md)
   * [Convertir un problema en un proyecto](/help/quicksilver/manage-work/issues/convert-issues/convert-issue-to-project.md)

   La tarjeta de tarifas se guarda automáticamente en el proyecto. En la sección Información general > Asociación del proyecto del cuadro Nuevo proyecto, puede quitar la tarjeta de tarifa o seleccionar una tarjeta de tarifa diferente en el campo **Tarjeta de tarifa**.

   ![La tarjeta Tarifa de la plantilla aparece en los detalles del proyecto](assets/create-project-from-template-rate-card.png)

   La tarjeta Tarifas y sus tarifas asociadas aparecen en el área Tarifas del proyecto.

   También puede eliminar la tarjeta de tarifas del proyecto o adjuntar una tarjeta de tarifas diferente en el área Tarifas. Para obtener más información, consulte [Adjuntar una tarjeta de tarifa a un proyecto](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md).

   ![Tarjeta de tarifa de la plantilla en el proyecto](assets/template-rates-on-project.png)

   >[!NOTE]
   >
   >Si hay una tasa individual en la plantilla y también se adjunta una tarjeta de tasa a la plantilla, al crear un proyecto a partir de la plantilla, tanto la tasa individual como la tarjeta de tasa aparecerán en la lista de tasas.

1. (Opcional) Para aplicar la tarjeta de tarifas a un proyecto existente, adjunte la plantilla al proyecto.

   Cuando use la opción **Personalizar y adjuntar** en la vista previa de la plantilla, puede seleccionar el elemento **Tarjeta de tarifa** en la sección Adjuntar plantilla > Opciones para agregar la tarjeta de tarifa al proyecto. Desactive la casilla de verificación para excluir la transferencia de la tarjeta de tarifa al proyecto.

   Para obtener más información, vea [Adjuntar una plantilla a un proyecto](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

1. (Opcional) Para guardar la tarjeta de tasas de un proyecto específico en una plantilla, guarde el proyecto como una plantilla.

   En la sección Opciones del cuadro Guardar como plantilla, puede seleccionar el elemento **Tarjeta de tarifa** para agregar la tarjeta de tarifa a la plantilla. Desactive la casilla de verificación para excluir la transferencia de la tarjeta de tarifa a la plantilla.

   Para obtener más información, vea [Guardar un proyecto como plantilla](/help/quicksilver/manage-work/projects/manage-projects/save-project-as-template.md)


