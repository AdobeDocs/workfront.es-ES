---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Enumerar objetos con procesos de aprobación pendientes que utilizan un estado determinado
description: Si intenta eliminar un estado, un mensaje de error puede indicarle que no se puede eliminar porque se está utilizando en procesos de aprobación pendientes en objetos del sistema. Si desea buscar y revisar esos objetos para decidir lo que debe hacer, puede ejecutar un informe que los enumere.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 52dd8750-9a6f-4ac6-9779-ba4ea9b6f4e0
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# Enumerar objetos con procesos de aprobación pendientes que utilizan un estado determinado

Si intenta eliminar un estado, un mensaje de error puede indicarle que no se puede eliminar porque está en al menos un proceso de aprobación pendiente en el sistema. Puede ejecutar un informe para enumerar los objetos en los que se encuentra en un proceso de aprobación pendiente y, a continuación, decidir qué debe hacer para cada uno.

## En modo estándar

1. Vaya al área de **Informes** en la barra de navegación global y, a continuación, seleccione la pestaña **Informes**.
1. Haga clic en el icono del menú principal ![](assets/main-menu-icon.png) en la esquina superior derecha y, a continuación, haga clic en **Informes**.
1. Haga clic en **Nuevo informe** y, a continuación, seleccione **Informe de proyecto**, **Informe de tarea** o **Informe de problema**.
1. Abra la ficha **Filtros**.
1. Haga clic en **Agregar una regla de filtro** y, a continuación, haga lo siguiente para configurar la regla:
   1. Empiece a escribir `status` y seleccione **Estado** cuando se muestre.
   1. Deje **Equal** en el segundo campo.
   1. Seleccione el nombre del estado en el tercer campo.
1. Vuelva a hacer clic en **Agregar una regla de filtro** y, a continuación, haga lo siguiente para configurar la regla
   1. Empiece a escribir `pending status` y, a continuación, seleccione ese elemento cuando se muestre bajo el tipo de objeto que está buscando (**Proyecto**, **Tarea** o **Problema**).
   1. Deje **Equal** en el segundo campo.
   1. Escriba `in` en el tercer campo.
1. Vuelva a hacer clic en **Agregar una regla de filtro** y, a continuación, haga lo siguiente para configurar la regla
   1. Empiece a escribir el proceso de aprobación y, a continuación, seleccione **Id. de grupo** cuando se muestre en **Proceso de aprobación**.
   1. Seleccione **Está en blanco** en el segundo campo.
1. Haga clic en **Guardar + Cerrar** para ejecutar el informe y enumerar todos los objetos del tipo especificado con procesos de aprobación en estado pendiente según el estado especificado (**Proyecto**, **Tarea** o **Problema**).
1. Repita estos pasos para buscar la misma información para los otros dos tipos de objetos.


## En modo de texto

1. Haga clic en el icono del menú principal ![](assets/main-menu-icon.png) en la esquina superior derecha y, a continuación, haga clic en **Informes**.
1. Haga clic en **Nuevo informe** y, a continuación, seleccione **Informe de proyecto**, **Informe de tarea** o **Informe de problema**.
1. Abra la ficha **Filtros**.
1. Seleccione **Cambiar al modo de texto**.
1. Copie y pegue lo siguiente en la ventana de edición, sustituyendo XXX por la clave de 3 letras para el estado:

   `status=XXX`

   `status_Mod=in`

   `approvalProcess:groupID_Mod=isblank`

   Puede ver la clave en la lista de estados, como se muestra en estos artículos:
   * [Acceso a la lista de estados de proyectos del sistema](project-statuses.md)
   * [Acceso a la lista de estados de tareas del sistema](task-statuses.md)
   * [Acceso a la lista de estados de problemas del sistema](issue-statuses.md)

1. Haga clic en **Guardar + Cerrar** para ejecutar el informe y enumerar todos los objetos del tipo especificado con procesos de aprobación en estado pendiente según el estado especificado (**Proyecto**, **Tarea** o **Problema**).
1. Repita estos pasos para buscar la misma información para los otros dos tipos de objetos.
