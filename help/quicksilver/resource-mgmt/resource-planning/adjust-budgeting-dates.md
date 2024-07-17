---
product-area: resource-management
navigation-topic: resource-planning
title: Ajustar fechas de presupuesto en el Planificador de recursos
description: Si observa que hay sobreasignaciones de los recursos después de haberlos presupuestado en el Planificador de recursos, puede explorar escenarios hipotéticos moviendo las horas presupuestadas, el valor de ETC o los costos a otro lapso de tiempo. En función de los resultados de estos escenarios, puede ajustar las horas presupuestadas, los jornadas completas o los costos.
author: Alina
feature: Resource Management
exl-id: bc49d45a-73a5-4b02-9054-9c9dbb54224d
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '535'
ht-degree: 1%

---

# Ajustar fechas de presupuesto en el Planificador de recursos

Si observa que hay sobreasignaciones de los recursos después de haberlos presupuestado en el Planificador de recursos, puede explorar escenarios hipotéticos moviendo las horas presupuestadas, el valor de ETC o los costos a otro lapso de tiempo. En función de los resultados de estos escenarios, puede ajustar las horas presupuestadas, los jornadas completas o los costos.

Las sobreasignaciones pueden aparecer cuando las horas presupuestadas, el valor de ETC o los costos de los recursos son superiores a las horas, el valor de ETC o los costos disponibles. Esto genera un valor neto negativo.

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
   <td> <p>Editar acceso a Administración de recursos que incluye acceso a Editar prioridades y horas presupuestadas en el Planificador de recursos</p> <p>Editar acceso a datos financieros, proyectos y usuarios</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, vea <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administre permisos a los proyectos para los que desea presupuestar información con capacidad de Administrar finanzas</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Ajustar fechas de presupuesto

1. Vaya al Planificador de recursos y seleccione **Ver por proyecto**.

   >[!NOTE]
   >
   >Sólo puede utilizar la opción Ajustar fechas presupuestadas cuando vea el Planificador de recursos por proyecto.

1. Pase el ratón sobre el nombre de un proyecto y luego haga clic en el menú **Más**.
1. Haga clic en **Ajustar fechas de presupuesto**.\
   Se muestra la cronología de asignación del proyecto.\
   El lapso de tiempo en el que las horas están presupuestadas actualmente se resalta en naranja si hay un conflicto de presupuestación y en azul si no hay conflictos.

   ![](assets/rp-adjust-budgeting-dates-with-no-done-button-350x63.png)

1. Arrastre y suelte el lapso de tiempo resaltado en otro momento para saber si no hay conflictos de presupuestos para el proyecto seleccionado. Cuando encuentra un lapso de tiempo en el que el valor neto es positivo, el lapso de tiempo resaltado cambia a azul.
1. Haga clic en la &quot;x&quot; en la esquina superior derecha de la cronología de asignación de proyectos para cerrarla.
1. Elimine las horas presupuestadas de la cronología existente del proyecto y agréguelas a la cronología que muestre la mayor disponibilidad.
1. Haga clic en **Guardar**.
1. (Condicional y opcional) Si los períodos de tiempo sin conflictos de presupuesto están fuera de la escala de tiempo del proyecto, haga clic en el nombre del proyecto para tener acceso al mismo.
1. (Condicional y opcional) Haga clic en **Editar proyecto** y, a continuación, edite la **Fecha planificada de inicio** o la **Fecha planificada de finalización** para modificar la escala de tiempo del proyecto para el lapso de tiempo sin conflictos de presupuestación.\
   Para obtener más información acerca de la edición de proyectos, vea el artículo [Editar proyectos](../../manage-work/projects/manage-projects/edit-projects.md).

1. (Condicional y opcional) Haga clic en **Guardar cambios**.
1. Vuelva al Planificador de Recursos y vuelva a introducir las horas presupuestadas, los jornadas completas o los costes en el lapso de tiempo sin conflictos de presupuesto.
1. Haga clic en **Guardar**.
