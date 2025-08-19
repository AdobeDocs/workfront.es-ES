---
title: Resumen de estado del proyecto
content-type: reference
description: La función Project Health utiliza el poder del Asistente de IA para ofrecerle instantáneamente una evaluación del rendimiento de sus proyectos.
author: Jenny
feature: Get Started with Workfront
exl-id: e4d200c6-7f35-4919-96d3-2880a655ed62
source-git-commit: 2024f19709f7859ed6f19b830321d9e4c09e71f8
workflow-type: tm+mt
source-wordcount: '1822'
ht-degree: 2%

---

# Resumen de estado del proyecto

>[!IMPORTANT]
>
>Actualmente, la función Estado del proyecto solo está disponible para los usuarios que participan en la fase beta.

La función Project Health de Adobe Workfront utiliza la potencia de AI Assistant para ofrecerle instantáneamente una evaluación del rendimiento de sus proyectos, qué áreas necesitan su atención y cómo evitar problemas que pueden costarle tiempo y dinero.

El Asistente de inteligencia artificial puede generar una evaluación del estado del proyecto para los siguientes objetos:

* Un solo proyecto
* Un solo programa
* Varios proyectos

Para obtener más información sobre el Asistente de IA, consulte [Descripción general del Asistente de IA](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).

+++ Amplíe para ver los requisitos de acceso. 
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Plan de Adobe Workfront</p></td> 
   <td> 
<p>Seleccionar, Prime o Ultimate </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td> 
<p>Estándar</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuraciones de nivel de acceso</p></td> 
   <td><p>Administrador para administrar las configuraciones de estado del proyecto </p>
   <p>Editar para aplicar configuraciones de estado del proyecto </p>
     <p>Ver para ver las configuraciones de estado del proyecto </p>
  </td> 
  </tr>  
    </tr>  
</tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Inscríbase en la versión beta de Project Health

Para utilizar Project Health, su organización debe tener habilitado el Asistente para IA.

Para habilitar el Asistente de IA para su organización, debe aplicar lo siguiente:

* Su organización debe haber migrado a Adobe IMS (sistema Identity Management).
* La experiencia unificada de Adobe debe estar habilitada.
* Adobe debe tener registrado un acuerdo de Adobe Gen AI.
* El administrador de Workfront debe habilitar el Asistente de IA para los usuarios de su organización. El asistente de IA se habilita mediante niveles de acceso.

Para obtener más información, consulte [Descripción general del Asistente de IA](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).

## Lista de peticiones del Asistente de IA

A continuación se muestra una lista de preguntas que puede utilizar para solicitar a la evaluación de IA que genere una evaluación de estado del proyecto para un proyecto, programa o todos los proyectos de su cuenta.

<table>
    <tr>
        <td><b>Ubicación</b></td>
        <td><b>Solicitud</b></td>
    </tr>
    <tr>
        <td>Página de detalles de un proyecto específico</td>
        <td><em>¿Cuál es la salud de este proyecto?</em></td>
    </tr>
    <tr>
        <td>Cualquier página de Workfront </td>
        <td><em>¿Cuál es el estado del proyecto [NOMBRE DEL PROYECTO]?</em></td>
    </tr>
    <tr>
        <td>Cualquier página de Workfront </td>
        <td><em>¿Cuál es la salud de mis proyectos?</em></td>
    </tr>
       <tr>
        <td>Página de detalles de un programa específico</td>
        <td><em>¿Cuál es la salud de este programa?</em></td>
    </tr>
       <tr>
        <td>Cualquier página de Workfront </td>
        <td><em>¿Cuál es el estado del programa [NOMBRE DEL PROGRAMA]?</em></td>
    </tr>
   </table>


## Lista de condiciones de proyecto y programa

A continuación se muestran las condiciones disponibles que el Asistente de inteligencia artificial asignará a su proyecto o programa al generar una evaluación de estado del proyecto.

