---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular coste presupuestado de trabajo programado (CPTP)
description: También conocido como Valor planificado, el Coste presupuestado de trabajo programado (CPTP) es una métrica de rendimiento del proyecto que representa la cantidad de la tarea que debería haberse completado en el momento en que se calcula esta métrica.
author: Lisa
feature: Work Management
exl-id: b9a36333-9430-42bd-99dd-3ad82803b633
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 100%

---

# Calcular coste presupuestado de trabajo programado (CPTP)

## Información general de coste presupuestado de trabajo programado (CPTP)

También conocido como Valor planificado, el Coste presupuestado de trabajo programado (CPTP) es una métrica de rendimiento del proyecto que representa la cantidad de la tarea que debería haberse completado en el momento en que se calcula esta métrica.

Adobe Workfront calcula el coste presupuestado de trabajo programado (CPTP) tanto para proyectos como para tareas.

Tenga en cuenta lo siguiente cuando revise los valores del CPTP en una tarea o proyecto:

* Workfront calcula el CPTP de una tarea en función de la configuración del Método de índice de rendimiento (PIM) del proyecto.

  Puede configurar el proyecto para que calcule el PIM mediante horas o coste, y que el CPTP se calcule también utilizando los mismos valores.

  Para obtener información acerca de cómo configurar el CPTP, consulte la sección [Configurar cómo se calcula el CPTP](#configure-how-bcws-is-calculated) en este artículo.

* Workfront calcula el CPTP de un proyecto añadiendo todos los valores de CPTP de todas las tareas principales y de las tareas individuales del proyecto.

  Los valores de las tareas secundarias no se añaden al CPTP del proyecto.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
   <p>Nuevo: estándar</p>
   <p>o</p>
   <p>Actual: plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>Acceso de edición a proyectos</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td>Administrar permisos del proyecto</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar cómo se calcula el CPTP {#configure-how-bcws-is-calculated}

Puede configurar si el CPTP se calcula en horas o costes configurando cómo se calcula el Método de índice de rendimiento (PIM) del proyecto.

1. Vaya a un proyecto y haga clic en **Detalles del proyecto** en el panel izquierdo.
1. En el área **Finanzas**, busque el campo **Método de índice de rendimiento** y haga doble clic en él para editarlo.

   ![](assets/pim-options-hour-cost-based-nwe.png)

1. Seleccione entre las siguientes opciones:

   | Opción | Cómo se realiza el cálculo |
   |---|---|
   | Basado en horas | Workfront calcula el CPTP utilizando las horas planificadas de las tareas. |
   | Basado en costes | Workfront calcula el CPTP utilizando el coste planificado de las tareas. |


1. Haga clic en **Guardar cambios**.

   El CPTP de las tareas del proyecto se calcula mediante horas o costes.

## Calcular el CPTP

Workfront calcula el coste presupuestado de trabajo programado (CPTP) para las tareas o los proyectos mediante las siguientes fórmulas:

```
Task BCWS = Planned Percent Complete x Task Budget
```

```
Project BCWS = SUM(BCWS values of all parent and individual tasks)
```

En este cálculo se utilizan los siguientes valores:

| Valor utilizado | Descripción del valor utilizado |
|---|---|
| Porcentaje completado planificado | Este es el porcentaje completado de la tarea cuando se observa la cantidad de tiempo transcurrido entre el inicio de la tarea y hoy. |
| Presupuesto de la tarea | Es el valor de las horas planificadas o el coste planificado de la tarea. |

Por ejemplo, si hoy es 12 de febrero y una tarea está programada para durar del 10 al 20 de febrero, la tarea debería estar completada al 20 %. Si el presupuesto de la tarea (coste planificado) es de 10.000 dólares, el CPTP de la tarea es:

```
Task BCWS = 20% x $10,000 = $2,000
```

## Localizar el CPTP de un proyecto o una tarea

Puede ver el valor del coste presupuestado del trabajo programado en un informe o lista, añadiendo la columna CPTP a la vista.

1. Vaya a una lista de tareas o proyectos.
1. Expanda el menú **Vista** y seleccione **Nueva vista** o **Personalizar vista**.

1. Haga clic en **Añadir columna**.
1. En el campo **Mostrar en esta columna:**, empiece a escribir **BCWS** y haga clic para seleccionarlo cuando se muestre en la lista.

   ![](assets/bcws-in-project-view.png)

1. Haga clic en **Guardar vista**.
1. El campo **CPTP** se muestra en la vista.
