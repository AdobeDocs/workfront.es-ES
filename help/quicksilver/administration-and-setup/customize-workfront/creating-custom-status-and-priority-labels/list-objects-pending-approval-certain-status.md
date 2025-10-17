---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Enumerar objetos con un proceso de aprobación pendiente que usa un estado determinado
description: Si intenta eliminar un estado, un mensaje de error puede indicarle que no se puede eliminar porque se está utilizando en procesos de aprobación pendientes en objetos del sistema. Si desea buscar y revisar esos objetos para decidir lo que debe hacer, puede ejecutar un informe que los enumere.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 52dd8750-9a6f-4ac6-9779-ba4ea9b6f4e0
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 14%

---

# Enumerar objetos con un proceso de aprobación pendiente que usa un estado determinado

Si intenta eliminar un estado, un mensaje de error puede indicarle que no se puede eliminar porque está en al menos un proceso de aprobación pendiente en el sistema. Puede ejecutar un informe para enumerar los objetos en los que se encuentra en un proceso de aprobación pendiente y, a continuación, decidir qué debe hacer para cada uno.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td>
     <p>Estándar</p>
     <p>Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td><p>Acceso de Edición a informes, paneles de control y calendarios</p><p>Acceso de edición a filtros, vistas y agrupaciones</p></td>
  </tr>
  <tr> 
   <td>Permisos de objeto</td> 
   <td>Puede obtener permisos de administración para los informes que cree.</td>
  </tr>
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## En modo estándar

{{step1-to-reports}}

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

{{step1-to-reports}}

1. Haga clic en **Nuevo informe** y, a continuación, seleccione **Informe de proyecto**, **Informe de tarea** o **Informe de problema**.
1. Abra la ficha **Filtros**.
1. Seleccione **Cambiar al modo de texto**.
1. Copie y pegue lo siguiente en la ventana de edición, sustituyendo XXX por la clave de 3 letras para el estado:

   `status=XXX`

   `status_Mod=in`

   `approvalProcess:groupID_Mod=isblank`

   Puede ver la clave en la lista de estados, como se muestra en estos artículos:
   * [Acceder a la lista de estados de proyectos del sistema](project-statuses.md)
   * [Acceso a la lista de estados de tareas del sistema](task-statuses.md)
   * [Acceso a la lista de estados de problemas del sistema](issue-statuses.md)

1. Haga clic en **Guardar + Cerrar** para ejecutar el informe y enumerar todos los objetos del tipo especificado con procesos de aprobación en estado pendiente según el estado especificado (**Proyecto**, **Tarea** o **Problema**).
1. Repita estos pasos para buscar la misma información para los otros dos tipos de objetos.