<table>
    <tr>
        <td><b>Condición del proyecto</b></td>
        <td><b>Estado de progreso del proyecto</b></td>
    </tr>
    <tr>
        <td>Bien encaminado</td>
        <td>Cuando el estado del progreso del proyecto es A tiempo, la condición del proyecto es A tiempo.</td>
    </tr>
    <tr>
        <td>En riesgo</td>
        <td>Cuando el estado del progreso del proyecto es Retrasado o En riesgo, la condición del proyecto es En riesgo.</td>
    </tr>
    <tr>
        <td>Con problemas</td>
        <td>Cuando el estado del progreso del proyecto es Retrasado, la condición del proyecto es En riesgo.</td>
    </tr>
    </tr>
   </table>

## Administrar configuraciones de estado del proyecto

Una configuración de mantenimiento del proyecto contiene criterios específicos que determinan cómo se calcula el estado del proyecto. Después de crear una configuración, puede aplicarla a un proyecto.

>[!NOTE]
>
>Debe ser administrador del sistema para administrar las configuraciones de estado del proyecto.

{{step-1-to-setup}}

1. Haga clic en **Preferencias del proyecto** en el panel izquierdo y, a continuación, seleccione **Estado del proyecto** en la lista desplegable que aparece.

1. En la esquina superior derecha de la página, seleccione **Nueva configuración**.

1. (Opcional) En la página de detalles de las configuraciones, reemplace *Configuración sin título* por una nueva configuración **Name**.

1. En la sección **Qué factores desea incluir en el estado del proyecto**, anule la selección de cualquier factor que no desee incluir al determinar los criterios de estado del proyecto:
   * **Cambio de ámbito**: Cuánto se ha ampliado el ámbito del proyecto desde que se inició.

   * **Campos obligatorios**: Si faltan campos obligatorios (por ejemplo, descripción del proyecto). Estos campos obligatorios determinan la finalización del proyecto y se especifican en el **¿Qué campos desea comprobar para ver si están completos?** sección de configuración a continuación.


   * **Cambios de horario**: Cuántos cambios de horario se han producido desde que se inició el proyecto.

   * **Estimación de tareas**: La precisión con que se ha calculado el trabajo de la tarea (por ejemplo, no hay tareas vencidas actualmente en el proyecto).

   * **Evolución de tareas**: Cómo progresa el trabajo del proyecto en comparación con la cronología del proyecto.

   * **Tareas vencidas**: Cuántas tareas están actualmente vencidas.

   * **Costo**: Si el proyecto está actualmente por encima del presupuesto.

1. En **¿Cuándo comienza oficialmente su proyecto?**, seleccione el evento que indica el comienzo del proyecto en la lista desplegable.

1. En **¿Cómo calcula el ámbito de trabajo de un proyecto?**, seleccione qué factor de proyecto aumentará a medida que aumente el ámbito del proyecto.

1. En el **¿Qué campos desea comprobar para ver si están completos?**, seleccione uno o más campos que se verificarán para determinar la integridad del proyecto.

   ![Campos de finalización del proyecto](assets/project-completeness-fields.png)


1. Haz clic en **Guardar** en la esquina superior derecha.

## Aplicar configuraciones de estado del proyecto

Una vez que un administrador ha creado una configuración de estado del proyecto, los usuarios con acceso de edición pueden aplicarla a un proyecto.


{{step1-to-projects}}

1. En la página **Proyectos**, seleccione un proyecto.

1. Haga clic en el icono **Más** ![Más icono](assets/more-icon.png) a la derecha del nombre del proyecto y, a continuación, seleccione **Editar**. Se abre el panel lateral **Editar proyecto**.

1. En el panel izquierdo, seleccione **Configuración del proyecto**.

1. En el campo **Configuración de mantenimiento del proyecto**, seleccione la configuración que desee aplicar a este proyecto.

   ![Campo de configuración de mantenimiento del proyecto](assets/project-health-configurations.png)

1. Haga clic en **Guardar** en la esquina inferior izquierda del panel.

## Generar una evaluación de estado del proyecto para un proyecto o programa

Si tiene acceso de visualización para un proyecto o programa, puede generar su evaluación del estado del proyecto con el asistente de IA.

Si está generando una evaluación para un proyecto, puede hacerlo desde la página del proyecto o haciendo referencia al nombre del proyecto cuando pregunte al asistente el rendimiento del proyecto.

Si está generando una evaluación para un programa, puede hacerlo desde la página de detalles del programa.

