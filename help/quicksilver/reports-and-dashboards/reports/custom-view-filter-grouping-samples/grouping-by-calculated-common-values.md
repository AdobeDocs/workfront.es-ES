---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Agrupación: organizar los resultados de la lista por un valor calculado común a todos los objetos de la agrupación'
description: Es posible que desee ver las tareas agrupadas por porcentaje completado en intervalos de 0-25, 26-50, 51-75, 75-99 y 100. Para ello, puede crear una agrupación mediante el modo de texto.
author: Nolan
feature: Reports and Dashboards
exl-id: 93b743ce-7e54-4a96-933b-912e2107a84f
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 81%

---

# Agrupación: organice los resultados de la lista por un valor calculado común a todos los objetos de la agrupación

<!--Audited: 10/2024-->

Es posible que desee ver las tareas agrupadas por porcentaje completado en intervalos de 0-25, 26-50, 51-75, 75-99 y 100. Para ello, puede crear una agrupación mediante el modo de texto.

![Agrupación por valor calculado](assets/grouping-calculated-value-column-to-all-objects.png)

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

## Organice los resultados de la lista por un valor calculado común a todos los objetos de la agrupación

Para aplicar esta agrupación a una lista de tareas:

1. Vaya a una lista de tareas.
1. En el menú desplegable **Agrupación** seleccione **Nueva agrupación**.

1. Haga clic en **Cambiar al modo de texto**.
1. En el espacio disponible, añada el siguiente código:

   ```
   textmode=true
   group.0.valueexpression=IF({percentComplete}>=0&&{percentComplete}<=25,'0-25%',IF({percentComplete}>25&&{percentComplete}<=50,'26-50%',IF({percentComplete}>50&&{percentComplete}<=75,'51-75%',IF({percentComplete}>75&&{percentComplete}<=100,'76-100%',''))))
   group.0.linkedname=direct
   group.0.valueformat=doubleAsString
   group.0.namekey=percentComplete
   ```

1. Haga clic en **Listo** y, a continuación, en **Guardar Agrupación**.
1. (Opcional) Actualice el nombre de la agrupación y, a continuación, haga clic en **Guardar agrupación**.
