---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular el coste presupuestado de trabajo realizado (CPTR)
description: También conocido como Valor acumulado, el Coste presupuestado del trabajo realizado (CPTR) es una métrica de rendimiento del proyecto que representa la cantidad de tarea que realmente se completó en el momento en que se calcula esta métrica.
author: Lisa
feature: Work Management
exl-id: 203709a7-e522-4875-b3eb-40b967a938ec
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 98%

---

# Calcular el coste presupuestado de trabajo realizado (CPTR)

## Información general del Coste presupuestado del trabajo realizado (CPTR)

También conocido como Valor acumulado, el Coste presupuestado del trabajo realizado (CPTR) es una métrica de rendimiento del proyecto que representa la cantidad de tarea que realmente se completó en el momento en que se calcula esta métrica.

Adobe Workfront calcula el coste presupuestado del trabajo realizado (CPTR) tanto para proyectos como para tareas.

Tenga en cuenta lo siguiente cuando revise los valores del CPTR de una tarea o proyecto:

* Workfront calcula el CPTR de una tarea en función de la configuración del Método de índice de rendimiento (PMI) del proyecto.

  Puede configurar el proyecto para que calcule el PMI mediante horas o coste y el CPTR también se calcula utilizando los mismos valores.

  Para obtener información acerca de cómo configurar el CPTR, consulte la sección [Configurar cómo se calcula el CPTR](#configure-how-bcwp-is-calculated) en este artículo.

* Workfront calcula el CPTR de un proyecto añadiendo todos los valores del CPTR de todas las tareas principales y de las tareas individuales del proyecto.

  Los valores de las tareas secundarias no se añaden al CPTR del proyecto.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>paquete de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td>
   <p>Estándar</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>Acceso de edición a proyectos</td> 
  </tr> 
  <tr> 
   <td>Permisos de objeto</td> 
   <td>Administrar permisos del proyecto</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar cómo se calcula el CPTR {#configure-how-bcwp-is-calculated}

Puede configurar si el CPTR se calcula en horas o costes configurando cómo se calcula el método de índice de rendimiento (PIM) del proyecto.

1. Vaya a un proyecto y expanda **Detalles del proyecto** en el panel izquierdo.
1. En el área **Finanzas**, busque el campo **Método del índice de rendimiento** y haga doble clic para editarlo.

   ![Opciones de PIM](assets/pim-options-hour-cost-based-nwe.png)

1. Seleccione entre las siguientes opciones:

   | Opción | Cómo se realiza el cálculo |
   |---|---|
   | Basado en horas | Workfront calcula el CPTR utilizando las horas planificadas de las tareas. |
   | Basado en costes | Workfront calcula el CPTR utilizando el coste planificado de las tareas. |

1. Haga clic en **Guardar cambios**.

   El CPTR de las tareas del proyecto se calcula mediante horas o costes.

## Calcular CPTR

Workfront calcula el coste presupuestado del trabajo realizado (CPTR) para una tarea o proyecto mediante las siguientes fórmulas:

```
Task BCWP = Actual Percent Complete x Task Budget
```

```
Project BCWP = SUM(BCWP values of all parent and individual tasks)
```

En estos cálculos se utilizan los siguientes valores:

| Valor utilizado | Descripción del valor utilizado |
|---|---|
| Porcentaje completado actual | Es el porcentaje completado real de la tarea, tal como aparece en Workfront. |
| Presupuesto de la tarea | Es el valor de las horas planificadas o el coste planificado de la tarea. |

Por ejemplo, si el porcentaje completado real de la tarea es 25% y el presupuesto de la tarea o el coste planificado es 10.000 $, el CPTR de la tarea es:

```
BCWP = 25% x $10,000 = $2,500
```

## Buscar el CPTR de un proyecto o tarea

Puede ver el valor del coste presupuestado del trabajo realizado en un informe o lista, añadiendo la columna CPTR a la vista.

1. Vaya a una lista de tareas o proyectos.
1. Expanda el menú **Vista** y seleccione **Nueva vista** o **Personalizar vista**.

1. Haga clic en **Añadir columna**.
1. En el campo **Mostrar en esta columna:**, empiece a escribir **CPTR** y haga clic para seleccionarlo cuando se muestre en la lista.

   ![CPTR en la vista de proyecto](assets/bcwp-project-view.png)

1. Haga clic en **Guardar vista**.
1. El campo CPTR se muestra en la vista.
