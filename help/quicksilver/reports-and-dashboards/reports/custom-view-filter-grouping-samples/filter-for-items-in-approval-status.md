---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: mostrar solo los elementos en un estado de aprobación'
description: Solo puede mostrar elementos en un estado determinado que esté actualmente en Aprobación pendiente. Funciona igual para cualquier otro objeto con un estado de aprobación.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '265'
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
