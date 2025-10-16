---
product-area: resource-management
navigation-topic: resource-planning
title: Ajustar fechas de presupuesto en el planificador de recursos
description: Si observa que hay sobreasignaciones de los recursos después de haberlos presupuestado en el Planificador de recursos, puede explorar escenarios alternativos moviendo los valores de horas presupuestadas, FTE o costes a otro lapso de tiempo. En función de los resultados de estos escenarios, puede ajustar las horas presupuestadas, el equivalente a jornadas completas o los costes.
author: Lisa
feature: Resource Management
exl-id: bc49d45a-73a5-4b02-9054-9c9dbb54224d
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 97%

---

# Ajustar fechas de presupuesto en el Planificador de recursos

Si observa que hay sobreasignaciones de los recursos después de haberlos presupuestado en el Planificador de recursos, puede explorar escenarios alternativos moviendo los valores de horas presupuestadas, FTE o costes a otro lapso de tiempo. En función de los resultados de estos escenarios, puede ajustar las horas presupuestadas, el equivalente a jornadas completas o los costes.

Las sobreasignaciones pueden aparecer cuando el valor de horas presupuestadas, FTE o costes de los recursos son superiores a las horas disponibles, FTE o costes. Esto genera un valor neto negativo.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td>
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p>
       <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a la administración de recursos que incluye acceso a Editar prioridades y horas presupuestadas en el Planificador de recursos</p> <p>Acceso de edición a datos financieros, proyectos y usuarios</p></td> 
  </tr> 
  <tr> 
   <td>Permisos de objeto</td> 
   <td> <p>Permisos de administración a los proyectos para los que desea presupuestar información con capacidad de Administrar finanzas</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ajustar fechas de presupuesto

1. Vaya al Planificador de recursos y seleccione **Ver por proyecto**.

   >[!NOTE]
   >
   >Solo puede utilizar la opción Ajustar fechas de presupuesto cuando vea el Planificador de recursos por proyecto.

1. Pase el puntero por encima del nombre de un proyecto y, a continuación, haga clic en el menú **Más**.
1. Haga clic en **Ajustar fechas de presupuesto**.\
   Se muestra la escala de tiempo de asignación del proyecto.\
   El lapso de tiempo en el que las horas están presupuestadas actualmente se resalta en naranja si hay un conflicto de presupuesto, y en azul si no hay conflictos.

   ![Ajustar fechas de presupuesto](assets/rp-adjust-budgeting-dates-with-no-done-button-350x63.png)

1. Arrastre y suelte el lapso de tiempo resaltado a otro momento para saber dónde no hay conflictos de presupuesto para el proyecto seleccionado. Cuando encuentre un lapso de tiempo en el que el valor neto sea positivo, el lapso de tiempo resaltado cambia a azul.
1. Haga clic en la “x” de la esquina superior derecha de la escala de tiempo de asignación del proyecto para cerrarla.
1. Elimine las horas presupuestadas de la escala de tiempo existente del proyecto y agréguelas a la escala de tiempo que muestre la mayor disponibilidad.
1. Haga clic en **Guardar**.
1. (Condicional y opcional) Si los lapsos de tiempo sin conflictos de presupuesto están fuera de la escala de tiempo del proyecto, haga clic en el nombre del proyecto para acceder a él.
1. (Condicional y opcional) Haga clic en **Editar proyecto** y, a continuación, modifique la **Fecha de inicio planificada** o la **Fecha de finalización planificada** para modificar la escala de tiempo del proyecto para el lapso de tiempo sin conflictos de presupuesto.\
   Para obtener más información sobre la edición de proyectos, consulte el artículo [Editar proyectos](../../manage-work/projects/manage-projects/edit-projects.md).

1. (Condicional y opcional) Haga clic en **Guardar cambios**.
1. Vuelva al Planificador de Recursos y vuelva a introducir los valores de Horas presupuestadas, FTE o Costes en el lapso de tiempo sin conflictos de presupuesto.
1. Haga clic en **Guardar**.
