---
product-area: resource-management;projects
navigation-topic: resource-planning
title: Priorizar los proyectos en el planificador de recursos
description: Los proyectos se enumeran por orden de prioridad en el Planificador de recursos con el proyecto más importante en la parte superior.
author: Alina
feature: Resource Management
exl-id: fe9c8cf9-f1e0-4cd5-9299-0f04893d71a5
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '1330'
ht-degree: 1%

---

# Priorizar los proyectos en el planificador de recursos

Los proyectos se enumeran por orden de prioridad en el Planificador de recursos con el proyecto más importante en la parte superior.

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

## Orden predeterminado de los proyectos en el planificador de recursos

De forma predeterminada, los proyectos se enumeran en la vista de proyecto del planificador de recursos teniendo en cuenta los criterios siguientes.

>[!IMPORTANT]
>
>Los proyectos se enumeran según los tres criterios siguientes solo la primera vez que abra el Planificador de recursos. Sin embargo, esta prioridad predeterminada se convierte automáticamente en su prioridad personalizada y no se puede revertir a la prioridad original cada vez que realice una de las siguientes acciones:
>
>* Cuando haga clic en Guardar en cualquier momento.
>* Cuando cambia manualmente la prioridad de planificación del proyecto. Para obtener información sobre cómo cambiar manualmente la prioridad de planificación del proyecto, consulte la sección [Cambiar manualmente la prioridad de planificación del proyecto](#manually-change-the-project-planning-priority) en este artículo.
>
>Una vez que la prioridad del proyecto se convierta en su prioridad personalizada, cualquier cambio en la información del proyecto ya no afectará a la ordenación de los proyectos mediante estos criterios. Después de esto, puede priorizar los proyectos solo manualmente.

Los criterios predeterminados originales para enumerar los proyectos en la vista de proyecto son los siguientes, en este orden:

1. Por la puntuación de alineación del proyecto.\
   Para obtener más información sobre la puntuación de alineación del proyecto, consulte [Aplicar un informe de valoración a un proyecto y generar una puntuación de alineación](../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md) .

1. Por la Fecha de inicio planeada del proyecto (si el campo Alineación es nulo o es el mismo para varios proyectos).
1. Alfabéticamente (si el campo Alignment es nulo o es el mismo, y la fecha de inicio planeado es la misma para varios proyectos).

Tenga en cuenta lo siguiente cuando trabaje con prioridades de proyecto en el Planificador de recursos:

* La prioridad del proyecto solo se puede personalizar manualmente al aplicar la vista del proyecto. Esto también cambia el orden de los proyectos en el Planificador de recursos.
* Cuando se aplica la función o las vistas del usuario en el planificador de recursos, los proyectos aparecen en el mismo orden de prioridad establecido en la vista de proyecto.
* El orden de los proyectos en el planificador de recursos es único para usted. Otros usuarios pueden ver los mismos proyectos en el Planificador de recursos, pero en un orden diferente. No se puede informar sobre el campo Prioridad de Planificación de Proyectos . Esto es visible solo en el planificador de recursos y sirve como indicador para priorizar sus proyectos.

Los proyectos asociados a un portafolio pueden tener una prioridad de nivel de portafolio. Puede activar la visualización de la prioridad de portafolio de un proyecto en el Planificador de recursos, además de la prioridad Planificador de recursos. También puede ordenar los proyectos según su prioridad de portafolio.

## Cambiar manualmente la prioridad de planificación del proyecto {#manually-change-the-project-planning-priority}

Debe tener acceso de edición a Gestión de recursos y Administrar permisos para proyectos, para reordenar proyectos en el Planificador de recursos.

Al dar a los proyectos una nueva prioridad, puede clasificarlos por orden de importancia.

Para editar la prioridad de planificación del proyecto:

1. Vaya a la **Planificador de recursos**.

1. Haga clic dentro del campo a la izquierda del nombre del proyecto que contiene un número, introduzca un número para cambiar la prioridad de Planning y, a continuación, pulse Intro.\
   ![](assets/mceclip4.png)\
   O\
   Pase el ratón sobre el nombre del proyecto y haga clic en el indicador situado a la izquierda del nombre del proyecto, arrástrelo y suéltelo en el punto correcto para cambiar la prioridad.

   ![arrastre_and_drop_projects_RP_1_.png](assets/drag-and-drop-projects-rp--1--350x184.png)

   Cuando seleccione números para priorizar proyectos, seleccione números inferiores para prioridades superiores (más importantes) y números superiores para prioridades inferiores (menos importantes). Cuando cambia el número de prioridad de un proyecto a un número menor (prioridad superior), todos los demás proyectos del Planificador de recursos se desplazan hacia abajo en la lista (se vuelven menos importantes).\
   Cuando cambia el número de prioridad de un proyecto a un número mayor (prioridad inferior), todos los demás proyectos del Planificador de recursos se desplazan hacia arriba en la lista (lo que resulta más importante).

1. Haga clic en **Guardar**.\
   El orden de los proyectos cambia según sus selecciones y esto se convierte en su prioridad de proyecto personalizada en el Planificador de recursos. Otros usuarios no pueden ver el orden de prioridad de los proyectos en el planificador de recursos, aunque podrían ver los mismos proyectos en sus planificadores de recursos.

## Solicite proyectos según su prioridad de Portfolio en el planificador de recursos

>[!IMPORTANT]
>
>Su empresa debe tener un plan de Workfront empresarial o superior para priorizar los proyectos en Portfolio Optimizer.
>
>Para obtener más información sobre los planes de Workfront, consulte [Nuestros planes](https://www.workfront.com/plans).
>
>Para obtener información sobre la priorización de proyectos en Portfolio Optimizer, consulte [Priorizar los proyectos en Portfolio Optimizer](../../manage-work/portfolios/portfolio-optimizer/prioritize-projects-in-portfolio-optimizer.md).

1. Abra el **Planificador de recursos** en el **Vista de proyecto**.
1. Haga clic en el **Configuración** icono.
1. Active la variable **Mostrar las prioridades del Portfolio** para mostrar las prioridades del proyecto según el Portfolio al que estén asignados. La prioridad de los proyectos según sus portafolios se muestra junto a la prioridad Planificador de recursos . Esta configuración está deshabilitada de forma predeterminada.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: check screen shot to see if this is accurate still - should say Order, and not Sort:)</p>
   -->

   ![](assets/rp-portfolio-priority-unordered-edit-350x180.png)

   Las prioridades de portafolio de los proyectos solo se muestran en la vista Proyecto del Planificador de Recursos.

1. Haga clic en **Pedido** para ordenar los proyectos según las prioridades de la cartera.

   Si tiene proyectos que pertenecen a más de un portafolio, puede ver varios proyectos con la misma prioridad de portafolio en el Planificador de recursos. En este caso, los proyectos con la misma prioridad de portafolio se enumeran según los siguientes criterios, en este orden:

   1. Puntuación de alineación
   1. Fecha planificada de inicio
   1. Nombre del proyecto

   ![](assets/rp-portfolio-priority-ordered-350x198.png)

1. Haga clic en **Guardar**.

## El efecto de cambiar la prioridad de planificación de proyectos en las horas disponibles para el usuario

La prioridad de planificación de proyectos afecta a las horas disponibles de los usuarios. Los usuarios asociados con el proyecto con la prioridad más alta muestran su máxima disponibilidad para la columna Horario disponible (AVL) de este proyecto, según sus programaciones.

Los mismos usuarios asociados con el segundo proyecto en orden de prioridad mostrarán un valor de Horas disponibles , que es la diferencia entre su cantidad completa de Horas disponibles y lo que ya se ha presupuestado para el primer proyecto en la columna Horas presupuestadas, etc. Para obtener información sobre la presupuestación de recursos en el planificador de recursos, consulte [Recursos presupuestarios en el planificador de recursos utilizando las vistas Proyecto y Función](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

Si no se ha presupuestado ninguna hora para el primer proyecto (en orden de prioridad) para un usuario, pero se han presupuestado horas para el segundo proyecto para el mismo usuario, el usuario mostrará la cantidad completa de horas disponibles para ambos proyectos.

Se recomienda actualizar la columna Horario presupuestado para los usuarios en el orden de los proyectos en el Planificador de recursos para garantizar que pueda ver con precisión las horas disponibles para el usuario en todo momento.

>[!NOTE]
>
>Como la prioridad de planificación de proyectos es única para cada administrador de recursos, su segundo proyecto prioritario puede ser de primera prioridad para otro usuario que vea los mismos proyectos en su planificador de recursos. Si otro administrador de recursos presupuesta un recurso para su primer proyecto, las horas disponibles disminuirán para ese recurso para el primer proyecto en función de ese cambio.
>
>El usuario que presupuesta las horas asigna primero ese recurso y reduce el número de horas disponibles para ese recurso en todo el sistema. La cantidad de horas disponibles se debe actualizar para todos los usuarios en cuanto se guarden las horas presupuestadas para un recurso en el Planificador de recursos.
>
>Para obtener más información sobre las horas disponibles, consulte [Disponibilidad y asignación de recursos](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md#availability-and-allocation-of-resources).
