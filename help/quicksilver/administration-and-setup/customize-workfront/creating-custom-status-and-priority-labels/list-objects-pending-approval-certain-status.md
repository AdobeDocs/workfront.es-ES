---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Enumerar objetos con procesos de aprobación pendientes con un estado determinado
description: Si intenta eliminar un estado, un mensaje de error podría indicarle que no se puede eliminar porque se está utilizando en procesos de aprobación pendientes en objetos del sistema. Si desea buscar y revisar esos objetos para decidir qué debe hacer, puede ejecutar un informe que los enumere.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 52dd8750-9a6f-4ac6-9779-ba4ea9b6f4e0
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# Enumerar objetos con procesos de aprobación pendientes con un estado determinado

Si intenta eliminar un estado, un mensaje de error podría indicarle que no se puede eliminar porque está en al menos un proceso de aprobación pendiente en su sistema. Puede ejecutar un informe para enumerar los objetos en los que se encuentran en un proceso de aprobación pendiente y, a continuación, decidir qué debe hacer para cada uno de ellos.

## En modo Estándar

1. Vaya a la **Informes** en la barra de navegación global y, a continuación, seleccione la **Informes** pestaña .
1. Haga clic en el icono del menú principal ![](assets/main-menu-icon.png) en la esquina superior derecha, haga clic en **Informes**.
1. Haga clic en **Nuevo informe** y, a continuación, seleccione **Informe de proyecto**, **Informe de tareas** o **Informe de problemas**.
1. Abra el **Filtros** pestaña .
1. Haga clic en **Agregar una regla de filtro**, haga lo siguiente para configurar la regla:
   1. Empezar a escribir `status`y, a continuación, seleccione **Estado** cuando se muestre.
   1. Leave **Igual** en el segundo campo.
   1. Seleccione el nombre del estado en el tercer campo.
1. Haga clic en **Agregar una regla de filtro** de nuevo, haga lo siguiente para configurar la regla
   1. Empezar a escribir `pending status`y, a continuación, seleccione el elemento cuando aparezca debajo del tipo de objeto que está buscando (**Proyecto**, **Tarea** o **Problema**).
   1. Leave **Igual** en el segundo campo.
   1. Tipo `in` en el tercer campo.
1. Haga clic en **Agregar una regla de filtro** de nuevo, haga lo siguiente para configurar la regla
   1. Comience a escribir el proceso de aprobación y, a continuación, seleccione **ID de grupo** cuando aparece debajo de **Proceso de aprobación**.
   1. Select **Está en blanco** en el segundo campo.
1. Haga clic en **Guardar + Cerrar** para ejecutar el informe y enumere cualquier objeto del tipo especificado con los procesos de aprobación en estado pendiente en función del estado especificado (**Proyecto**, **Tarea** o **Problema**).
1. Repita estos pasos para encontrar la misma información para los otros dos tipos de objetos.


## En modo de texto

1. Haga clic en el icono del menú principal ![](assets/main-menu-icon.png) en la esquina superior derecha, haga clic en **Informes**.
1. Haga clic en **Nuevo informe** y, a continuación, seleccione **Informe de proyecto**, **Informe de tareas** o **Informe de problemas**.
1. Abra el **Filtros** pestaña .
1. Select **Cambiar al modo de texto**.
1. Copie y pegue lo siguiente en la ventana de edición, sustituyendo XXX por la clave de 3 letras para el estado:

   `status=XXX`

   `status_Mod=in`

   `approvalProcess:groupID_Mod=isblank`

   Puede ver la clave en la lista de estados, como se muestra en estos artículos:
   * [Acceso a la lista de estados de proyectos del sistema](project-statuses.md)
   * [Acceso a la lista de estados de tareas del sistema](task-statuses.md)
   * [Acceda a la lista de estados de problemas del sistema](issue-statuses.md)

1. Haga clic en **Guardar + Cerrar** para ejecutar el informe y enumere cualquier objeto del tipo especificado con los procesos de aprobación en estado pendiente en función del estado especificado (**Proyecto**, **Tarea** o **Problema**).
1. Repita estos pasos para encontrar la misma información para los otros dos tipos de objetos.
