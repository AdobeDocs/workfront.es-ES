---
navigation-topic: business-case-and-scorecards
title: Aplicar un cuadro de resultados a un proyecto y generar una puntuación de alineación
description: Puede utilizar un cuadro de resultados para medir la alineación de un proyecto con los criterios de un portafolio establecidos anteriormente. Un cuadro de resultados suele reflejar la misión, los valores y los objetivos estratégicos de una organización.
author: Alina
feature: Work Management
exl-id: 21cf5493-147d-4b8d-8b16-2891eb7e0491
source-git-commit: db362bd73e51b30090708822876ad02f7804d064
workflow-type: tm+mt
source-wordcount: '1229'
ht-degree: 0%

---

# Aplicar un cuadro de resultados a un proyecto y generar una puntuación de alineación

<!-- Audited: 02/2024 -->

Puede utilizar un cuadro de resultados para medir la alineación de un proyecto con los criterios de un portafolio establecidos anteriormente. Un cuadro de resultados suele reflejar la misión, los valores y los objetivos estratégicos de una organización.

Para obtener más información sobre los cuadros de resultados y cómo crearlos, consulte [Crear un informe de valoración](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>
   <p>Nuevo: Prime o superior</p>
   <p>o</p>
   <p>Actual: Empresa o superior</p> </td>
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
   <td> <p>Editar acceso a Proyectos</p> <p>Acceso de visualización o superior a los Portfolio</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td><p>Administración de permisos en un proyecto</p> <p>Ver o permisos superiores de un portafolio</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Cuadros de resultados del proyecto {#project-scorecards}

* [Resumen de informes de valoración](#scorecards-overview)
* [Aplicar un cuadro de resultados a un proyecto](#apply-a-scorecard-to-a-project)

### Resumen de informes de valoración {#scorecards-overview}

Normalmente, un administrador de proyectos completa la información del cuadro de mandos para generar un valor de alineación entre 0 y 100 para el proyecto. El valor producido se utiliza posteriormente cuando el administrador de portafolios revisa los proyectos en el optimizador de portafolios para compararlos.

Para obtener más información sobre la optimización del portafolio, consulte [Información general de Portfolio Optimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

### Aplicar un cuadro de resultados a un proyecto

Como usuario con una licencia estándar o de planificación y permisos de administración en un proyecto, puede adjuntar un cuadro de resultados al proyecto.

Para obtener más información sobre los permisos del proyecto, consulte [Uso compartido de un proyecto en Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

Puede agregar cuadros de resultados a un proyecto como parte de la creación del caso empresarial para el proyecto.

Para obtener más información sobre la creación de un caso empresarial, consulte [Crear un caso comercial para un proyecto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

El administrador de Adobe Workfront o del grupo debe habilitar la sección Informe de valoración en el área de Caso comercial de sus proyectos para que pueda acceder a los informes de valoración desde el Caso comercial. Para obtener información sobre la configuración de preferencias de proyecto y la habilitación de áreas del caso empresarial, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Para aplicar un cuadro de resultados a un proyecto:

1. Vaya a un proyecto al que desee aplicar un cuadro de mandos.
1. Clic **Caso comercial** en el panel izquierdo.
1. Busque el **Informe de valoración** de la sección de caso comercial.\
   Debe crear un informe de valoración antes de la **Informe de valoración** La sección se muestra en el caso comercial.

   Para obtener información sobre cómo crear un cuadro de mandos, consulte [Crear un informe de valoración](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

1. Seleccione un informe de valoración en el menú desplegable.

   ![Nuevo cuadro de resultados](assets/new-scorecard.png)

1. Escriba una respuesta para todas las preguntas del informe de valoración.

   Workfront aplica una puntuación a cada pregunta respondida y calcula una puntuación general del proyecto en función de la puntuación individual de cada pregunta.

   Para obtener más información sobre la generación de la puntuación de alineación general del proyecto, consulte [Generación de una puntuación de alineación para un proyecto](#generate-an-alignment-score-for-a-project).

1. Clic **Guardar** para guardar el cuadro de resultados y puntuar el proyecto.

   El cuadro de resultados ahora está asociado con el proyecto y se puntúa el proyecto.

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

* [Generación de una puntuación de alineación para un proyecto](#generate-an-alignment-score-for-a-project)
* [Generación de una puntuación de alineación para un portafolio](#generate-an-alignment-score-for-a-portfolio)

### Generación de una puntuación de alineación para un proyecto {#generate-an-alignment-score-for-a-project}

La puntuación de alineación es el valor producido después de completar el cuadro de resultados.

Los informes de valoración contienen preguntas con opciones de respuesta a las que se les han asignado valores numéricos, denominados puntos de alineación. Estos puntos se utilizan para determinar cómo se alinea el proyecto con su organización. Los puntos de alineación de cada pregunta contienen un número entre 0 y 100.

Cuando finaliza el cuadro de resultados, Workfront calcula la puntuación de alineación del proyecto como un porcentaje, utilizando la fórmula siguiente:

`Project Alignment Score = The sum of the question points from the scorecard met at a given time / The sum of the possible points on the scorecard`

Para obtener más información, consulte [Crear un informe de valoración](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

### Generación de una puntuación de alineación para un portafolio {#generate-an-alignment-score-for-a-portfolio}

La puntuación de alineación del portafolio es un promedio de las puntuaciones de alineación de todos los proyectos del portafolio.

Cuando se completan los cuadros de resultados de los proyectos, Workfront utiliza esos valores para calcular la puntuación de alineación del portafolio como porcentaje, mediante la fórmula siguiente:

`Portfolio Alignment Score = The sum of the percentages of the project alignment scores / Number of projects in the portfolio`

>[!NOTE]
>
>Si un proyecto no tiene asociado un informe de valoración y, por lo tanto, no tiene una puntuación de alineación, se considera que tiene una alineación del 0% en el portafolio. El proyecto se tiene en cuenta en el número de proyectos del portafolio.

## Visualización de la puntuación de alineación

Puede ver la puntuación de alineación de un proyecto en el nivel de proyecto o en Portfolio Optimizer.

* [Visualización de la puntuación de alineación en un proyecto](#view-the-alignment-score-on-a-project)
* [Vea las puntuaciones de alineación del proyecto y del portafolio en Portfolio Optimizer](#view-the-alignment-scores-of-the-project-and-of-the-portfolio-in-the-portfolio-optimizer)

### Visualización de la puntuación de alineación en un proyecto

Puede ver la puntuación de alineación de un proyecto en el nivel de proyecto si tiene derechos de contribución sobre el proyecto.

1. Vaya al proyecto cuya puntuación de alineación desee ver.
1. Clic **Caso comercial** en el panel izquierdo.
1. Vaya a la **Resumen de caso comercial** en el lado derecho de la pantalla.

   La puntuación de alineación se encuentra en el resumen del caso empresarial, en la variable **Alineado** valor.

   ![Puntuación de alineación en un proyecto](assets/alignment-score-on-a-project.png)

### Vea las puntuaciones de alineación del proyecto y del portafolio en Portfolio Optimizer

Puede ver la puntuación de alineación de un proyecto o de un portafolio en Portfolio Optimizer si tiene acceso de Administración al portafolio.

Para obtener más información sobre la información mostrada en Portfolio Optimizer, consulte [Información general de Portfolio Optimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* [Busque la puntuación de alineación del proyecto en Portfolio Optimizer](#locate-the-alignment-score-of-the-project-in-the-portfolio-optimizer)
* [Busque la puntuación de alineación del portafolio en Portfolio Optimizer](#locate-the-alignment-score-of-the-portfolio-in-the-portfolio-optimizer)

  ![Puntuación de alineación en Portfolio Optimizer](assets/alignment-score-in-portfolio-optimizer.png)

#### Busque la puntuación de alineación del proyecto en Portfolio Optimizer {#locate-the-alignment-score-of-the-project-in-the-portfolio-optimizer}

{{step1-to-portfolios}}

1. Haga clic en el nombre de un portafolio.
1. Clic **Optimización de Portfolio** en el panel izquierdo.

   Se muestra Portfolio Optimizer.

   La puntuación de alineación de un proyecto se muestra como un porcentaje en la variable **Alineación** de Portfolio Optimizer.

   Esta es la puntuación de alineación del proyecto basada en el cuadro de resultados asociado al proyecto.

#### Busque la puntuación de alineación del portafolio en Portfolio Optimizer  {#locate-the-alignment-score-of-the-portfolio-in-the-portfolio-optimizer}

{{step1-to-portfolios}}

1. Haga clic en el nombre de un portafolio.
1. Clic **Optimización de Portfolio** en el panel izquierdo.
1. En la parte superior de Portfolio Optimizer, encontrará lo siguiente **Alineado** , así como la variable **Alineación** medidor, que indica la puntuación de alineación del portafolio.

   Esta es la puntuación de alineación del portafolio.

   Para obtener más información sobre cómo se genera la puntuación de alineación de un portafolio, consulte [Generación de una puntuación de alineación para un portafolio](#generate-an-alignment-score-for-a-portfolio).

## Descripción general de la puntuación de Portfolio Optimizer

Hay una diferencia entre la puntuación de alineación y la puntuación del optimizador de portafolio de un proyecto.

La puntuación de alineación de un proyecto se calcula según los puntos obtenidos tras completar el cuadro de resultados. A continuación, esta puntuación se utiliza para determinar la puntuación de alineación del portafolio. La puntuación de alineación se muestra como un porcentaje.

La puntuación de alineación de un proyecto se muestra en la variable **Alineación** de Portfolio Optimizer.

La puntuación del optimizador de portafolios es una clasificación calculada automáticamente en Portfolio Optimizer mediante la cual se pueden priorizar los proyectos. La puntuación del optimizador de portafolios se muestra como un icono indicador acompañado de un número y se muestra en la **Puntuación** de Portfolio Optimizer. Solo se genera una puntuación de Portfolio Optimizer cuando se completan todas las secciones del caso empresarial, excepto los objetivos.

Para obtener más información sobre la creación de un caso empresarial para un proyecto, consulte [Crear un caso comercial para un proyecto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Para obtener más información sobre el cálculo de la puntuación del optimizador de portafolios de un proyecto, consulte [Descripción general de la puntuación de Portfolio Optimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md).
