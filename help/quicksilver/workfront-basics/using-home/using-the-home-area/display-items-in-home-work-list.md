---
product-area: projects
navigation-topic: use-the-home-area
title: Mostrar elementos en la [!UICONTROL Lista de trabajos] del área de inicio
description: Cada widget contiene su propia lista de trabajos. Las listas de trabajo muestran todos los elementos de trabajo que tiene asignados. Puede controlar qué elementos se muestran en su [!UICONTROL lista de trabajo] mediante filtros y agrupaciones.
author: Courtney
feature: Get Started with Workfront, Work Management
exl-id: eac2e065-9e32-43c1-90ff-0f841b508c35
TQID: https://experienceleague.adobe.com/fITdY6-HlQ-4527-RiI9m52-Kg3nRUxsk32vjpw-A-g
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 990
ht-degree: 7%

---

# Mostrar elementos en la [!UICONTROL lista de trabajo] del área [!UICONTROL Hogar]

<!-- Audited: 1/2024 -->

Cada widget contiene su propia lista de trabajos. Las listas de trabajo muestran todos los elementos de trabajo que tiene asignados. Puede controlar qué elementos se muestran en su [!UICONTROL lista de trabajo] mediante filtros y agrupaciones.

>[!IMPORTANT]
>
>* Para mostrar tareas y problemas en los widgets de Inicio, su proyecto principal debe estar en estado Actual o un estado igual al actual.
>* Los proyectos también deben estar en Estado actual o un estado que equivalga al actual para mostrarlos en Inicio.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licencia</strong></td> 
   <td><ul><li>[!UICONTROL Contributor] solo para aprobaciones</li> <li>[!UICONTROL Standard] o superior para todos los demás objetos</li> <p>O</p> 
  </ul><ul><li>[!UICONTROL Review] solo para aprobaciones</li> <li>[!UICONTROL Work] o superior para todos los demás objetos</li> </td> 
  </tr> </ul>
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso</strong></td> 
   <td> <p>[!UICONTROL View] o acceso superior a Proyectos, Tareas, Problemas y Documentos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Aportar permisos o superiores a las tareas y problemas en los que tiene que trabajar</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos para que los elementos de trabajo se muestren en la lista de trabajo

Hay requisitos integrados para los que los elementos de trabajo se muestran en una determinada lista de trabajos de widgets. Los elementos de trabajo deben cumplir estos requisitos para aparecer en las listas de trabajo del widget siguiente.

### Widget de Mis tareas

Las tareas deben cumplir los siguientes requisitos para aparecer en el widget Mis tareas:

* El estado de la tarea no es igual a Completo.
* El usuario que ha iniciado sesión debe estar asignado a la tarea.
* El estado de la tarea no es igual a Listo.
* El proyecto al que pertenece la tarea debe estar en un estado equivalente a Actual.


### Widget de Mis problemas

Los problemas deben cumplir los siguientes requisitos para aparecer en el widget Mis problemas:

* El usuario que ha iniciado sesión debe estar asignado al problema.
* El estado del problema no equivale a Completo.
* No hay ningún objeto sin resolver adjunto al problema.
* El estado del problema no es igual a Listo.
* El proyecto al que pertenece el problema debe estar en un estado equivalente a Actual.

### Widget de Mis equipos

Las solicitudes de equipo deben cumplir los siguientes requisitos para aparecer en el widget Mis equipos:

* El usuario que ha iniciado sesión pertenece al equipo al que está asignado el elemento de trabajo.
* El estado del elemento de trabajo no es igual a Completo.
* El elemento de trabajo no tiene adjunto un proceso de aprobación sin resolver.
* El elemento de trabajo no es una tarea recurrente.
* El proyecto al que pertenece el elemento de trabajo debe estar en un estado equivalente a Actual.

## Filtrar su trabajo

Puede filtrar elementos en la [!UICONTROL Lista de trabajos] de un widget para ver solamente tipos de elementos específicos. Por ejemplo, puede filtrar Mi trabajo [!UICONTROL Lista de trabajos] para mostrar solo los problemas o las solicitudes.

>[!NOTE]
>
>Las opciones de filtro se almacenan en el explorador. Si utiliza el mismo explorador de forma constante en el mismo equipo (y no borra los datos del sitio), los filtros seleccionados no cambian. Si cambia de un navegador a otro o de un ordenador, los filtros vuelven a la opción predeterminada, que es la que no está seleccionada para todos los filtros.

Para filtrar su trabajo:

