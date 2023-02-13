---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Agrupación: Agrupación de tareas de 4 niveles para Propietario del Portfolio, Propietario del Programa, Propietario del Proyecto y Estado del Proyecto"
description: Esta tarea Grouping proporciona 4 niveles de Grouping. En este caso, las tareas se agrupan por propietario del Portfolio, propietario del programa, propietario del proyecto y estado del proyecto. Solo puede tener hasta 3 niveles de agrupación mediante la interfaz estándar. Para añadir un cuarto nivel, debe utilizar el modo de texto. No se pueden agrupar los informes por más de 4 criterios al mismo tiempo.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a1780a57-b94c-4d3a-b526-9bf45dba21f1
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---

# Agrupación: Agrupación de tareas de 4 niveles para el propietario del Portfolio, el propietario del programa, el propietario del proyecto y el estado del proyecto

Esta tarea Grouping proporciona 4 niveles de Grouping. En este caso, las tareas se agrupan por propietario del Portfolio, propietario del programa, propietario del proyecto y estado del proyecto. Solo puede tener hasta 3 niveles de agrupación mediante la interfaz estándar. Para añadir un cuarto nivel, debe utilizar el modo de texto. No se pueden agrupar los informes por más de 4 criterios al mismo tiempo.

![four_tier_grouping_for_tasks.png](assets/four-tier-grouping-for-tasks-350x239.png)

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Editar acceso a filtros, vistas y grupos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en un informe</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Crear un grupo de tareas de 4 niveles para el propietario del Portfolio, el propietario del programa, el propietario del proyecto y el estado del proyecto

Para aplicar esta agrupación:

1. Vaya a una lista de tareas.
1. En el **Agrupación** menú desplegable, seleccione **Nuevo grupo**.

1. Haga clic en **Cambiar al modo de texto**.
1. Elimine el texto de la sección **Agrupar su informe** .
1. Reemplace el texto por el siguiente código:

   <pre>group.0.linkedname=project<br>group.0.name=Propietario del Portfolio<br>group.0.notime=false<br>group.0.valuefield=project:portfolio:propietario:nombre<br>group.0.valueformat=string<br>group.1.linkedname=project<br>group.1.name=Propietario del programa<br>group.1.notime=false<br>group.1.valuefield=project:program:propietario:nombre<br>group.1.valueformat=string<br>group.2.linkedname=projectOwnerMM<br>group.2.listgrouingparsedmethod=nested(project).nested(owner).string(name)<br>group.2.namekey=projectownermm<br>group.2.notime=false<br>group.2.valuefield=projectOwnerMM:name<br>group.2.valueformat=string<br>group.3.enumclass=com.attask.common.constants.ProjectStatusEnum<br>group.3.linkedname=project<br>group.3.namekey=view.relatedcolumn<br>group.3.namekeyargkey.0=project<br>group.3.namekeyargkey.1=status<br>group.3.notime=false<br>group.3.valuefield=project:status<br>group.3.valueformat=val</pre>

1. Haga clic en **Guardar agrupación**.
