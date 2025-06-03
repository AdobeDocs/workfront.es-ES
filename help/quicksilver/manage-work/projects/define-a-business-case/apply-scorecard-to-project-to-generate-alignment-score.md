---
navigation-topic: business-case-and-scorecards
title: Aplicar un cuadro de resultados a un proyecto y generar una puntuación de alineación
description: Puede utilizar un cuadro de resultados para medir la alineación de un proyecto con los criterios de un portafolios establecidos anteriormente. Un cuadro de resultados suele reflejar la misión, los valores y las metas estratégicas de una organización.
author: Alina
feature: Work Management
exl-id: 21cf5493-147d-4b8d-8b16-2891eb7e0491
source-git-commit: 9cfb67f627c06a5926e820860d52ba9f1ab58bcf
workflow-type: tm+mt
source-wordcount: '1227'
ht-degree: 99%

---

# Aplicar un cuadro de resultados a un proyecto y generar una puntuación de alineación

<!-- Audited: 02/2024 -->

Puede utilizar un cuadro de resultados para medir la alineación de un proyecto con los criterios de un portafolios establecidos anteriormente. Un cuadro de resultados suele reflejar la misión, los valores y las metas estratégicas de una organización.

Para obtener más información sobre los cuadros de resultados y cómo crearlos, consulte [Crear un cuadro de resultados](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td>
   <p>Actual: Prime o superior</p>
   <p>o</p>
   <p>Heredado: Empresa o superior</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
   <p>Actual: Estándar</p>
   <p>o</p>
   <p>Heredado: plan</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a proyectos</p> <p>Acceso de visualización o superior a los portafolios</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td><p>Administración de permisos en un proyecto</p> <p>Permisos de visualización o superiores para un portafolio</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Cuadros de resultados del proyecto {#project-scorecards}

* [Información general sobre los cuadros de resultados](#scorecards-overview)
* [Aplicar un cuadro de resultados a un proyecto](#apply-a-scorecard-to-a-project)

### Información general de los cuadros de resultados {#scorecards-overview}

Normalmente, un administrador de proyectos completa la información del cuadro de resultados para generar un valor de alineación de entre 0 y 100 para el proyecto. El valor producido se utiliza posteriormente cuando el administrador del portafolios revisa los proyectos en el Optimizador de portafolios para compararlos.

Para obtener más información acerca de la optimización del portafolio, consulte [Información general sobre el optimizador de portafolios](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

### Aplicar un cuadro de resultados a un proyecto

Como usuario con una licencia estándar o de planificación y permisos de administración en un proyecto, puede adjuntar un cuadro de resultados al proyecto.

Para obtener más información acerca de los permisos del proyecto, consulte [Compartir un proyecto en Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

Puede añadir cuadros de resultados a un proyecto como parte de la creación del caso empresarial para el proyecto.

Para obtener más información sobre cómo crear un caso empresarial, consulte [Crear un caso empresarial para un proyecto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

El administrador de Adobe Workfront o del grupo debe habilitar la sección Cuadro de resultados en el área de Caso empresarial de sus proyectos para que pueda acceder a los cuadros de resultados desde el caso empresarial. Para obtener información sobre cómo configurar las preferencias de proyecto y habilitar áreas del caso empresarial, consulte [Configurar las preferencias de proyecto en todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Para aplicar un cuadro de resultados a un proyecto:

1. Vaya a un proyecto al que desee aplicar un cuadro de resultados.
1. Haga clic en **Caso empresarial** en el panel izquierdo.
1. Busque la sección **Cuadro de resultados** del caso empresarial.\
   Debe crear un cuadro de resultados antes de que se muestre la sección **Cuadro de resultados** en el caso empresarial.

   Para obtener información acerca de cómo crear un cuadro de resultados, consulte [Crear un cuadro de resultados](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

1. Seleccione un cuadro de resultados en el menú desplegable.

   ![Nuevo cuadro de resultados](assets/new-scorecard.png)

1. Escriba una respuesta para todas las preguntas del cuadro de resultados.

   Workfront aplica una puntuación a cada pregunta respondida y calcula una puntuación general del proyecto en función de la puntuación individual de cada pregunta.

   Para obtener más información sobre cómo generar la puntuación de alineación general del proyecto, consulte [Generar una puntuación de alineación para un proyecto](#generate-an-alignment-score-for-a-project).

1. Haga clic en **Guardar** para guardar el cuadro de resultados y puntuar el proyecto.

   El cuadro de resultados ahora está asociado con el proyecto y el proyecto se puntúa.

<!--This functionality was removed when we redesigned bulk editing projects with 23.2: 

1. (Conditional) When changes occur in the values of scorecard questions, you must recalculate the scorecard to reflect the new values for the project score. To recaulate the scorecard, do the following: 

   1. Go to a list of projects and select all projects in the list. 
   1. Click the **Edit** icon at the top of the list. 
   1. Click **Settings** in the left panel, then check the **Recalculate Scorecards** option at the end of the Settings area. 
   1. Click Save. This recalculates the score value based on the scorecards attached for all the selected projects.  

      >[!NOTE]
      >
      >   The option to recalculate scorecards has been removed from the Preview environment, when editing projects in bulk. 

-->

## Generación de una puntuación de alineación

* [Generar una puntuación de alineación para un proyecto](#generate-an-alignment-score-for-a-project)
* [Generar una puntuación de alineación para un portafolio](#generate-an-alignment-score-for-a-portfolio)

### Generación de una puntuación de alineación para un proyecto {#generate-an-alignment-score-for-a-project}

La puntuación de alineación es el valor producido después de completar el cuadro de resultados.

Los cuadros de resultados contienen preguntas con opciones de respuesta a las que se han asignado valores numéricos, denominados puntos de alineación. Estos puntos se utilizan para determinar cómo se alinea el proyecto con su organización. Los puntos de alineación de cada pregunta contienen un número entre 0 y 100.

Cuando se finaliza el cuadro de resultados, Workfront calcula la puntuación de alineación del proyecto como un porcentaje, utilizando la fórmula siguiente:

`Project Alignment Score = The sum of the question points from the scorecard met at a given time / The sum of the possible points on the scorecard`

Para obtener más información, consulte [Crear un cuadro de resultados](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

### Generar una puntuación de alineación para un portafolio {#generate-an-alignment-score-for-a-portfolio}

La puntuación de alineación del portafolios es un promedio de las puntuaciones de alineación de todos los proyectos del portafolios.

Cuando se completan los cuadros de resultados de los proyectos, Workfront utiliza esos valores para calcular la puntuación de alineación del portafolios como porcentaje, mediante la fórmula siguiente:

`Portfolio Alignment Score = The sum of the percentages of the project alignment scores / Number of projects in the portfolio`

>[!NOTE]
>
>Si un proyecto no tiene asociado un cuadro de resultados y, por lo tanto, no tiene una puntuación de alineación, se considera que tiene una alineación del 0 % en el portafolios. El proyecto se tiene en cuenta en el número de proyectos del portafolios.

## Visualización de la puntuación de alineación

Puede ver la puntuación de alineación de un proyecto a nivel de proyecto o en el Optimizador de portafolios.

* [Ver la puntuación de alineación en un proyecto](#view-the-alignment-score-on-a-project)
* [Vea las puntuaciones de alineación del proyecto y del portafolios en el Optimizador de portafolios](#view-the-alignment-scores-of-the-project-and-of-the-portfolio-in-the-portfolio-optimizer)

### Visualización de la puntuación de alineación en un proyecto

Puede ver la puntuación de alineación de un proyecto en el nivel de proyecto si tiene derechos de aportación para el proyecto.

1. Vaya al proyecto cuya puntuación de alineación desee ver.
1. Haga clic en **Caso empresarial** en el panel izquierdo.
1. Vaya a **Resumen del caso empresarial** al lado derecho de la pantalla.

   La puntuación de alineación se encuentra en el resumen del caso empresarial, en el valor **Alineado**.

   ![Puntuación de alineación en un proyecto](assets/alignment-score-on-a-project.png)

### Vea las puntuaciones de alineación del proyecto y del portafolios en el Optimizador de portafolios

Puede ver la puntuación de alineación de un proyecto o de un portafolios en el Optimizador de portafolios si tiene acceso de administración al portafolios.

Para obtener más información acerca de la información mostrada en el Optimizador de portafolios, consulte [Información general sobre el Optimizador de portafolios](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* [Busque la puntuación de alineación del proyecto en el Optimizador de portafolios](#locate-the-alignment-score-of-the-project-in-the-portfolio-optimizer)
* [Busque la puntuación de alineación del portafolios en el Optimizador de portafolios](#locate-the-alignment-score-of-the-portfolio-in-the-portfolio-optimizer)

  ![Puntuación de alineación en el Optimizador de portafolios](assets/alignment-score-in-portfolio-optimizer.png)

#### Busque la puntuación de alineación del proyecto en el Optimizador de portafolios {#locate-the-alignment-score-of-the-project-in-the-portfolio-optimizer}

{{step1-to-portfolios}}

1. Haga clic en el nombre de un portafolio.
1. Haga clic en **optimización del portafolio** en el panel izquierdo.

   Se muestra el Optimizador de portafolios.

   La puntuación de alineación de un proyecto se muestra como un porcentaje en la columna **Alineación** del Optimizador de portafolios.

   Esta es la puntuación de alineación del proyecto basada en el cuadro de resultados asociado al proyecto.

#### Busque la puntuación de alineación del portafolios en el Optimizador de portafolios  {#locate-the-alignment-score-of-the-portfolio-in-the-portfolio-optimizer}

{{step1-to-portfolios}}

1. Haga clic en el nombre de un portafolio.
1. Haga clic en **Optimización del portafolio** en el panel de la izquierda.
1. En la parte superior del Optimizador de portafolios se encuentra el valor **Alineado**, así como el indicador **Alineación**, que indica la puntuación de alineación del portafolios.

   Esta es la puntuación de alineación del portafolios.

   Para obtener más información sobre cómo se genera la puntuación de alineación de un portafolios, consulte [Generar una puntuación de alineación para un portafolios](#generate-an-alignment-score-for-a-portfolio).

## Información general de la puntuación del Optimizador de portafolios

Hay una diferencia entre la puntuación de alineación y la puntuación del Optimizador de portafolios de un proyecto.

La puntuación de alineación de un proyecto se calcula según los puntos obtenidos tras completar el cuadro de resultados. A continuación, esta puntuación se utiliza para determinar la puntuación de alineación del portafolios. La puntuación de alineación se muestra como un porcentaje.

La puntuación de alineación de un proyecto se muestra en la columna **Alineación** del Optimizador de portafolios.

La puntuación del Optimizador de portafolios es una clasificación calculada automáticamente en el Optimizador de portafolios mediante la cual se pueden priorizar los proyectos. La puntuación del Optimizador de portafolios se muestra como un icono indicador acompañado de un número y se muestra en la columna **Puntuación** del Optimizador de portafolios Solo se genera una puntuación del Optimizador de portafolios cuando se completan todas las secciones del caso empresarial, excepto las metas.

Para obtener más información sobre cómo crear un caso empresarial para un proyecto, consulte [Crear un caso empresarial para un proyecto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Para obtener más información sobre cómo calcular la puntuación del Optimizador de portafolios de un proyecto, consulte [Información general sobre la puntuación del Optimizador de portafolios](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md).
