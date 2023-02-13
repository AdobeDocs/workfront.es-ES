---
product-area: resource-management
navigation-topic: resource-planning
title: Ajustar fechas de presupuesto en el planificador de recursos
description: Si descubre que hay sobreasignaciones de sus recursos después de haberlos presupuestado en el Planificador de recursos, puede explorar escenarios de alternativas moviendo las horas presupuestadas, los FTE o los costes a otro intervalo de tiempo. En función de los resultados de estos escenarios, puede ajustar las horas, los FTE o el coste presupuestados.
author: Alina
feature: Resource Management
exl-id: bc49d45a-73a5-4b02-9054-9c9dbb54224d
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '535'
ht-degree: 1%

---

# Ajustar fechas de presupuesto en el planificador de recursos

Si descubre que hay sobreasignaciones de sus recursos después de haberlos presupuestado en el Planificador de recursos, puede explorar escenarios de alternativas moviendo las horas presupuestadas, los FTE o los costes a otro intervalo de tiempo. En función de los resultados de estos escenarios, puede ajustar las horas, los FTE o el coste presupuestados.

Las sobreasignaciones pueden aparecer cuando las horas, los costes o los costes presupuestados de sus recursos sean superiores a las horas, los costes o los costes disponibles. Esto genera un valor neto negativo.

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Edite el acceso a la Administración de recursos que incluye acceso a Editar prioridades y horas de presupuesto en el Planificador de recursos</p> <p>Editar acceso a datos financieros, proyectos y usuarios</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administre los permisos de los proyectos para los que desea presupuestar información con capacidad para Administrar finanzas</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Ajustar fechas de presupuesto

1. Vaya al planificador de recursos y seleccione **Ver por proyecto**.

   >[!NOTE]
   >
   >La opción Ajustar fechas presupuestadas solo se puede usar cuando se vea el Planificador de recursos por proyecto.

1. Pase el ratón sobre el nombre de un proyecto y, a continuación, haga clic en la **Más** para abrir el Navegador.
1. Haga clic en **Ajustar fechas de presupuesto**.\
   Se muestra la cronología de asignación del proyecto.\
   El lapso de tiempo en el que las horas están presupuestadas actualmente se resalta en naranja si hay un conflicto presupuestario y en azul si no hay conflictos.

   ![](assets/rp-adjust-budgeting-dates-with-no-done-button-350x63.png)

1. Arrastre y suelte el lapso de tiempo resaltado en otro momento para comprender dónde no hay conflictos de presupuesto para el proyecto seleccionado. Cuando se encuentra un lapso de tiempo en el que el valor de Red es positivo, el lapso de tiempo resaltado cambia a azul.
1. Haga clic en la &quot;x&quot; en la esquina superior derecha de la cronología de asignación de proyectos para cerrarla.
1. Elimine las horas presupuestadas de la cronología existente del proyecto y agréguelas a la cronología que muestre la mayor disponibilidad.
1. Haga clic en **Guardar**.
1. (Condicional y opcional) Si los intervalos de tiempo sin conflictos de presupuesto están fuera de la cronología del proyecto, haga clic en el nombre del proyecto para acceder a él.
1. (Condicional y opcional) Haga clic en **Editar proyecto** y, a continuación, edite el **Fecha de inicio planeada** o **Fecha de finalización planeada** para modificar la cronología del proyecto para el lapso de tiempo sin conflictos de presupuesto.\
   Para obtener más información sobre la edición de proyectos, consulte el artículo [Editar proyectos](../../manage-work/projects/manage-projects/edit-projects.md).

1. (Condicional y opcional) Haga clic en **Guardar cambios**.
1. Vuelva al planificador de recursos y vuelva a introducir las horas, los FTE o los costes presupuestados en el lapso de tiempo sin conflictos presupuestarios.
1. Haga clic en **Guardar**.
