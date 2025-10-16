---
product-area: resource-management;projects
navigation-topic: resource-planning
title: Priorizar proyectos en el Planificador de recursos
description: Los proyectos se muestran en orden de prioridad en el Planificador de recursos, con el proyecto más importante en la parte superior.
author: Lisa
feature: Resource Management
exl-id: fe9c8cf9-f1e0-4cd5-9299-0f04893d71a5
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '1279'
ht-degree: 98%

---

# Priorizar proyectos en el Planificador de recursos

Los proyectos se muestran en orden de prioridad en el Planificador de recursos, con el proyecto más importante en la parte superior.

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

## Orden predeterminado de los proyectos en el Planificador de recursos

De manera predeterminada, los proyectos se enumeran en la vista de proyecto del Planificador de recursos teniendo en cuenta los criterios siguientes.

>[!IMPORTANT]
>
>Los proyectos se muestran de acuerdo con los tres criterios que aparecen a continuación, solamente la primera vez que abre el Planificador de recursos. Sin embargo, esta prioridad predeterminada se convierte automáticamente en su prioridad personalizada y no se puede revertir a la prioridad original cada vez que realice una de las siguientes acciones:
>
>* Al hacer clic en Guardar en cualquier momento.
>* Al cambiar manualmente la prioridad de planificación del proyecto. Para obtener información acerca de cómo cambiar manualmente la prioridad de planificación del proyecto, consulte la sección [Cambiar manualmente la prioridad de planificación del proyecto](#manually-change-the-project-planning-priority) en este artículo.
>
>Una vez que la prioridad del proyecto se convierta en su prioridad personalizada, los cambios en la información del proyecto ya no afectarán al orden de los proyectos según estos criterios. Después de esto, puede priorizar proyectos solo manualmente.

Los criterios predeterminados originales para enumerar los proyectos en la vista del proyecto son los siguientes, en este orden:

1. Por la puntuación de alineación en el proyecto.\
   Para obtener más información sobre la puntuación de alineación del proyecto, consulte [Aplicar un cuadro de resultados a un proyecto y generar una puntuación de alineación](../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md) .

1. En la fecha de inicio planificada del proyecto (si el campo de alineación es nulo o es el mismo para varios proyectos).
1. Alfabéticamente (si el campo Alineación es nulo o es el mismo y la Fecha de inicio planificada es la misma para varios proyectos).

Tenga en cuenta lo siguiente al trabajar con prioridades del proyecto en el Planificador de recursos:

* La prioridad del proyecto solo se puede personalizar manualmente al aplicar la vista del proyecto. Esto también cambia el orden de los proyectos en el Planificador de recursos.
* Al aplicar las vistas de función o de usuario en el Planificador de recursos, los proyectos aparecen en el mismo orden de prioridad establecido en la Vista del proyecto.
* El orden de los proyectos en el Planificador de recursos es exclusivo suyo. Otros usuarios pueden ver los mismos proyectos en el Planificador de recursos, pero en un orden diferente. No puede generar informes en el campo Prioridad de planificación del proyecto. Esto solo es visible en el Planificador de recursos y sirve como indicador para priorizar los proyectos.

Los proyectos asociados con un portafolio pueden tener una prioridad de nivel de portafolio. Puede habilitar la visualización de la prioridad de portafolio de un proyecto en el Planificador de recursos, además de la prioridad del Planificador de recursos. También puede ordenar los proyectos según su prioridad de portafolio.

## Cambiar manualmente la prioridad de planificación del proyecto {#manually-change-the-project-planning-priority}

Debe tener acceso de edición a la administración de recursos y permisos de administración a los proyectos para reordenar los proyectos en el Planificador de recursos.

Al dar una nueva prioridad a los proyectos, puede clasificarlos por orden de importancia.

Para editar la prioridad de planificación del proyecto:

1. Vaya al **Planificador de recursos**.

1. Haga clic dentro del campo a la izquierda del nombre del proyecto que contiene un número e introduzca un número para cambiar la prioridad de planificación y, a continuación, pulse Entrar.\
   ![Cambiar prioridad de planificación](assets/mceclip4.png)\
   O\
   Pase el puntero por encima del nombre del proyecto y haga clic en el indicador a la izquierda del nombre del proyecto, arrástrelo y suéltelo en el lugar correcto para cambiar la prioridad.

   ![drag_and_drop_projects_RP__1_.png](assets/drag-and-drop-projects-rp--1--350x184.png)

   Cuando seleccione números para priorizar proyectos, seleccione números más bajos para prioridades más altas (más importantes) y números más altos para prioridades más bajas (menos importantes). Cuando cambia el número de prioridad de un proyecto a un número inferior (prioridad superior), todos los demás proyectos del Planificador de recursos bajan en la lista (se vuelven menos importantes).\
   Cuando cambia el número de prioridad de un proyecto a un número superior (prioridad inferior), todos los demás proyectos del Planificador de recursos suben en la lista (y adquieren mayor importancia).

1. Haga clic en **Guardar**.\
   El orden de los proyectos cambia según sus selecciones y se convierte en su prioridad de proyecto personalizada en el Planificador de recursos. Otros usuarios no pueden ver el orden de prioridad de los proyectos en el Planificador de recursos, aunque es posible que puedan ver los mismos proyectos en sus Planificadores de recursos.

## Ordenar proyectos según su prioridad de portafolio en el Planificador de recursos

>[!IMPORTANT]
>
>Su empresa debe tener un plan empresarial o superior de Workfront para priorizar los proyectos en Optimizador de portafolios.
>
>Para obtener más información sobre los planes de Workfront, consulte [Nuestros planes](https://business.adobe.com/products/workfront/pricing.html).
>
>Para obtener información sobre cómo priorizar proyectos en Optimizador de portafolios, consulte [Priorizar proyectos en Optimizador de portafolios](../../manage-work/portfolios/portfolio-optimizer/prioritize-projects-in-portfolio-optimizer.md).

1. Abra el **Planificador de recursos** en la **Vista de proyecto**.
1. Haga clic en el icono **Configuración**.
1. Habilite la opción **Mostrar prioridades de portafolio** para mostrar las prioridades del proyecto según el portafolio al que estén asignadas. La prioridad de los proyectos según sus carteras se muestra junto a la prioridad del Planificador de recursos. Esta opción está desactivada de forma predeterminada.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: check screen shot to see if this is accurate still - should say Order, and not Sort:)</p>
   -->

   ![Prioridad de Portfolio](assets/rp-portfolio-priority-unordered-edit-350x180.png)

   Las prioridades del portafolio de los proyectos se muestran solamente en la vista Proyecto del Planificador de recursos.

1. Haga clic en **Ordenar** para ordenar los proyectos según las prioridades del portafolio.

   Si tiene proyectos que pertenecen a más de un portafolio, puede ver varios proyectos con la misma prioridad de portafolio en el Planificador de recursos. En este caso, los proyectos con la misma prioridad de portafolio se enumeran según los siguientes criterios, en este orden:

   1. Puntuación de alineación
   1. Fecha de inicio planificada
   1. Nombre del proyecto

   ![Prioridad de Portfolio ordenada](assets/rp-portfolio-priority-ordered-350x198.png)

1. Haga clic en **Guardar**.

## Efecto de cambiar la prioridad de planificación del proyecto en las horas disponibles del usuario

La prioridad de planificación del proyecto afecta a las horas disponibles de los usuarios. Los usuarios asociados al proyecto con la prioridad más alta muestran la disponibilidad más completa de la columna Horas disponibles (AVL) para este proyecto, según sus horarios.

Los mismos usuarios asociados con el segundo proyecto, por orden de prioridad, mostrarán un valor de Horas disponibles, que es la diferencia entre la cantidad completa de Horas disponibles y las que ya se han presupuestado para el primer proyecto en la columna Horas presupuestadas, y así sucesivamente. Para obtener información sobre cómo presupuestar recursos en el Planificador de recursos, consulte [Presupuestar recursos en el Planificador de recursos mediante las vistas Proyecto y Función](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

Si no se han presupuestado horas para el primer proyecto (en orden de prioridad) de un usuario, pero se han presupuestado horas para el segundo proyecto del mismo usuario, el usuario mostrará la cantidad completa de horas disponibles para ambos proyectos.

Se recomienda actualizar la columna Horas presupuestadas para los usuarios en el orden de los proyectos en el Planificador de recursos, a fin de garantizar que pueda ver con precisión las horas disponibles para el usuario en todo momento.

>[!NOTE]
>
>Debido a que la prioridad de planificación del proyecto es única para cada administrador de recursos, su segundo proyecto de prioridad podría ser un proyecto de primera prioridad para otro usuario que vea los mismos proyectos en su Planificador de recursos. Si otro administrador de recursos presupuesta un recurso para su primer proyecto, las horas disponibles disminuirán para ese recurso para el primer proyecto en función de ese cambio.
>
>El usuario que presupueste las horas primero asigna ese recurso y reduce el número de horas disponibles para ese recurso en todo el sistema. La cantidad de horas disponibles debe actualizarse para todos los usuarios en cuanto se guarden las horas presupuestadas de un recurso en el Planificador de recursos.
>
>Para obtener más información acerca de las horas disponibles, consulte [Disponibilidad y asignación de recursos](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md#availability-and-allocation-of-resources).