>[!NOTE]
>
>No se puede generar una evaluación de estado del proyecto para un proyecto hasta que se haya iniciado el proyecto. Puede configurar los déclencheur de evento de un proyecto para que comiencen en la configuración del proyecto.

Para obtener más información, vea la siguiente sección de este artículo: [Administrar configuraciones de estado del proyecto](#manage-project-health-configurations).

1. Desplácese hasta el proyecto o programa para el que desee generar una evaluación de estado del proyecto.

1. En la página de detalles del proyecto o programa, haga clic en el icono **Asistente de IA** ![Icono del Asistente de IA](assets/ai-assistant-icon.png) en la esquina superior derecha de la pantalla. Se abre el Ayudante de IA.

1. Escriba lo siguiente en el campo **Preguntarme acerca de Workfront**: *¿Cuál es el estado de este proyecto?*

   O

   Escriba lo siguiente en el campo **Preguntarme acerca de Workfront**: *¿Cuál es el estado de este programa?*

   >[!NOTE]
   >
   >Si accede al Asistente de IA desde una página diferente en Workfront, escriba *¿Cuál es el estado del proyecto [NOMBRE DEL PROYECTO]?* o *Cuál es el estado del programa [NOMBRE DEL PROGRAMA]?* <br>
   >Para obtener una lista completa de los mensajes actuales que puede especificar, consulte la siguiente sección en este artículo: [Lista de mensajes del Asistente de IA](#ai-assistant-prompts-list).

1. Pulse el icono **Enviar** ![Enviar icono](assets/send-icon.png). La evaluación del estado del proyecto genera y aparece en el panel. Aparece una insignia en la parte superior de cada evaluación de estado del proyecto, que refleja la condición actual del proyecto.

   ![Evaluación del estado del proyecto](assets/health-assessment.png)

   Si está generando una evaluación para un portafolio, se enumerarán varias insignias que mostrarán la condición de cada proyecto en el programa. Para obtener más información sobre las etiquetas de distintivo, consulte la siguiente sección en este artículo: [Lista de condiciones del proyecto y del programa](#project-and-program-conditions-list).

1. (Opcional) Haga clic en uno de los puntos de evaluación para ampliar sus detalles.

1. (Opcional) En el modo de detalles expandidos, haga clic en el vínculo de la tarea para abrir los detalles de la tarea.

   ![Detalles ampliados](assets/expanded-details.png)

1. Después de revisar los detalles del estado del proyecto, haz clic en el icono **Cerrar** ![Cerrar icono](assets/close-icon.png) en la esquina superior derecha del Ayudante de IA.

## Generar una evaluación de estado del proyecto para varios proyectos

Puede generar una evaluación combinada del estado del proyecto para todos los proyectos para los que actualmente tiene acceso de visualización (o superior).

Un proyecto solo se incluirá en la evaluación combinada del estado del proyecto si el proyecto ha comenzado. Puede configurar los déclencheur de evento de un proyecto para que comiencen en la configuración del proyecto. Para obtener más información, vea la siguiente sección de este artículo: [Administrar configuraciones de estado del proyecto](#manage-project-health-configurations).

1. Haga clic en el icono **Asistente de IA** ![Icono del Asistente de IA](assets/ai-assistant-icon.png) en la esquina superior derecha de la pantalla. Se abre el Ayudante de IA.

1. Escriba lo siguiente en el campo **Preguntarme acerca de Workfront**: *¿Cuál es el estado de mis proyectos?*

   Para obtener una lista completa de los mensajes actuales que puede especificar, consulte la siguiente sección en este artículo: [Lista de mensajes del Asistente de IA](#ai-assistant-prompts-list).

1. Pulse el icono **Enviar** ![Enviar icono](assets/send-icon.png). La evaluación del estado del proyecto genera y aparece en el panel.

   ![Evaluación de varios proyectos](assets/multiple-projects-assessment.png)

   Al generar una evaluación para varios proyectos, el Asistente de IA agrupa los resultados en función del rendimiento actual de los proyectos.

1. (Opcional) Haga clic en uno de los distintivos de estado del proyecto para expandir la lista de proyectos y, a continuación, seleccione un vínculo para que un proyecto específico vaya a la página de detalles de ese proyecto.

1. Después de revisar los detalles de estado de los proyectos, haga clic en el icono **Cerrar** ![Cerrar icono](assets/close-icon.png) en la esquina superior derecha del Ayudante de IA para cerrarlo.


## Crear un informe de tabla de estado de proyecto en un panel de lienzo

>[!IMPORTANT]
>
>Actualmente, la función Paneles de lienzo solo está disponible para los usuarios que participan en la fase beta. Para obtener más información, consulte [Información beta de paneles de lienzo](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md).

Puede agregar un informe de tabla a un panel de lienzo para visualizar fácilmente los datos del estado del proyecto en formato de tabla.

### Requisitos previos

Debe crear un tablero para poder crear un informe de tabla.

Para obtener más información, consulte [Crear un panel de lienzo](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

### Generar un informe de tabla Estado del proyecto

Hay muchas opciones de configuración disponibles para crear un informe de tabla Estado del proyecto. En esta sección, le guiaremos por el proceso de creación de uno que muestre las siguientes columnas:

* **Nombre**: contiene el nombre del proyecto.
* **Análisis del estado del proyecto**: contiene un resumen de la evaluación del estado del proyecto.
* **Se creó el estado del proyecto a las**: contiene la fecha y la hora en que se generó por última vez la evaluación del estado del proyecto.
* **Etiqueta de mantenimiento del proyecto**: contiene la etiqueta del proyecto (p. ej. En el objetivo, en riesgo o con problemas).

{{step1-to-dashboards}}

1. En el panel izquierdo, haga clic en **Paneles de lienzo**.
1. En la esquina superior derecha, haga clic en **Nuevo panel**.
1. En el cuadro **Crear tablero**, escriba el **Nombre** y la **Descripción** del tablero.
1. Haga clic en **Crear**.
1. En el cuadro **Agregar informe**, seleccione **Crear informe**.
1. En el lado izquierdo, seleccione **Tabla**.
1. En la esquina superior derecha, haga clic en **Crear informe**.
1. (Opcional) Siga los pasos a continuación para configurar la sección **Detalles** ![Icono de detalles](assets/details-icon.png):
   1. Escriba un informe **Nombre**.
   1. Escriba un informe **Descripción**.
1. Siga los pasos a continuación para configurar la sección **Generar tabla** ![icono de generación de tabla](assets/drilldown-column.png):
   1. En el panel izquierdo, haga clic en el icono **Columnas de tabla**.
   1. Haga clic en **Agregar columna** y luego seleccione **Proyecto** > **Nombre**.
   1. Haga clic en **Agregar columna** y, a continuación, seleccione **Proyecto** > **Estado del proyecto** > **Análisis de estado**.
   1. Haga clic en **Agregar columna** y, a continuación, seleccione **Proyecto** > **Estado del proyecto** > **Creado a las**.
   1. Haga clic en **Agregar columna** y, a continuación, seleccione **Proyecto** > **Estado del proyecto** > **Etiqueta de estado**.

1. Siga los pasos a continuación para configurar la sección **Filtro** ![Icono de filtro](assets/filter-icon.png):
   1. En el panel izquierdo, haga clic en el icono **Filtro**.
   1. Seleccione **Editar filtro**.
   1. Haga clic en **Agregar condición** y, a continuación, especifique el campo por el que desea filtrar y el modificador que define qué tipo de condición debe cumplir el campo. La columna aparece en la sección de vista previa de la derecha.
   1. (Opcional) Haga clic en **Agregar grupo de filtros** para agregar otro conjunto de criterios de filtrado. El operador predeterminado entre los conjuntos es Y. Haga clic en el operador para cambiarlo a OR.

1. Siga los pasos a continuación para configurar la sección **Configuración del grupo de desglose** ![Configuración del grupo](assets/drilldown-group-icon.png):
   1. En el panel izquierdo, haga clic en el icono **Configuración de grupo**.
   1. Haga clic en el botón **Agregar agrupación** y, a continuación, seleccione el campo que desee crear como agrupación. La columna de agrupación aparece en la sección de vista previa de la derecha.

1. Haga clic en **Guardar** para crear el informe.
