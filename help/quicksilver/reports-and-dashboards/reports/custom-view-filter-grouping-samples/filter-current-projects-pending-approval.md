---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filtro: mostrar los proyectos actuales con aprobación pendiente"
description: El siguiente filtro de proyecto muestra los proyectos en el estado Actual - Pendiente de aprobación, donde el usuario que ha iniciado sesión es el Patrocinador del proyecto o el Administrador de Portfolio.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 32045aec-acc5-44d2-bad5-7759dc797414
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 1%

---

# Filter: muestra los proyectos actuales con aprobación pendiente

El siguiente filtro de proyecto muestra los proyectos en el estado Actual - Pendiente de aprobación, donde el usuario que ha iniciado sesión es el Patrocinador del proyecto o el Administrador de Portfolio.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Solicitud para modificar un filtro </p>
   <p>Plan para modificar un informe</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar el acceso a Informes, Tableros y Calendarios para modificar un informe</p> <p>Editar el acceso a filtros, vistas y agrupaciones para modificar un filtro</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr>
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Filtrar proyectos actuales con aprobación pendiente

Para aplicar este filtro:

1. Ir a una lista de proyectos.
1. En el menú desplegable **Filtro**, seleccione **Nuevo filtro**.

1. Haga clic **Cambiar al modo de texto**.
1. En el área **Establecer reglas de filtro para su informe**, copie y pegue el siguiente código:
   <pre>status=CUR:A<br>esponsorID=$$USER.ID<br>O:a:status=CUR:A<br>O:a:portafolio:ownerID=$$USER.ID</pre>

1. Haga clic en **Guardar filtro**.
