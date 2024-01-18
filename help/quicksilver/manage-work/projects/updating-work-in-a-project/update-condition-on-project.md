---
product-area: projects
navigation-topic: update-work-in-a-project
title: Actualizar la condición de un proyecto
description: La condición de un proyecto es un indicador que se coloca en él para indicar si el trabajo asociado con él se está realizando sin problemas o si se ha encontrado con algún obstáculo. Esto es diferente al estado del proyecto, que indica si está trabajando activamente en él o no.
author: Alina
feature: Work Management
exl-id: 1f46386e-e1ae-4845-8cc4-09dd7d39076f
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 0%

---

# Actualizar la condición de un proyecto

La condición de un proyecto es un indicador que se coloca en él para indicar si el trabajo asociado con él se está realizando sin problemas o si se ha encontrado con algún obstáculo. Esto es diferente al estado del proyecto, que indica si está trabajando activamente en él o no.

Puede establecer la condición de un proyecto de forma automática o manual. Para cambiar la condición de un proyecto manualmente, debe ser el propietario del proyecto o tener derechos de administración sobre él.

El administrador de Adobe Workfront puede crear condiciones personalizadas para su entorno, tal como se describe en [Crear o editar una condición personalizada](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td><p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td>

Para las nuevas licencias:
<p>Estándar</p>

Para licencias actuales:
<ul><li><p>Plan</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de visualización o superior a los proyectos</p> <p>Editar acceso a tareas y problemas </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos superiores en tareas y problemas para ver su condición</p>
   <p>Administrar permisos en tareas y problemas para actualizar la condición</p>
     </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront. Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Establecer automáticamente la condición

La configuración automática de la condición de un proyecto viene determinada por el tipo de condición del proyecto. El tipo de condición debe establecerse en Estado de progreso para que Workfront establezca automáticamente la condición del proyecto.

El administrador de Workfront o de grupo determina el valor predeterminado del campo Tipo de condición para los nuevos proyectos del sistema al establecer las preferencias de proyecto en el área de Configuración. Para obtener más información, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Al crear un proyecto, la condición del proyecto se establece automáticamente para que coincida con el estado de progreso del proyecto en ese momento. El estado del progreso del proyecto se basa en el progreso de las tareas del proyecto.

Para obtener información sobre las condiciones del proyecto y cómo se calculan en función del estado de progreso, consulte [Resumen del estado del progreso del proyecto](../../../manage-work/projects/planning-a-project/project-progress-status.md).

## Actualizar manualmente la condición de un proyecto

Si establece el tipo de condición del proyecto en Manual en lugar del estado de progreso, puede actualizar manualmente la condición de un proyecto.

1. Vaya al proyecto para el que desea actualizar la condición.
1. Haga clic en **Detalles del proyecto** en el panel izquierdo.

1. Asegúrese de que la variable **Tipo de condición** el campo está configurado como **Manual**.

   ![](assets/project-details-overview-edit-enabled-with-condition-shot-nwe-350x251.png)

1. En el **Condición** , seleccione entre las siguientes opciones la que coincida con su comprensión de si el trabajo asociado a él se está realizando sin problemas o si hay algún retraso:

   * **En Target**
   * **En riesgo**
   * **Con problemas**

   Para obtener más información sobre las condiciones del proyecto, consulte [Descripción general de la condición y el tipo de condición del proyecto](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

   >[!NOTE]
   >
   >Las condiciones se pueden personalizar para su entorno, por lo que puede encontrar más de tres opciones para Condición en su entorno. Los nombres de las condiciones pueden ser diferentes a los enumerados anteriormente. Para obtener información sobre la personalización de condiciones en Workfront, consulte [Crear o editar una condición personalizada](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

1. Haga clic en **Guardar cambios**.
