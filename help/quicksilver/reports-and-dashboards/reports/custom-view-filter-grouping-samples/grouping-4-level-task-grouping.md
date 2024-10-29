---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Agrupación: agrupación de tareas de 4 niveles para el propietario del Portfolio, el propietario del programa, el propietario del proyecto y el estado del proyecto"
description: Esta tarea Grouping ofrece 4 niveles de Grouping. En este caso, las tareas se agrupan por Propietario del Portfolio, Propietario del programa, Propietario del proyecto y Estado del proyecto. Solo puede tener hasta 3 niveles de agrupación mediante la interfaz estándar. Para agregar un cuarto nivel, debe utilizar el modo Texto. No se pueden agrupar informes por más de 4 criterios al mismo tiempo.
author: Nolan
feature: Reports and Dashboards
exl-id: a1780a57-b94c-4d3a-b526-9bf45dba21f1
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 0%

---

# Agrupación: agrupación de tareas de 4 niveles para Propietario del Portfolio, Propietario del programa, Propietario del proyecto y Estado del proyecto

<!--Audited: 10/2024-->

Esta tarea Grouping ofrece 4 niveles de Grouping. En este caso, las tareas se agrupan por Propietario del Portfolio, Propietario del programa, Propietario del proyecto y Estado del proyecto. Solo puede tener hasta 3 niveles de agrupación mediante la interfaz estándar. Para agregar un cuarto nivel, debe utilizar el modo Texto. No se pueden agrupar informes por más de 4 criterios al mismo tiempo.

![four_tier_grouping_for_tasks.png](assets/four-tier-grouping-for-tasks-350x239.png)

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> 
    <p>Nuevo:</p>
   <ul><li><p>Colaborador para modificar un filtro </p></li>
   <li><p>Estándar para modificar un informe</p></li> </ul>

<p>Actual:</p>
   <ul><li><p>Solicitud para modificar un filtro </p></li>
   <li><p>Plan para modificar un informe</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Informes, Tableros y Calendarios para modificar un informe</p> <p>Editar el acceso a filtros, vistas y agrupaciones para modificar un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Crear una agrupación de tareas de 4 niveles para el propietario del Portfolio, el propietario del programa, el propietario del proyecto y el estado del proyecto

Para aplicar esta agrupación:

1. Ir a una lista de tareas.
1. En el menú desplegable **Agrupación**, seleccione **Nueva agrupación**.

1. Haga clic en **Cambiar al modo de texto**.
1. Elimine el texto del área **Agrupar su informe**.
1. Reemplace el texto del cuadro mostrado con el siguiente código:
   <pre>group.0.linkedname=project<br>group.0.name=Portfolio Owner<br>group.0.notime=false<br>group.0.valuefield=project:portfolio:owner:name<br>group.0.valueformat=string<br>group.1.linkedname=project<br>group.1.name=Program Owner<br>group.1.notime=false<br>group.1.valuefield=project:program:owner:name<br>group.1.valueformat=string<br>group.2.linkedname=projectOwnerMM<br>group.2.listgrouingparsedmethod=nested(project).nested(owner).string(name)<br>group.2.namekey=projectownermm<br>group.2.notime=false<br>group.2.valuefield=projectOwnerMM:name<br>group.2.valueformat=string<br>group.3.enumclass=com.attask.common.ProjectStatusEnum<br>group.3 linkedname=project<br>group.3.namekey=view.relatedcolumn<br>group.3.namekeyargkey.0=project<br>group.3.namekeyargkey.1=status<br>group.3.notime=false<br>group.3.valuefield=project:status<br>group.3.valueformat=val</pre>

1. Haga clic en **Listo** y luego en **Guardar agrupación**.
1. (Opcional) Actualice el nombre de la agrupación y, a continuación, haga clic en **Guardar agrupación**.
