---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: mostrar los proyectos actuales pendientes de aprobación'
description: El siguiente filtro de proyecto muestra los proyectos en el estado Actual - Pendiente de aprobación , donde el usuario que ha iniciado sesión es el Patrocinador del proyecto o el Administrador de Portfolio.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 32045aec-acc5-44d2-bad5-7759dc797414
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 0%

---

# Filtro: mostrar los proyectos actuales pendientes de aprobación

El siguiente filtro de proyecto muestra los proyectos en el estado Actual - Pendiente de aprobación , donde el usuario que ha iniciado sesión es el Patrocinador del proyecto o el Administrador de Portfolio.

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

## Filtrar proyectos actuales pendientes de aprobación

Para aplicar este filtro:

1. Vaya a una lista de proyectos.
1. En el **Filtro** menú desplegable, seleccione **Nuevo filtro**.

1. Haga clic en **Cambiar al modo de texto**.
1. En el **Definir reglas de filtro para el informe** , copie y pegue el siguiente código:
   <pre>status=CUR:A<br>sponsoredID=$$USER.ID<br>O:a:status=CUR:A<br>O:a:portafolio:ownerID=$$USER.ID</pre>

1. Haga clic en **Guardar filtro**.
