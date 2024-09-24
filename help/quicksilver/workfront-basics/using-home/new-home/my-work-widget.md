---
product-area: home
navigation-topic: use-the-home-area
title: Administre su trabajo con el widget Mi trabajo
description: El widget Mi trabajo muestra todas las tareas, problemas y solicitudes asignados en un solo lugar. Aquí puede filtrar y organizar su trabajo, registrar el tiempo, realizar actualizaciones y marcar los elementos de trabajo como completados.
author: Courtney
feature: Get Started with Workfront
source-git-commit: 20791e9f2cc0716b9b0ddd8f98c31ae0bea7ff45
workflow-type: tm+mt
source-wordcount: '704'
ht-degree: 5%

---


# Administre su trabajo con el widget Mi trabajo

El widget Mi trabajo muestra todas las tareas, problemas y solicitudes asignados en un solo lugar. Aquí puede filtrar y organizar su trabajo, registrar el tiempo, realizar actualizaciones y marcar los elementos de trabajo como completados.

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
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licencia</strong></td> 
   <td> <p>Actual: Contribute</p>
   <p>O</p> 
   <p>Nuevo:[!UICONTROL Light] o superior<p> 
  </td> 
  </tr> </ul>
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso</strong></td> 
   <td> <p>[!UICONTROL View] o acceso superior a Proyectos, Tareas, Problemas y Documentos</p> </td> 
  </tr>  
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Permisos de Contribute o superiores para las tareas y problemas en los que debe trabajar</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Búsqueda del trabajo con filtros

Puede ajustar los filtros de Mi trabajo para que se centren en elementos específicos de la lista de trabajo:

![](assets/filter-my-work-widget.png)

### Detalles del filtro

<table>
  <tbody>
    <tr>
      <td>Trabajando en</td>
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
    <tr>
      <td>Delegado por mí</td>
      <td>Muestra elementos que ha delegado en otros usuarios</td>
    </tr>
    <tr>
      <td>Se me ha delegado</td>
      <td>Muestra los elementos que los usuarios le han delegado</td>
    </tr>
    <tr>
      <td>Finalizado</td>
      <td>Muestra el trabajo completado en las últimas dos semanas. Esta opción de filtro no incluye aprobaciones.</td>
    </tr>
  </tbody>
</table>

>[!TIP]
>
>Si busca opciones de filtrado más específicas, puede utilizar los widgets Mi tarea o Mi problema. Para obtener más información sobre los filtros Mi tarea y Mi problema, consulte [Información general sobre los filtros de los widgets de inicio nuevos](/help/quicksilver/workfront-basics/using-home/new-home/widget-filter-overview-new-home.md).

## Organizar su trabajo

Puede utilizar las funciones de ordenación y grupo del widget Mi trabajo para organizar el trabajo de forma que tenga sentido.

### Ordenar

Puede ordenar la lista de trabajos por

* Fecha de vencimiento
Los elementos vencidos muestran un icono de advertencia junto a la fecha. Workfront utiliza la fecha planificada de finalización para determinar si las tareas y los problemas están vencidos.
* Nombre
* Porcentaje completado
* Estado

>[!TIP]
>
>Para crear una lista que muestre todos los elementos vencidos en la parte superior del widget Mi trabajo, ordene por Fecha de vencimiento y no aplique una agrupación.


![](assets/sort-my-work-widget.png)

### Grupo

Puede agrupar la lista de trabajos por

* Proyecto
* Estado
* Fecha de vencimiento
La fecha de vencimiento viene determinada por la fecha planificada de finalización.

>[!NOTE]
>
>Cuando se aplica una agrupación, la selección en el menú Ordenar determina el orden dentro de la agrupación.


![](assets/group-my-work-widget.png)

## Actualizar la información del elemento de trabajo en el resumen

Puede abrir el Panel de resumen para actualizar rápidamente la información de una tarea o un problema. En el Resumen, puede hacer lo siguiente

* Actualizar el porcentaje completado
* Añadir una actualización
* Vaya al área de Documento para cargar un documento
* Ver detalles del elemento de trabajo y actualizar campos personalizados
Los administradores de Workfront pueden personalizar qué campos aparecen en el resumen de la plantilla de diseño. Para obtener más información, consulte [Personalizar inicio y resumen con una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).
* Cambiar el estado del elemento de trabajo
* Ver subtareas
* Hora de registro
* Ver procesos de aprobación adjuntos

Para abrir el resumen, pase el ratón sobre el elemento de trabajo y haga clic en el icono **Resumen** ![](assets/open-summary-new-home.png).

Para obtener información adicional sobre cómo usar el Panel de resumen, consulte [Resumen general](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md).

## Usar acciones rápidas para actualizar elementos de trabajo

Puede utilizar el menú de acciones rápidas para lo siguiente

* Hora de registro
* Añadir una actualización
* Actualizar un formulario personalizado
* Cargar un archivo

Para localizar el menú de acciones rápidas, pase el ratón sobre el elemento de trabajo. La lista de acciones rápidas se muestra cerca del botón **Trabajar en ello** o **Listo**.

![](assets/quick-actions-new-home.png)


## Ver aprobaciones y solicitudes de equipo

Las aprobaciones y las solicitudes de equipo no se muestran en el widget Mi trabajo. Si trabaja regularmente con aprobaciones y solicitudes de equipo, le recomendamos que añada los siguientes widgets a su nueva página de inicio:

* En espera de mi aprobación
* Todas las aprobaciones
* Solicitudes de equipo

Para obtener información acerca de cómo agregar widgets a su nueva página de inicio, vea [Agregar, editar o quitar widgets en la nueva página de inicio](/help/quicksilver/workfront-basics/using-home/new-home/add-edit-remove-widgets-in-new-home.md).




