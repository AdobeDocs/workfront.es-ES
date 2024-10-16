---
navigation-topic: get-started-with-workfront
title: Filtrar y agrupar su trabajo con Prioridades
description: Puede utilizar filtros para encontrar el trabajo que busca y, a continuación, aplicar una agrupación para mantenerla organizada.
author: Courtney
feature: Get Started with Workfront
recommendations: noDisplay, noCatalog
source-git-commit: 75396c3f066abc6070ae2a89c2ded0255dbc0751
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 6%

---


# Filtrar y agrupar su trabajo con Prioridades

Puede utilizar filtros para encontrar el trabajo que está buscando y, a continuación, aplicar una agrupación para mantenerlo organizado.

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
   <td role="rowheader"><strong>plan de Adobe Workfront</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe Workfront*</strong></td> 
   <td> 
   <p>Actual: Solicitud o superior</p>
   <p>Nuevo: Colaborador o superior</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso</strong></td> 
   <td> <p>Acceso de visualización o edición para el objeto en el que se encuentra la actualización</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Ver acceso al objeto</p></td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtrar su trabajo

Puede filtrar las tareas y los problemas que se le hayan asignado.

{{step1-to-priorities}}

1. Haga clic en **Filtros** en la parte superior derecha de la lista de trabajos.
1. Seleccione uno o varios filtros para reducir los elementos de trabajo.
   ![](assets/filters.png)

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

1. (Opcional) Haga clic en **Volver al valor predeterminado** para restablecer su selección.

## Agrupar su trabajo

{{step1-to-priorities}}

1. Haga clic en **Grupos** en la parte superior derecha de la lista de trabajos.
1. Seleccione un grupo para organizar la lista de trabajos
   ![](assets/groups.png)

+++Amplíe para ver información detallada sobre los grupos disponibles

| Grupo | Descripción |
|-----------|-------------|
| Ninguno | Esto elimina las agrupaciones de la lista de trabajo. |
| Mi enfoque | Agrupa los elementos según el nivel de enfoque que asigne. |
| Vence la semana | Agrupa los elementos según la semana de vencimiento. Las fechas de vencimiento están determinadas por la fecha planificada de finalización. |
| Estado | Agrupa los elementos según los siguientes estados: Nuevo, En curso y Completado. <br>Nota: no puede usar estados personalizados en Prioridades en este momento. |
| Proyecto | Agrupa los elementos por proyecto. |

+++

## Ordenar el trabajo

Para ordenar tu trabajo, abre **Grupo** y haz clic en **Orden ascendente** o **Orden descendente**.

![](assets/expand-sort-groups.png)

>[!IMPORTANT]
>
>La opción de ordenación no está disponible temporalmente si se ha aplicado un grupo.



## Expandir o contraer todas las secciones

Para expandir o contraer todas las secciones, abra **Grupo** y haga clic en **Expandir todo** o **Contraer todo**.

![](assets/expand-sort-groups.png)

