---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: mostrar solo los elementos en un estado de aprobación'
description: Solo puede mostrar elementos en un estado determinado que esté actualmente en Aprobación pendiente. Funciona igual para cualquier otro objeto con un estado de aprobación.
author: Lisa and Courtney
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/nvD3qBAK0Y-k9P0Vzp9aY1GiHp2L5qVLCdkT32s698c
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 265
ht-degree: 76%

---

# Filtro: mostrar solo los elementos en un estado de aprobación

<!--Audited: 10/2024-->

Solo puede mostrar elementos en un estado determinado que esté actualmente en Aprobación pendiente. Funciona igual para cualquier otro objeto con un estado de aprobación.

Puede colocar los siguientes objetos en un estado de aprobación:

* Tareas
* Problemas
* Proyectos

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
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

## Mostrar solo los elementos en estado de aprobación

1. Ir a una lista de proyectos.
1. En el menú desplegable **Filtro**, seleccione **Nuevo filtro**.
1. Elija filtrar por **Proyecto: Estado** y, a continuación, seleccione el estado por el que desea filtrar en la lista.

   Por ejemplo, en un informe de proyecto, añada **Planificación de estado igual**, si desea mostrar solamente los proyectos que están en un estado de **Planificación: aprobación pendiente**.
1. Haga clic en **Modo de texto**.
1. Modifique la línea `status` agregando **:A** a la clave de 3 letras del estado:
   <pre>status=PLN:A<br>status_Mod=in</pre>

1. Haga clic en **Aplicar** > **Guardar como nuevo**.

   En la lista solo se muestran los proyectos que están en estado de Planificación: Aprobación pendiente.
