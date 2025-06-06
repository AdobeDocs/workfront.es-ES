---
product-area: reporting
navigation-topic: reporting-elements
title: Quitar filtros, vistas y agrupaciones
description: Puede quitar un filtro, una vista o una agrupación de listas e informes si los ha creado o si se han compartido con usted. No se pueden quitar filtros, vistas o agrupaciones predeterminados.
author: Nolan
feature: Reports and Dashboards
exl-id: 422d262e-e19d-4070-85f1-77ecb7430342
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 95%

---

# Quitar filtros, vistas y agrupaciones

<!-- Audited: 11/2024 -->

Puede quitar un filtro, una vista o una agrupación de listas e informes si los ha creado o si se han compartido con usted. No se pueden quitar filtros, vistas o agrupaciones predeterminados.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Plan de Adobe Workfront*</strong></td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe Workfront*</strong></td> 
   <td> 
      <p>Nuevo:</p>
         <ul>
         <li><p>Colaborador o superior</p></li>
         </ul>
      <p>Actual:</p>
         <ul>
         <li><p>Solicitud o superior</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td><p>Acceso de visualización o superior a filtros, vistas y agrupaciones</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td><p>Ver los permisos con acceso para compartir en el filtro, vista o agrupación que desee quitar</p>
   </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Quitar o eliminar un filtro con el generador estándar

Puede quitar un filtro que se haya compartido con usted de las listas de proyectos, tareas o problemas mediante la interfaz del generador estándar. La interfaz del generador estándar no está disponible para ningún otro objeto, ni para vistas o agrupaciones.

También puede eliminar los filtros que posea de las listas de proyectos, tareas o problemas mediante la interfaz del generador estándar.

Los filtros predeterminados del sistema no se pueden quitar o eliminar.

### Consideraciones sobre la eliminación de filtros mediante el generador estándar

Cuando se quita o elimina un filtro con el generador estándar, se dan los siguientes escenarios:

* Si el filtro se compartió con usted y lo elimina, solo se eliminará para usted. El usuario que lo creó originalmente y cualquier otro usuario con el que se haya compartido siguen teniendo acceso al filtro.
* Si es el propietario del filtro y lo elimina, el filtro se elimina del sistema de Workfront. El filtro ya no está disponible para ningún usuario con el que lo haya compartido anteriormente.
* Si es administrador de Workfront, puede eliminar el filtro y este se eliminará de forma permanente para todos los usuarios, incluido el propietario.

### Quite un filtro mediante el generador estándar

1. Vaya a una lista de proyectos, tareas, problemas, portafolios, programas, usuarios, plantillas o grupos.
1. Haga clic en el icono **Filtro** ![Icono de filtro](assets/filter-nwepng.png).
1. Pase el ratón sobre un filtro en **Compartido conmigo**, haga clic en el menú **Más** ![Icono de más](assets/more-icon-spectrum.png) y, a continuación, haga clic en **Quitar**.
1. Seleccione **Quitar** en el mensaje de confirmación para quitar el filtro de forma permanente.

### Elimine un filtro mediante el generador estándar

1. Vaya a una lista de proyectos, tareas, problemas, portafolios, programas, usuarios, plantillas o grupos.
1. Haga clic en el icono **Filtro** ![Icono de filtro](assets/filter-nwepng.png).
1. Pase el ratón sobre un filtro para el que tenga permisos para eliminarlo, haga clic en el menú **Más** ![Icono de más](assets/more-icon-spectrum.png) y, a continuación, haga clic en **Eliminar**.

   ![Eliminar filtro](assets/new-filters-more-menu-options-with-delete.png)

1. (Opcional) Haga clic en **Cancelar** en el mensaje de confirmación para que no se elimine y volver a la lista de filtros.
1. Haga clic en **Eliminar** en el mensaje de confirmación para confirmar su eliminación.

   El filtro se elimina para usted y todos los usuarios que tenían permisos para utilizarlo.

## Quitar un filtro, una vista o una agrupación mediante el generador heredado

Puede quitar un filtro, una vista o una agrupación para todas las listas de objetos mediante la interfaz del generador heredado.

### Consideraciones acerca de la eliminación de filtros, vistas y agrupaciones mediante el generador heredado

La forma de eliminar un elemento de creación de informes depende de si lo creó inicialmente o se compartió con usted.

Cuando se quita un filtro, una vista o una agrupación, existen los siguientes escenarios:

* **Si creó el elemento y lo quita**, se quita el elemento del sistema de Workfront. Ya no está disponible para ningún usuario con el que lo haya compartido anteriormente.
* **Si el elemento se compartió con usted y lo quita**, se quita el elemento sólo para usted. El usuario que lo creó originalmente y cualquier otro usuario con el que se haya compartido siguen teniendo acceso a él.

### Quitar un filtro, una vista o una agrupación mediante el generador heredado

1. Ir a una lista de objetos o a un informe.
1. (Condicional) En una lista, haga clic en el icono **Filtro**, **Vista** o **Agrupación** y, a continuación, pase el ratón sobre el filtro, la vista o la agrupación que desee quitar; haga clic en el icono **Más** ![Más iconos](assets/more-icon.png) y después en **Quitar**. Se elimina el filtro, la vista o la agrupación.
1. (Condicional) En un informe, haga clic en el menú desplegable **Agrupación**, **Filtro** o **Ver** y seleccione **Quitar agrupación**, **Quitar filtro** o **Quitar vista**.

   Se muestra el cuadro de diálogo **Mis agrupaciones**, **Mis filtros,** o **Mis vistas**.

   Todos los elementos de creación de informes de los cuales tenga derechos están disponibles para su eliminación. Otros elementos de creación de informes se muestran atenuados.

1. Haga clic en el icono **x** junto a cualquier elemento de informe que desee quitar.
1. (Condicional) Haga clic en **Sí, eliminarlo** si seleccionó quitar un filtro, una vista o una agrupación que creó y compartió posteriormente con otros usuarios. Esto elimina el filtro, la vista o la agrupación del sistema de Workfront.

   >[!TIP]
   >
   >Al quitar un filtro, una vista o una agrupación que haya creado sin compartirlo con otros, se quita del sistema sin solicitar una confirmación.

1. Haga clic en **Listo**.

