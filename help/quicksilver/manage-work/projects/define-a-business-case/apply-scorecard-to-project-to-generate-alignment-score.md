---
navigation-topic: business-case-and-scorecards
title: Aplicar un informe de valoración a un proyecto y generar una puntuación de alineación
description: Puede utilizar un informe de valoración para medir cómo se alinea un proyecto con los criterios establecidos anteriormente para un portafolio. Un informe de valoración a menudo refleja la misión, los valores y los objetivos estratégicos de una organización.
author: Alina
feature: Work Management
exl-id: 21cf5493-147d-4b8d-8b16-2891eb7e0491
source-git-commit: 78878fa3578e4f3a33baec3806298282d3909d8d
workflow-type: tm+mt
source-wordcount: '1292'
ht-degree: 0%

---

# Aplicar un informe de valoración a un proyecto y generar una puntuación de alineación

Puede utilizar un informe de valoración para medir cómo se alinea un proyecto con los criterios establecidos anteriormente para un portafolio. Un informe de valoración a menudo refleja la misión, los valores y los objetivos estratégicos de una organización.

Para obtener más información sobre los informes de valoración y cómo crear uno, consulte [Crear un informe de valoración](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Negocios o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos</p> <p>Ver o acceso superior a los Portfolio</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en un proyecto</p> <p>Ver o permisos superiores de un portafolio </p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Informes de valoración del proyecto {#project-scorecards}

* [Información general sobre los informes de valoración](#scorecards-overview)
* [Informes de valoración del proyecto](#project-scorecards)

### Información general sobre los informes de valoración {#scorecards-overview}

Normalmente, un administrador de proyectos completa la información del informe de valoración para producir un valor de alineación entre 0 y 100 para el proyecto. El valor producido se utiliza más tarde cuando el administrador de portafolios revisa los proyectos en el optimizador de portafolios para compararlos.

Para obtener más información sobre la optimización del portafolio, consulte el artículo [Información general sobre Portfolio Optimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

### Aplicar un informe de valoración a un proyecto

Como usuario con una licencia de plan y permisos de gestión a un proyecto, puede adjuntar un informe de valoración al proyecto.

Para obtener más información sobre los permisos del proyecto, consulte [Uso compartido de un proyecto en Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

Puede agregar informes de valoración a un proyecto como parte de la creación del caso empresarial del proyecto.

Para obtener más información sobre cómo crear un caso empresarial, consulte [Creación de un caso empresarial para un proyecto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

El administrador de Adobe Workfront o el administrador de grupos deben habilitar la sección Informe de valoración en el área Caso empresarial de sus proyectos para poder acceder a los informes de valoración desde el caso empresarial. Para obtener información sobre la configuración de preferencias de proyecto y las áreas de activación del caso práctico, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Para aplicar un informe de valoración a un proyecto:

1. Vaya a un proyecto al que desee aplicar un informe de valoración.
1. Haga clic en **Caso empresarial** en el panel izquierdo.
1. Busque la **Informe de valoración** del caso empresarial.\
   Debe crear un informe de valoración antes de **Informe de valoración** se muestra en el caso empresarial.

   Para obtener información sobre la creación de un informe de valoración, consulte [Crear un informe de valoración](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

1. Seleccione un informe de valoración en el menú desplegable.

   ![new_scorecard.png](assets/new-scorecard-350x149.png)

1. Especifique una respuesta para todas las preguntas del informe de valoración.

   Workfront aplica una puntuación a cada pregunta respondida y calcula una puntuación general del proyecto en función de la puntuación individual de cada pregunta.

   Para obtener más información sobre la generación de la puntuación de alineación general del proyecto, consulte [Generación de una puntuación de alineación para un proyecto](#generate-an-alignment-score-for-a-project).

1. Haga clic en **Guardar** para guardar el informe de valoración y puntuar el proyecto.

   El informe de valoración ahora está asociado al proyecto y se clasifica el proyecto.

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

## Generar una puntuación de alineación

* [Generación de una puntuación de alineación para un proyecto](#generate-an-alignment-score-for-a-project)
* [Generación de una puntuación de alineación para un portafolio](#generate-an-alignment-score-for-a-portfolio)

### Generación de una puntuación de alineación para un proyecto {#generate-an-alignment-score-for-a-project}

La puntuación de alineación es el valor producido después de completar el informe de valoración.

Los informes de valoración contienen preguntas con opciones de respuesta a las que se han asignado valores numéricos, denominados puntos de alineación. Estos puntos se utilizan para determinar la alineación del proyecto con su organización. Los puntos de alineación de cada pregunta contienen un número entre 0 y 100.

Cuando se completa el informe de valoración, Workfront calcula la puntuación de alineación del proyecto como porcentaje mediante la fórmula siguiente:

```
Project Alignment Score = The sum of the question points from the scorecard met at a given time/ The sum of the possible points on the scorecard
```

Para obtener más información, consulte [Crear un informe de valoración](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

### Generación de una puntuación de alineación para un portafolio {#generate-an-alignment-score-for-a-portfolio}

La puntuación de alineación del portafolio es una media de las puntuaciones de alineación de todos los proyectos del portafolio.

Cuando se completan los informes de valoración de los proyectos, Workfront utiliza esos valores para calcular la puntuación de alineación del portafolio como porcentaje, utilizando la fórmula siguiente:

Puntuación de alineación del Portfolio = La suma de los porcentajes de las puntuaciones de alineación del proyecto/Número de proyectos del portafolio

>[!NOTE]
>
>Si un proyecto no tiene asociado un informe de valoración y, por lo tanto, no tiene una puntuación de alineación, se considera que tiene una alineación del 0 % en el portafolio. El proyecto se tiene en cuenta en el número de proyectos de la cartera.

## Ver la puntuación de alineación

Puede ver la puntuación de alineación de un proyecto en el nivel de proyecto o en el Optimizador de Portfolio.

* [Visualización de la puntuación de alineación en un proyecto](#View%20the)
* [Ver las puntuaciones de alineación del proyecto y del portafolio en el Optimizador de Portfolio](#View%20the2)

### Visualización de la puntuación de alineación en un proyecto

Puede ver la puntuación de alineación de un proyecto a nivel de proyecto si tiene derechos de Contribute sobre el proyecto.

1. Vaya al proyecto cuya puntuación de alineación desee ver.
1. Haga clic en **Caso empresarial** en el panel izquierdo.
1. Vaya a la **Resumen de caso empresarial** a la derecha de la pantalla.

   La puntuación de alineación se encuentra en el resumen de caso empresarial, en la sección **Alineado** valor.

   ![alignment_score_on_a_project.png](assets/alignment-score-on-a-project.png)

### Ver las puntuaciones de alineación del proyecto y del portafolio en el Optimizador de Portfolio

Puede ver la puntuación de alineación de un proyecto o de un portafolio en el Optimizador de Portfolio, si tiene acceso Administrar al portafolio.

Para obtener más información sobre la información mostrada en el Optimizador de Portfolio, consulte [Información general sobre Portfolio Optimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* [Localice la puntuación de alineación del proyecto en el Optimizador de Portfolio](#locate-the-alignment-score-of-the-project-in-the-portfolio-optimizer)
* [Localice la puntuación de alineación del portafolio en el Optimizador de Portfolio](#locate-the-alignment-score-of-the-portfolio-in-the-portfolio-optimizer)

   ![](assets/alignment-score-in-portfolio-optimizer-nwe-350x97.png)

#### Localice la puntuación de alineación del proyecto en el Optimizador de Portfolio {#locate-the-alignment-score-of-the-project-in-the-portfolio-optimizer}

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png), luego **Portfolio**.

1. Haga clic en el nombre de un Portfolio.
1. Haga clic en **Optimización del Portfolio** en el panel izquierdo.

   Aparece el Optimizador de Portfolio.

1. La puntuación de alineación de un proyecto se muestra como un porcentaje en la variable **Alineación** del Portfolio Optimizer.

   Esta es la puntuación de alineación del proyecto basada en el informe de valoración asociado al proyecto.

#### Localice la puntuación de alineación del portafolio en el Optimizador de Portfolio  {#locate-the-alignment-score-of-the-portfolio-in-the-portfolio-optimizer}

1. Vaya a la **Proyectos** en la barra de navegación global.
1. Seleccione el **Portfolio** pestaña .
1. Haga clic en el nombre de un Portfolio.
1. Seleccione el **Optimización del Portfolio** pestaña .
1. En la parte superior del Portfolio Optimizer encontrará la variable **Alineado** , así como la variable **Alineación** Indicador que indica la puntuación de alineación del portafolio.

   Esta es la puntuación de alineación del portafolio.

   Para obtener más información sobre cómo se genera la puntuación de alineación de un portafolio, consulte [Generación de una puntuación de alineación para un portafolio](#generate-an-alignment-score-for-a-portfolio).

## Descripción general de la puntuación del optimizador de Portfolio

Existe una diferencia entre la puntuación de alineación y la puntuación del optimizador de portafolios de un proyecto.

La puntuación de alineación de un proyecto se calcula en función de los puntos obtenidos tras completar el informe de valoración. A continuación, esta puntuación se utiliza para determinar la puntuación de alineación del portafolio. La puntuación de alineación se muestra como un porcentaje.

La puntuación de alineación de un proyecto se muestra en la variable **Alineación** del Portfolio Optimizer.

La puntuación del optimizador de portafolios es una clasificación calculada automáticamente en el Optimizador de Portfolio mediante la cual se puede priorizar los proyectos. La puntuación del optimizador de portafolio se muestra como un icono de indicador acompañado de un número y se muestra en la variable **Puntuación** del Portfolio Optimizer. La puntuación del Optimizador de Portfolio solo se genera cuando se completan todas las secciones del Caso de negocio, excepto para los Objetivos.

Para obtener más información sobre la creación de un caso práctico para un proyecto, consulte [Creación de un caso empresarial para un proyecto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Para obtener más información sobre el cálculo de la puntuación del optimizador de portafolio de un proyecto, consulte [Descripción general de la puntuación del optimizador de Portfolio](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md).
