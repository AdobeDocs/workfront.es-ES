---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular costo presupuestado de trabajo programado (BCWS)
description: También conocido como valor planeado, el costo presupuestado del trabajo programado (BCWS) es una métrica de rendimiento del proyecto que representa la cantidad de tarea que debería haberse completado en el momento en que se calcula esta métrica.
author: Alina
feature: Work Management
exl-id: b9a36333-9430-42bd-99dd-3ad82803b633
source-git-commit: 1d5de5ff0ebebd84482507c71730cfbd05c513a5
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 0%

---

# Calcular costo presupuestado de trabajo programado (BCWS)

## Visión General del Coste de Trabajo Presupuestado Programado (BCWS)

También conocido como valor planeado, el costo presupuestado del trabajo programado (BCWS) es una métrica de rendimiento del proyecto que representa la cantidad de tarea que debería haberse completado en el momento en que se calcula esta métrica.

Adobe Workfront calcula el costo presupuestado del trabajo programado (BCWS) tanto para proyectos como para tareas.

Tenga en cuenta lo siguiente al revisar los valores de BCWS en una tarea o proyecto:

* Workfront calcula el CPTP de una tarea en función de su configuración para el método de índice de rendimiento (PIM) del proyecto.

   Puede configurar el proyecto para que calcule el PIM utilizando horas o coste, y el BCWS también se calcula utilizando los mismos valores.

   Para obtener información sobre cómo se calcula el CPTP, consulte la sección [Configurar cómo se calcula el CPTP](#configure-how-bcws-is-calculated) en este artículo.

* Workfront calcula el CPTP de un proyecto añadiendo todos los valores de CPTP de todas las tareas principales y tareas individuales del proyecto.

   Los valores de las tareas secundarias no se agregan al CPTP del proyecto.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos</p> <p>Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para el proyecto</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Configurar cómo se calcula el CPTP {#configure-how-bcws-is-calculated}

Puede configurar si el CPTP se calcula en horas o en costes configurando cómo se calcula el método de índice de rendimiento (PIM) del proyecto.

1. Vaya a un proyecto y haga clic en **Detalles del proyecto** en el panel izquierdo.
1. En el **Finanzas** , ubique la variable **Método de índice de rendimiento** y haga doble clic en él para editarlo.

   ![](assets/pim-options-hour-cost-based-nwe.png)

1. Seleccione entre las siguientes opciones:

   | Opción | Cómo se realiza el cálculo |
   |---|---|
   | Basado en horas | Workfront calcula el CPTP utilizando las horas planificadas de las tareas. |
   | Basado en costos | Workfront calcula el CPTP utilizando el coste planificado de las tareas. |


1. Haga clic en **Guardar cambios**.

   El CPTP de las tareas del proyecto se calcula mediante horas o costes.

## Calcular BCWS

Workfront calcula el costo presupuestado del trabajo programado (BCWS) para tareas o proyectos mediante las siguientes fórmulas:

```
Task BCWS = Planned Percent Complete x Task Budget
```

```
Project BCWS = SUM(BCWS values of all parent and individual tasks)
```

En este cálculo se utilizan los valores siguientes:

| Valor utilizado | Descripción del valor utilizado |
|---|---|
| Porcentaje completado planificado | Esto es lo que debe ser el porcentaje completado de la tarea mirando la cantidad de tiempo transcurrido entre el comienzo de la tarea y hoy. |
| Presupuesto de tareas | Este es el valor de las horas planificadas o el coste planificado de la tarea. |

Por ejemplo, si hoy es 12 de febrero y una tarea está programada para durar desde el 10 de febrero hasta el 20 de febrero, la tarea debe estar 20% completa hoy. Si el presupuesto de la tarea (costo planificado) es de 10.000 $, el CPTP de la tarea es:

```
Task BCWS = 20% x $10,000 = $2,000
```

## Localización del CPTP para un proyecto o una tarea

Puede ver el valor del Coste de trabajo presupuestado programado en un informe o lista, agregando la columna de CPTP a la vista.

1. Vaya a una lista de tareas o proyectos.
1. Expanda el **Ver** y seleccione **Nueva vista** o **Personalizar vista**.

1. Haga clic en **Agregar columna**.
1. En el **Mostrar en esta columna:** introducción de campo **BCWS** y haga clic en para seleccionarlo cuando aparezca en la lista.

   ![](assets/bcws-in-project-view.png)

1. Haga clic en **Guardar vista**.
1. La variable **BCWS** se muestra en la vista .
