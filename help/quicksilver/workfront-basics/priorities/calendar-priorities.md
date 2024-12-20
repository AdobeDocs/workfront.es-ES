---
navigation-topic: get-started-with-workfront
title: Administrar el trabajo en el calendario de prioridades
description: Realice un seguimiento de su trabajo con un calendario claro y visual.
author: Courtney
feature: Get Started with Workfront
recommendations: noDisplay, noCatalog
source-git-commit: a351028e7c76c92bd93a0d7f8460e644e940a256
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 17%

---


# Administrar el trabajo en el calendario de prioridades

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa de espacio aislado.</span>

Realice fácilmente un seguimiento de su trabajo con un calendario claro y visual. Con el calendario de Prioridades, puede

* Utilice los filtros para encontrar su trabajo
* Aplique campos personalizados como estado y nivel de enfoque para identificar el trabajo de alta prioridad
* Aplicar colores para una organización rápida

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Plan de Adobe Workfront</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe Workfront*</strong></td> 
   <td> 
   <p>Actual: Revisor o superior</p>
   <p>Nuevo: Light o superior</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso</strong></td> 
   <td> <p>Acceso de visualización o edición para el objeto en el que se encuentra la actualización</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Acceso de visualización al objeto</p></td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ver su trabajo en el calendario

{{step1-to-priorities}}

1. Haga clic en el icono de Calendario en la parte superior de la lista de trabajos.
   ![icono de calendario](assets/calendar-tab.png)
1. Seleccione uno o varios filtros para reducir los elementos de trabajo.

   +++Amplíe para ver información detallada sobre los filtros disponibles
   <table>
    <tbody>
    <tr>
    <th>Filtro</th>
    <th>Descripción</th>
    </tr>
        <tr>
        <td>Trabajando en ello</td>
        <td>Muestra los elementos en los que está trabajando actualmente</td>
        </tr>
        <tr>
        <td>Listo para comenzar</td>
        <td>Muestra elementos con 
        <ul>
        <li>Sin predecesoras incompletas ni restricciones de tarea</li>
        <p>y</p>
        <li>La fecha planificada de inicio es anterior o inferior a dos semanas</li>
        </ul>
        </td>
        </tr>
        <tr>
        <td>Sin preparar</td>
        <td>Muestra elementos que tienen
        <ul>
        <li>Predecesoras incompletas o delimitaciones de tareas que impiden trabajar en el elemento</li>
        <p>o</p>
        <li>La fecha planificada de inicio es dentro de más de dos semanas</li>
        </ul>
        </td>
        </tr>
        <tr>
        <td>Solicitud</td>
        <td>Muestra los problemas en los que no ha empezado a trabajar</td>
        </tr>
        <td>Listo</td>
        <td>Muestra el trabajo completado en las últimas dos semanas. Esta opción de filtro no incluye aprobaciones.</td>
        </tr>
        <tr>
        <td>Proyecto</td>
        <td>Muestra los proyectos que contienen tareas o problemas a los que se le ha asignado</td>
        </tr>
        <tr>
        <td>Fecha de vencimiento</td>
        <td>Muestra el trabajo por fecha planificada de finalización</td>
        </tr>
        <tr>
        <td>Estado</td>
        <td>Muestra tareas o problemas en estados nuevos, en curso y completos</td>
        </tr>
        <tr>
        <td>Mi enfoque</td>
        <td>Muestra tareas o problemas en que tienen niveles de enfoque asignados. El usuario individual asigna y administra los niveles de enfoque.</td>
        </tr>
    </tbody>
    </table>

+++

1. Haga clic en la barra del elemento de trabajo del calendario para abrir el resumen lateral. El resumen lateral le permite

* Ver y editar detalles de proyecto y elemento de trabajo
* Crear y ver comentarios
* Ver y cargar documentos
* Crear una prueba
* Vaya a la página del proyecto en Workfront
* Vaya a la página de detalles del elemento de trabajo en Prioridades
* Hora de registro
* Adición de vínculos rápidos

1. (Opcional) Haga clic en **Crear nuevo** para agregar un nuevo elemento de trabajo al calendario. Para obtener más información, consulte [Crear una tarea o problema nuevo en Prioridades](/help/quicksilver/workfront-basics/priorities/create-task-issue-priorities.md).

## Configuración del calendario

{{step1-to-priorities}}

1. Haga clic en el icono de Calendario en la parte superior de la lista de trabajos.
   ![icono de calendario](assets/calendar-tab.png)
1. Haga clic en el icono **Configuración** en la esquina derecha del calendario.

1. En la ficha **Estilo de barra**, elija hasta 5 campos para mostrar en la barra de elementos de trabajo del calendario.
   ![barra de muestra](assets/sample-task-for-field-config.png)

1. En la ficha **Color**, elija cómo desea que se muestren los elementos de trabajo. Por ejemplo, si elige Proyecto, los elementos de trabajo se muestran según el color asignado al proyecto en la lista de trabajo.
   ![proyecto de color de muestra](assets/sample-calendar-projects.png)

