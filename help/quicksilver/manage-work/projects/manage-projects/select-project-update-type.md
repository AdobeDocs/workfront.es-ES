---
product-area: projects
navigation-topic: manage-projects
title: Seleccione el tipo de actualización del proyecto
description: Al seleccionar un Tipo de actualización para un proyecto, puede controlar la frecuencia con la que los cambios realizados en la línea de tiempo del proyecto se guardan en las tareas principales o en el proyecto.
author: Alina
feature: Work Management
exl-id: ffdfffec-d217-4daa-9849-cb0c794992c0
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 96%

---

# Seleccionar el tipo de actualización del proyecto

Al seleccionar un Tipo de actualización para un proyecto, puede controlar la frecuencia con la que los cambios realizados en la línea de tiempo del proyecto se guardan en las tareas principales o en el proyecto.

Cuando se actualiza la línea de tiempo del proyecto, se vuelve a calcular en función de los cambios realizados en el proyecto, sus tareas o los cambios realizados en otro proyecto del que depende la línea de tiempo.

Por ejemplo, los siguientes cambios en las tareas del proyecto activan una actualización en la línea de tiempo del proyecto:

* Actualizar las fechas de las tareas
* Cambiar relaciones de predecesoras de tareas
* Cambie las relaciones principal-secundario, añadiendo o quitando asignaciones además de cambiar la restricción de tarea o el tipo de duración.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a proyectos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos en un proyecto</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Actualizar el tipo de actualización de un proyecto

Cuando se actualizan las tareas, sus objetos principales (tareas principales o el proyecto) se actualizan en el momento indicado por el Tipo de actualización.  Para especificar un tipo de actualización para el proyecto:

1. Vaya al proyecto cuyo tipo de actualización desea especificar.
1. Haga clic en el menú Más ![Más icono](assets/more-icon.png) junto al nombre del proyecto y, a continuación, haga clic en **Editar** .

1. Haga clic en **Proyecto** **Configuración**.

   ![](assets/update-type-field-on-project-edit-box-nwe-350x378.png)

1. En el campo **Tipo de actualización**, seleccione si desea que Workfront calcule la línea de tiempo del proyecto automáticamente a diario, cuando haya un cambio o si desea que el administrador ddel proyecto la calcule manualmente.

   Seleccione entre las opciones de la lista siguiente. 

   >[!IMPORTANT]
   >
   >Si la línea de tiempo de un proyecto supera los 15 años, Workfront no calcula la línea de tiempo automáticamente o al cambiar. El tipo de actualización de un proyecto de más de 15 años siempre es manual.

   * **Automático y al cambiar:** esta es la configuración predeterminada. La línea de tiempo del proyecto se actualiza cada vez que se produce un cambio en el proyecto o en otro proyecto del que depende la línea de tiempo. La línea de tiempo del proyecto también se actualiza cada noche. \
     Esta es la configuración recomendada, ya que garantiza que la línea de tiempo del proyecto siempre esté actualizada.

     Al actualizar una tarea o el proyecto y activar un recálculo de la línea de tiempo, se muestran inmediatamente todas las fechas disponibles, lo que le permite continuar trabajando. En proyectos con más de 100 tareas, las fechas que requieren cálculos más largos se atenúan.

     ![](assets/dates-dimmed-when-insline-editing-350x146.png)

     Esto indica que el recálculo aún no ha finalizado y que las fechas están sujetas a cambios.

   * **Solo al cambiar:** la escala de tiempo del proyecto se actualiza cada vez que se produce un cambio en el proyecto o en otro proyecto del que depende la escala de tiempo; las actualizaciones programadas no se llevan a cabo.\
     Es posible que desee seleccionar esta opción si le preocupa el rendimiento del sistema y si los cambios rara vez se producen en el proyecto o en otros proyectos de los que depende la línea de tiempo.

   * **Solo automático:** la escala de tiempo del proyecto se actualiza cada noche; no se actualiza inmediatamente después de realizar los cambios.\
     Es posible que desee seleccionar esta opción si le preocupa el rendimiento del sistema y si se producen muchos cambios cada día en el proyecto o en otros proyectos de los que depende la línea de tiempo.

     >[!NOTE]
     >
     >Un proyecto no se recalcula automáticamente cada noche si se encuentra en estado de Planificación. Solo se recalcula al cambiar.

   * **Solo manual:** la escala de tiempo del proyecto solo se actualiza cuando selecciona la opción **Volver a calcular las escalas de tiempo**, tal como se describe en la sección “Recálculo manual” del artículo [Volver a calcular las escalas de tiempo del proyecto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).\
     Es posible que desee seleccionar esta opción si realiza muchos cambios en el proyecto al mismo tiempo y desea que el cálculo de la escala de tiempo se produzca después de realizar todos los cambios (en lugar de después de cada cambio individual).

1. Haga clic en **Guardar**.
