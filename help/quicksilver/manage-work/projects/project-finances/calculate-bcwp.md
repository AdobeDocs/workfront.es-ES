---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular costo presupuestado de trabajo realizado (CPTR)
description: También conocido como Valor acumulado, el Costo presupuestado del trabajo realizado (CPTR) es una métrica de rendimiento del proyecto que representa la cantidad de tarea que realmente se completó en el momento en que se calcula esta métrica.
author: Alina
feature: Work Management
exl-id: 203709a7-e522-4875-b3eb-40b967a938ec
source-git-commit: 1d5de5ff0ebebd84482507c71730cfbd05c513a5
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 2%

---

# Calcular costo presupuestado de trabajo realizado (CPTR)

## Visión General del Coste Presupuestado de Trabajo Realizado (CPTR)

También conocido como Valor acumulado, el Costo presupuestado del trabajo realizado (CPTR) es una métrica de rendimiento del proyecto que representa la cantidad de tarea que realmente se completó en el momento en que se calcula esta métrica.

Adobe Workfront calcula el costo presupuestado del trabajo realizado (CPTR) tanto para proyectos como para tareas.

Tenga en cuenta lo siguiente cuando revise los valores del CPTR de una tarea o proyecto:

* Workfront calcula el CPTR de una tarea en función de la configuración del Método de índice de rendimiento (PMI) del proyecto.

  Puede configurar el proyecto para que calcule el PMI mediante horas o costo y el CPTR también se calcula utilizando los mismos valores.

  Para obtener información acerca de cómo configurar el CPTR, vea la sección [Configurar cómo se calcula el CPTR](#configure-how-bcwp-is-calculated) en este artículo.

* Workfront calcula el CPTR de un proyecto agregando todos los valores del CPTR de todas las tareas principales y de las tareas individuales del proyecto.

  Los valores de las tareas secundarias no se agregan al CPTR del proyecto.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos</p> <p>Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos del proyecto</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Configurar cómo se calcula el CPTR {#configure-how-bcwp-is-calculated}

Puede configurar si el CPTR se calcula en horas o costos configurando cómo se calcula el método de índice de rendimiento (PIM) del proyecto.

1. Vaya a un proyecto y expanda **Detalles del proyecto** en el panel izquierdo.
1. En el área **Finanzas**, busque el campo **Método del índice de rendimiento** y haga doble clic para editarlo.

   ![](assets/pim-options-hour-cost-based-nwe.png)

1. Seleccione entre las siguientes opciones:

   | Opción | Cómo se realiza el cálculo |
   |---|---|
   | Basado en horas | Workfront calcula el CPTR utilizando las horas planificadas de las tareas. |
   | Basado en costos | Workfront calcula el CPTR utilizando el costo planificado de las tareas. |

1. Haga clic en **Guardar cambios**.

El CPTR de las tareas del proyecto se calcula mediante horas o costos.

## Calcular CPTR

Workfront calcula el costo presupuestado del trabajo realizado (CPTR) para una tarea o proyecto mediante las siguientes fórmulas:

```
Task BCWP = Actual Percent Complete x Task Budget
```

```
Project BCWP = SUM(BCWP values of all parent and individual tasks)
```

En estos cálculos se utilizan los siguientes valores:

| Valor utilizado | Descripción del valor utilizado |
|---|---|
| Porcentaje real completado | Es el porcentaje completado real de la tarea tal como aparece en Workfront. |
| Presupuesto de tareas | Es el valor de las horas planificadas o el costo planificado de la tarea. |

Por ejemplo, si el porcentaje completado real de la tarea es 25% y el presupuesto de la tarea o el costo planificado es 10.000 $, el CPTR de la tarea es:

```
BCWP = 25% x $10,000 = $2,500
```

## Busque el CPTR de un proyecto o tarea

Puede ver el valor del costo presupuestado del trabajo realizado en un informe o lista, agregando la columna CPTR a la vista.

1. Ir a una lista de tareas o proyectos.
1. Expanda el menú **Vista** y seleccione **Nueva vista** o **Personalizar vista**.

1. Haga clic en **Añadir columna**.
1. En el campo **Mostrar en esta columna:**, empiece a escribir **CPTR** y haga clic para seleccionarlo cuando se muestre en la lista.

   ![](assets/bcwp-project-view.png)

1. Pulse **Guardar vista**.
1. El campo CPTR se muestra en la vista.
