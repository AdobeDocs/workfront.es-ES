---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ver: Muestra la relación principal-secundario en una tarea sangrando las tareas'
description: Puede mantener la distinción de relaciones principal-secundaria en una lista de tareas exportada añadiendo una vista personalizada a la lista de tareas y asegurándose de que esta vista esté seleccionada antes de exportar la lista.
author: Nolan
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 85%

---

# Vista: mostrar la relación principal y secundaria en una tarea aplicando una sangría a las tareas

<!--Audited: 11/2024-->

Puede mantener la distinción de relaciones principal-secundaria en una lista de tareas exportada añadiendo una vista personalizada a la lista de tareas y asegurándose de que esta vista esté seleccionada antes de exportar la lista.

![Sangría primaria secundaria](assets/parent-child-indented-custom-view-350x94.png)

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p> Actual: 
   <ul>
   <li>Solicitud para modificar una vista</li> 
   <li>Plan para modificar un informe</li>
   </ul>
     </p>
     <p> Nuevo: 
   <ul>
   <li>Colaborador para modificar una vista</li> 
   <li>Estándar para modificar un informe</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar el acceso a Informes, Paneles de control y Calendarios para modificar un informe</p> <p>Edición del acceso a Filtros, Vistas y Agrupaciones para modificar una vista</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración para un informe</p> </td> 
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
