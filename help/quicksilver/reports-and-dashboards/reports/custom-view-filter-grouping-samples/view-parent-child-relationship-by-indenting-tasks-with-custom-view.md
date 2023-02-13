---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ver: mostrar la relación principal-secundario en una tarea sangrando las tareas'
description: Puede mantener la distinción entre relaciones principales y secundarias en una lista de tareas exportada añadiendo una vista personalizada a la lista de tareas y asegurándose de que esta vista esté seleccionada antes de exportar la lista.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 1%

---

# Ver: mostrar la relación principal-secundario en una tarea sangrando las tareas

Puede mantener la distinción entre relaciones principales y secundarias en una lista de tareas exportada añadiendo una vista personalizada a la lista de tareas y asegurándose de que esta vista esté seleccionada antes de exportar la lista.  

![](assets/parent-child-indented-custom-view-350x94.png)

1. Vaya al proyecto con la lista de tareas que desea exportar.
1. Haga clic en el **Ver** menú desplegable y seleccione **Nueva vista**.

1. Asigne un nombre al filtro en la esquina superior izquierda de la pantalla.
1. Haga clic en el **Nombre de la tarea** encabezado de columna.

1. Select **Cambiar al modo de texto** en la esquina superior derecha.
1. Haga clic en cualquier lugar del cuadro de texto para editar texto y elimine todo el texto existente.
1. Pegue el siguiente texto:

   ```
   displayname=<br>linkedname=direct<br>namekey=name<br>querysort=name<br>textmode=true<br>valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(" - ",{name}),IF({indent}<3,CONCAT(" - - ",{name}),IF({indent}<4,CONCAT(" - - - ",{name}),CONCAT(" - - - - ",{name})))))<br>valueformat=HTML
   ```

1. Haga clic en **Guardar**.
1. Haga clic en **Guardar vista**.
