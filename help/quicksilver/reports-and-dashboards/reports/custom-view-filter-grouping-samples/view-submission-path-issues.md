---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ver: Ruta de envío de problemas'
description: Puede mostrar la ruta a través de la cual se ha enviado un problema en la vista de un informe de problemas. La ruta indica la cola, el grupo de temas y el tema de la cola donde se envió el problema originalmente.
author: Nolan
feature: Reports and Dashboards
exl-id: bee1e066-c3f4-4d74-92b0-ab7f43d52a50
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 30%

---

# Ver: ruta de envío de problemas

<!--Audited: 11/2024-->

Puede mostrar la ruta a través de la cual se ha enviado un problema en la vista de un informe de problemas. La ruta indica la cola, el grupo de temas y el tema de la cola donde se envió el problema originalmente.

![ruta_envío_problema.png](assets/issue-submission-path-350x66.png)

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
   <p>Colaborador o solicitud para modificar una vista </p>
   <p>Estándar o Plan para modificar un informe</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Informes, Paneles de control y Calendarios para modificar un informe</p> <p>Edición del acceso a Filtros, Vistas y Agrupaciones para modificar una vista</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración para un informe</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Ver la ruta de envío de los problemas

1. Ir a una lista de problemas.
1. En el menú desplegable **Vista**, seleccione **Nueva vista**.

1. En el área **Vista previa de columna**, haga clic en **Agregar columna**.
1. Haga clic en el encabezado de la nueva columna y, a continuación, haga clic en **Cambiar al modo de texto** > **Editar modo de texto**.
1. Elimine el texto que encuentre en el cuadro **Editar modo de texto** y reemplácelo por el siguiente código:

   ```
   displayname= Issue Path
   linkedname=direct
   namekey=displayQueueBreadcrumb
   valuefield=displayQueueBreadcrumb
   valueformat=HTML
   ```

1. Haga clic en **Listo** > **Guardar vista**.
