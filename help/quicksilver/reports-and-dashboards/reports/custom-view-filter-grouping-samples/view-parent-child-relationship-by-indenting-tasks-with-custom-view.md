---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ver: Muestra la relación principal-secundario en una tarea sangrando las tareas'
description: Puede mantener la distinción de relaciones principal-secundaria en una lista de tareas exportada añadiendo una vista personalizada a la lista de tareas y asegurándose de que esta vista esté seleccionada antes de exportar la lista.
author: Courtney
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/QSBA40vOIbB8cm0YydDuJN9NS2X6SoXNF-dCBUHFniM
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 244
ht-degree: 78%

---

# Vista: mostrar la relación principal y secundaria en una tarea aplicando una sangría a las tareas

<!--Audited: 11/2024-->

Puede mantener la distinción de relaciones principal-secundaria en una lista de tareas exportada añadiendo una vista personalizada a la lista de tareas y asegurándose de que esta vista esté seleccionada antes de exportar la lista.

![Sangría primaria secundaria](assets/parent-child-indented-custom-view-350x94.png)

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

## Mostrar la relación principal y secundaria en una tarea aplicando una sangría a las tareas

1. Vaya al proyecto con la lista de tareas que desee exportar.
1. Haga clic en el menú desplegable **Vista** y seleccione **Nueva vista**.
1. Haga clic en el encabezado de columna **Nombre de la tarea**.
1. Seleccione **Cambiar al modo de texto** en la esquina superior derecha.
1. Haga clic en **Editar modo de texto** y quite todo el texto existente.
1. Pegue el siguiente texto:


   ```
   displayname=
   linkedname=direct
   namekey=name
   querysort=name
   textmode=true
   valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(" - ",{name}),IF({indent}<3,CONCAT(" - - ",{name}),IF({indent}<4,CONCAT(" - - - ",{name}),CONCAT(" - - - - ",{name})))))
   valueformat=HTML
   ```

1. Haga clic en **Listo** > **Guardar vista**.
