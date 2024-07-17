---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular costo presupuestado de trabajo programado (CPTP)
description: También conocido como Valor planificado, el Costo presupuestado del trabajo programado (CPTP) es una métrica de rendimiento del proyecto que representa la cantidad de la tarea que debería haberse completado en el momento en que se calcula esta métrica.
author: Alina
feature: Work Management
exl-id: b9a36333-9430-42bd-99dd-3ad82803b633
source-git-commit: 1d5de5ff0ebebd84482507c71730cfbd05c513a5
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 2%

---

# Calcular costo presupuestado de trabajo programado (CPTP)

## Visión General del Costo Presupuestado de Trabajo Programado (CPTP)

También conocido como Valor planificado, el Costo presupuestado del trabajo programado (CPTP) es una métrica de rendimiento del proyecto que representa la cantidad de la tarea que debería haberse completado en el momento en que se calcula esta métrica.

Adobe Workfront calcula el costo presupuestado del trabajo programado (CPTP) tanto para proyectos como para tareas.

Tenga en cuenta lo siguiente cuando revise los valores del CPTP en una tarea o proyecto:

* Workfront calcula el CPTP de una tarea en función de la configuración del Método de índice de rendimiento (PIM) del proyecto.

  Puede configurar el proyecto para que calcule el PIM mediante horas o costo y el CPTP también se calcula utilizando los mismos valores.

  Para obtener información acerca de cómo configurar el CPTP, vea la sección [Configurar cómo se calcula el CPTP](#configure-how-bcws-is-calculated) en este artículo.

* Workfront calcula el CPTP de un proyecto agregando todos los valores del CPTP de todas las tareas principales y de las tareas individuales del proyecto.

  Los valores de las tareas secundarias no se agregan al CPTP del proyecto.

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

## Configurar cómo se calcula el CPTP {#configure-how-bcws-is-calculated}

Puede configurar si el CPTP se calcula en horas o costos configurando cómo se calcula el método de índice de rendimiento (PIM) del proyecto.

1. Vaya a un proyecto y haga clic en **Detalles del proyecto** en el panel izquierdo.
1. En el área **Finanzas**, busque el campo **Método del índice de rendimiento** y haga doble clic en él para editarlo.

   ![](assets/pim-options-hour-cost-based-nwe.png)

1. Seleccione entre las siguientes opciones:

   | Opción | Cómo se realiza el cálculo |
   |---|---|
   | Basado en horas | Workfront calcula el CPTP utilizando las horas planificadas de las tareas. |
   | Basado en costos | Workfront calcula el CPTP utilizando el costo planificado de las tareas. |


1. Haga clic en **Guardar cambios**.

   El CPTP de las tareas del proyecto se calcula mediante horas o costos.

## Calcular CPTP

Workfront calcula el costo presupuestado del trabajo programado (CPTP) para tareas o proyectos mediante las siguientes fórmulas:

```
Task BCWS = Planned Percent Complete x Task Budget
```

```
Project BCWS = SUM(BCWS values of all parent and individual tasks)
```

En este cálculo se utilizan los siguientes valores:

| Valor utilizado | Descripción del valor utilizado |
|---|---|
| Porcentaje planificado completado | Este es el porcentaje completado de la tarea al observar la cantidad de tiempo transcurrido entre el comienzo de la tarea y hoy. |
| Presupuesto de tareas | Es el valor de las horas planificadas o el costo planificado de la tarea. |

Por ejemplo, si hoy es 12 de febrero y una tarea está programada para durar del 10 al 20 de febrero, la tarea debería estar completada al 20 %. Si el presupuesto de la tarea (costo planificado) es de 10.000 $, el CPTP de la tarea es:

```
Task BCWS = 20% x $10,000 = $2,000
```

## Busque el CPTP para un proyecto o una tarea

Puede ver el valor del costo presupuestado del trabajo programado en un informe o lista, agregando la columna CPTP a la vista.

1. Ir a una lista de tareas o proyectos.
1. Expanda el menú **Vista** y seleccione **Nueva vista** o **Personalizar vista**.

1. Haga clic en **Añadir columna**.
1. En el campo **Mostrar en esta columna:** empiece a escribir **BCWS** y haga clic para seleccionarlo cuando se muestre en la lista.

   ![](assets/bcws-in-project-view.png)

1. Pulse **Guardar vista**.
1. El campo **BCWS** se muestra en la vista.
