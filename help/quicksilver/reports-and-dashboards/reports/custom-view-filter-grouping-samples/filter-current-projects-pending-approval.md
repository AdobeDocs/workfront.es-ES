---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: mostrar los proyectos actuales con aprobación pendiente'
description: 'El siguiente filtro de proyecto muestra los proyectos en el estado Actual: aprobación pendiente, donde el usuario que ha iniciado sesión es el Patrocinador del proyecto o el Administrador de portafolios.'
author: Lisa and Jenny
feature: Reports and Dashboards
exl-id: 32045aec-acc5-44d2-bad5-7759dc797414
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 78%

---

# Filtro: mostrar los proyectos actuales con aprobación pendiente

<!--Audited: 10/2024-->

El siguiente filtro de proyecto muestra los proyectos en el estado Actual - Aprobación pendiente, donde el usuario que ha iniciado sesión es el Patrocinador del proyecto o el Administrador de portafolios.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
   <p>Colaborador o solicitud para modificar un filtro </p>
   <p>Estándar o Plan para modificar un informe</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Informes, Paneles de control y Calendarios para modificar un informe</p> <p>Acceso de edición a filtros, vistas y agrupaciones para modificar un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración para un informe</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtrar proyectos actuales con aprobación pendiente

Para aplicar este filtro:

1. Ir a una lista de proyectos.
1. En el menú desplegable **Filtro**, seleccione **Nuevo filtro**.

1. Haga clic en **Modo de texto**.
1. En el área mostrada, copie y pegue el siguiente código:
   <pre>status=CUR:A<br>esponsorID=$$USER.ID<br>O:a:status=CUR:A<br>O:a:portafolio:ownerID=$$USER.ID</pre>

1. Haga clic en **Aplicar** > **Guardar como nuevo**.
