---
product-area: projects
navigation-topic: manage-projects
title: Seleccione el tipo de actualización del proyecto
description: Al seleccionar un tipo de actualización para un proyecto, puede controlar con qué frecuencia se guardan los cambios realizados en la cronología del proyecto en las tareas principales o en el proyecto.
author: Alina
feature: Work Management
exl-id: ffdfffec-d217-4daa-9849-cb0c794992c0
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---

# Seleccione el tipo de actualización del proyecto

Al seleccionar un tipo de actualización para un proyecto, puede controlar con qué frecuencia se guardan los cambios realizados en la cronología del proyecto en las tareas principales o en el proyecto.

Cuando se actualiza la cronología del proyecto, se vuelve a calcular en función de los cambios realizados en el proyecto, sus tareas o los cambios realizados en otro proyecto del que dependa la cronología.

Por ejemplo, los siguientes cambios en las tareas del proyecto déclencheur una actualización de la cronología del proyecto:

* Actualizar las fechas de las tareas
* Cambiar las relaciones predecesoras de las tareas
* Cambiar las relaciones padre-hijo, agregar o quitar asignaciones además de cambiar la restricción de tarea o el tipo de duración.

## Requisitos de acceso

<!-- drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en un proyecto</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Actualizar el tipo de actualización de un proyecto

Cuando se actualizan las tareas, sus objetos principales (tareas principales o el proyecto) se actualizan en el momento indicado por el tipo de actualización.  Para especificar un tipo de actualización para el proyecto:

1. Vaya al proyecto cuyo tipo de actualización desee especificar.
1. Haga clic en el menú Más ![](assets/more-icon.png) junto al nombre del proyecto y, a continuación, haga clic en **Editar** .

1. Haga clic en  **Proyecto** **Configuración**.

   ![](assets/update-type-field-on-project-edit-box-nwe-350x378.png)

1. En el **Tipo de actualización** , seleccione si desea que Workfront calcule la línea de tiempo del proyecto automáticamente diariamente, cuando hay un cambio o si desea que el administrador del proyecto lo calcule manualmente.

   Seleccione entre las opciones de la lista siguiente. 

   >[!IMPORTANT]
   >
   >Si la escala de tiempo de un proyecto supera los 15 años, Workfront no calcula la escala de tiempo automáticamente ni si cambia. El tipo de actualización de un proyecto que dure más de 15 años siempre es manual.

   * **Automático y en cambio:** Esta es la configuración predeterminada. La cronología del proyecto se actualiza cada vez que se produce un cambio en el proyecto o en otro proyecto del que depende la cronología. La cronología del proyecto también se actualiza cada noche. \
      Esta es la configuración recomendada, ya que garantiza que la cronología del proyecto esté siempre actualizada.

      Cuando se actualiza una tarea o el proyecto y se genera un déclencheur para un nuevo cálculo de la cronología, todas las fechas disponibles se muestran inmediatamente, lo que le permite continuar trabajando. En los proyectos con más de 100 tareas, las fechas que requieren cálculos más largos aparecen atenuadas.

      ![](assets/dates-dimmed-when-insline-editing-350x146.png)

      Esto indica que el nuevo cálculo aún no ha finalizado y que las fechas están sujetas a cambios.

   * **Cambiar solo:** La cronología del proyecto se actualiza cada vez que se produce un cambio en el proyecto o en otro proyecto del que depende la cronología; no se producen actualizaciones programadas.\
      Es posible que desee seleccionar esta opción si le preocupa el rendimiento del sistema y si los cambios raramente se producen en el proyecto o en otros proyectos de los que depende la cronología.

   * **Solo automático:** La cronología del proyecto se actualiza cada noche; no se actualiza inmediatamente después de realizar los cambios.\
      Es posible que desee seleccionar esta opción si le preocupa el rendimiento del sistema y si se producen muchos cambios cada día en el proyecto o en otros proyectos de los que depende la cronología.

      >[!NOTE]
      >
      >Un proyecto no se vuelve a calcular automáticamente cada noche si está en estado de Planning. Solo se vuelve a calcular al cambiar.

   * **Sólo manual:** La cronología del proyecto solo se actualiza cuando selecciona la opción para **Volver a calcular las líneas de tiempo**, tal como se describe en la sección &quot;Cálculo manual&quot; del artículo [Volver a calcular las líneas de tiempo del proyecto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).\
      Es posible que desee seleccionar esta opción si está realizando muchos cambios en el proyecto al mismo tiempo y desea que el cálculo de la cronología se produzca después de que se hayan realizado todos los cambios (en lugar de después de cada cambio individual).

1. Haga clic en **Guardar**.