1. Haga clic en el **[!UICONTROL Menú principal]** ![icono del menú principal](assets/main-menu-icon.png) en la esquina superior derecha y, a continuación, haga clic en **[!UICONTROL Inicio]**.
1. (Condicional) Haga clic en **Personalizar** para agregar cualquiera de los siguientes widgets:

   | Widget | Descripción |
   |--------------|---------------------------------------------------------------------------------------------------|
   | Tableros | Muestra los tableros que ha creado o que se le ha invitado a utilizar |
   | Mi trabajo | Muestra las tareas y problemas asignados a usted |
   | Mis proyectos | Muestra los proyectos que posee o en los que participa |
   | Mis tareas | Muestra las tareas asignadas a usted |
   | Mis problemas | Muestra los problemas asignados a usted |
   | Mis solicitudes | Muestra todas las solicitudes que ha enviado |
   | Mis aprobaciones | Muestra todas las aprobaciones pendientes, asignadas, delegadas y enviadas |

1. Haga clic en el icono **Filtro** ![Icono de filtro](assets/filter-nwepng.png) en la esquina superior derecha de la lista de trabajo del widget.
1. Elija un filtro **Sugerido** o un filtro que haya creado.
Para obtener información detallada sobre los filtros sugeridos, consulte [Resumen de los filtros del widget de inicio](/help/quicksilver/workfront-basics/using-home/using-the-home-area/widget-filter-overview-home.md).
1. (Opcional) Active **Apilar filtros** para seleccionar varias opciones de filtro.

   ![Mi filtro de tareas abierto](assets/my-task-filter-open.png)


## Agrupar su trabajo

Puede agrupar el widget [!UICONTROL lista de trabajo] para mantener los elementos de trabajo organizados.

Para agrupar la lista de trabajos:

1. Haga clic en el **[!UICONTROL Menú principal]** ![icono del menú principal](assets/main-menu-icon.png) en la esquina superior derecha y, a continuación, haga clic en **[!UICONTROL Inicio]**.
1. (Condicional) Haga clic en **Personalizar** para agregar cualquiera de los siguientes widgets:

   | Widget | Descripción |
   |--------------|---------------------------------------------------------------------------------------------------|
   | Tableros | Muestra los tableros que ha creado o que se le ha invitado a utilizar |
   | Mi trabajo | Muestra las tareas y problemas asignados a usted |
   | Mis proyectos | Muestra los proyectos que posee o en los que participa |
   | Mis tareas | Muestra las tareas asignadas a usted |
   | Mis problemas | Muestra los problemas asignados a usted |
   | Mis solicitudes | Muestra todas las solicitudes que ha enviado |
   | Mis aprobaciones | Muestra todas las aprobaciones pendientes, asignadas, delegadas y enviadas |

1. Haga clic en el icono **Grupo** ![Icono de grupo](assets/group-icon.png) en la esquina superior derecha de la lista de trabajo del widget.
1. Elija una agrupación **sugerida** o una agrupación que haya creado.
   ![Agrupación expandida](assets/grouping-expanded.png)


## Personalizar columnas de lista de trabajo

Puede elegir qué columnas aparecen en la lista de trabajo de widgets:

1. Haga clic en el **[!UICONTROL Menú principal]** ![icono del menú principal](assets/main-menu-icon.png) en la esquina superior derecha y, a continuación, haga clic en **[!UICONTROL Inicio]**.
1. (Condicional) Haga clic en **Personalizar** para agregar cualquiera de los siguientes widgets:

   | Widget | Descripción |
   |--------------|---------------------------------------------------------------------------------------------------|
   | Tableros | Muestra los tableros que ha creado o que se le ha invitado a utilizar |
   | Mi trabajo | Muestra las tareas y problemas asignados a usted |
   | Mis proyectos | Muestra los proyectos que posee o en los que participa |
   | Mis tareas | Muestra las tareas asignadas a usted |
   | Mis problemas | Muestra los problemas asignados a usted |
   | Mis solicitudes | Muestra todas las solicitudes que ha enviado |
   | Mis aprobaciones | Muestra todas las aprobaciones pendientes, asignadas, delegadas y enviadas |

1. Haga clic en el icono **Columna** ![Icono de columna](assets/column-icon.png) en la esquina superior derecha de la lista de trabajo del widget.
1. Active o desactive las columnas según sus preferencias.
1. (Opcional) Haga clic en el icono **Arrastrar** ![Arrastrar icono](assets/drag-icon.png) para reordenar las columnas.
   ![Columnas expandidas](assets/columns-expanded.png)


## Ver elementos atrasados

[!DNL Adobe Workfront] usa las fechas siguientes para determinar si las solicitudes de trabajo están atrasadas:

* **Tareas**: [!UICONTROL Fecha planificada de finalización]
* **Problemas**: [!UICONTROL Fecha planificada de finalización]
* **Documentos**: [!UICONTROL Fecha de envío]
* **Plantillas de horas**: [!UICONTROL Fecha de envío]
* **Aprobaciones**: [!UICONTROL Fecha de envío]
* **Aprobaciones de revisión**: [!UICONTROL Plazo de revisión]


