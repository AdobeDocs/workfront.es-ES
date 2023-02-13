---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular el índice de rendimiento de la programación (SPI)
description: El Índice de Rendimiento de Programación (SPI) describe la relación entre la programación planificada y la programación real.
author: Alina
feature: Work Management
exl-id: 38259774-f22b-4b69-9e22-5b541118a7de
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 0%

---

# Calcular el índice de rendimiento de la programación (SPI)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

El Índice de Rendimiento de Programación (SPI) describe la relación entre la programación planificada y la programación real. Adobe Workfront calcula el SPI en los niveles de proyecto y tarea. Los administradores de proyectos revisan esta métrica para identificar si las tareas o los proyectos están realizando un seguimiento antes o después de lo programado.

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
   <td> <p>Revisar o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Ver acceso a Proyectos y Datos Financieros</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver o permisos superiores del proyecto con permisos para Ver finanzas</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Información general sobre el Índice de Rendimiento del Programa (SPI)

* [Qué muestra el valor de SPI](#what-the-spi-value-shows)
* [Cómo calcula Workfront SPI](#how-workfront-calculates-spi)

### Qué muestra el valor de SPI {#what-the-spi-value-shows}

Los administradores de proyectos entienden que un valor de SPI de 1 significa que el proyecto está planificado o planificado.  Los valores buenos a la 1 indican que un proyecto está por delante de la programación y los valores inferiores a 1 indican que un proyecto está por detrás de la programación.  Además del 1, la buena desviación del plan.

| **Valor de SPI** | **Indicación de &quot;según lo programado&quot;** |
|---|---|
| 1 | Según el plan o según el calendario |
| > 1 (bueno que 1) | Antes de la programación |
| &lt; 1 (menor que 1) | Retraso de programación |

{style=&quot;table-layout:auto&quot;}

### Cómo calcula Workfront SPI  {#how-workfront-calculates-spi}

Workfront calcula el SPI mediante la fórmula siguiente:

```
SPI = (Total Planned Hours x % Complete) / Planned Hours Scheduled to Date*
```

*&#42;Si las horas programadas están programadas para la fecha = 0, SPI = 1*.

Horario planificado El programa hasta la fecha se calcula en el minuto en que se realizan los cálculos. Muestra la cantidad de horas planeadas planeadas hasta la fecha actual. Se puede volver a calcular automáticamente cuando cambie los datos financieros para que sean precisos. No hay ningún campo en Workfront que indique este valor.

Por ejemplo, si tiene un proyecto con 1 tarea y la tarea tiene 10 horas planificadas y una duración de 10 días, el Horario planificado programado programado hasta la fecha del quinto día es 5. 

## Localización de SPI en un proyecto o tarea

1. Vaya al proyecto o tarea en el que desea ver el SPI.
1. Dependiendo de si desea ver SPI en un proyecto o una tarea, realice una de las siguientes acciones:

   1. Haga clic en **Detalles del proyecto** en el panel izquierdo y, a continuación, vea la **Finanzas** .

   1. Haga clic en **Detalles de la tarea** en el panel izquierdo y, a continuación, vea la **Finanzas** .

      ![](assets/spi-on-project-nwe.png)

1. Busque la **CPI/ SPI/ CSI** campo .
