---
product-area: reporting
navigation-topic: reporting-elements
title: Eliminación de filtros, vistas y agrupaciones
description: Puede quitar un filtro, una vista o una agrupación de listas e informes si los ha creado o si se han compartido con usted. No se pueden quitar filtros, vistas o agrupaciones predeterminados.
author: Lisa
feature: Reports and Dashboards
exl-id: 422d262e-e19d-4070-85f1-77ecb7430342
source-git-commit: a3e4eb500570f86c689ef3bef654d659b9c465a2
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 0%

---

# Eliminación de filtros, vistas y agrupaciones

Puede quitar un filtro, una vista o una agrupación de listas e informes si los ha creado o si se han compartido con usted. No se pueden quitar filtros, vistas o agrupaciones predeterminados.

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plan de Adobe Workfront*</strong></td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe Workfront*</strong></td> 
   <td> <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Ver o acceder más a filtros, vistas y grupos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Ver permisos con acceso para compartir en el filtro, la vista o la agrupación que desee eliminar</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Eliminación de un filtro, una vista o una agrupación mediante el generador estándar

Puede quitar un filtro, una vista o una agrupación para todas las listas de objetos mediante la interfaz del generador estándar.

### Consideraciones sobre la eliminación de filtros, vistas y agrupaciones

La forma de eliminar un elemento de informe depende de si lo creó inicialmente o si se compartió con usted.

Los siguientes escenarios existen cuando se elimina una agrupación:

* **Si ha creado la agrupación y la ha eliminado**, la agrupación se elimina del sistema de Workfront. La agrupación ya no está disponible para ningún usuario con el que la haya compartido anteriormente.
* **Si la agrupación se compartió con usted y la elimina**, la agrupación se elimina únicamente por usted. El usuario que lo creó originalmente y cualquier otro usuario con el que se haya compartido siguen teniendo acceso a la agrupación.

### Eliminación de un filtro, una vista o una agrupación mediante el generador estándar

1. Vaya a una lista de objetos o a un informe.
1. (Condicional) En una lista, haga clic en el **Filtro**, **Ver** o **Agrupación** y, a continuación, pase el ratón sobre el filtro, la vista o la agrupación que desee eliminar. **Más** icono ![](assets/more-icon.png), luego **Eliminar**. Se elimina el filtro, la vista o la agrupación.
1. (Condicional) En un informe, haga clic en el **Agrupación**, **Filtro** o **Ver** menú desplegable y seleccione **Quitar agrupación**, **Quitar filtro** o **Quitar vista**.

   La variable **Mis grupos**, **Mis filtros,** o **Mis vistas** se abre.

   Todos los elementos de informes que tenga derechos para eliminar se pueden eliminar. Otros elementos de informes se muestran como atenuados.

1. Haga clic en el **x** junto a cualquier elemento de informe que desee eliminar.
1. (Condicional) Haga clic en **Sí, elimínelo** si ha seleccionado eliminar un filtro, una vista o una agrupación que haya creado y compartido posteriormente con otros usuarios. Esto elimina el filtro, la vista o la agrupación del sistema Workfront.

   >[!TIP]
   >
   >Al eliminar un filtro, una vista o una agrupación que haya creado sin compartirlo con otros, se elimina del sistema sin solicitar confirmación.

1. Haga clic en **Listo**.

## Eliminación o eliminación de un filtro mediante el generador de beta

Puede eliminar un filtro que se haya compartido con usted desde listas de proyectos, tareas o problemas a través de la interfaz del creador beta. La interfaz del generador de beta no está disponible para ningún otro objeto, ni para vistas o agrupaciones.

También puede eliminar filtros de su propiedad de listas de proyectos, tareas o problemas mediante la interfaz del creador beta.

Los filtros predeterminados del sistema no se pueden eliminar ni eliminar.

### Consideraciones sobre la eliminación o eliminación de filtros con el generador beta

Los siguientes escenarios existen cuando elimina o elimina un filtro:

* Si el filtro se compartió con usted y lo elimina, solo se eliminará por usted. El usuario que lo creó originalmente y cualquier otro usuario con el que se haya compartido siguen teniendo acceso al filtro.
* Si es propietario del filtro y lo elimina, este se elimina del sistema de Workfront. El filtro ya no está disponible para ningún usuario con el que lo haya compartido anteriormente.
* Si es administrador de Workfront, puede eliminar el filtro y este se elimina de forma permanente para todos los usuarios, incluido el propietario.

### Eliminación de un filtro mediante el generador de beta

1. Vaya a una lista de proyectos, tareas o problemas.
1. Haga clic en el **Filtro** icono ![Icono de filtro](assets/filter-nwepng.png) y habilite el generador beta si es necesario.
1. Pase el ratón sobre un filtro debajo de **Compartido conmigo**, haga clic en **Más** menú ![Más icono](assets/more-icon-spectrum.png)y haga clic en **Eliminar**.

   ![Quitar filtro](assets/new-filters-more-menu-remove-filter.png)

1. Select **Eliminar** en el mensaje de confirmación para eliminar permanentemente el filtro.

### Eliminación de un filtro mediante el generador de beta

1. Vaya a una lista de proyectos, tareas o problemas.
1. Haga clic en el **Filtro** icono ![Icono de filtro](assets/filter-nwepng.png) y habilite el generador beta si es necesario.
1. Pase el ratón sobre un filtro que tenga permisos para eliminar y haga clic en la **Más** menú ![Más icono](assets/more-icon-spectrum.png)y haga clic en **Eliminar**.

   ![Eliminar filtro](assets/new-filters-more-menu-options-with-delete.png)

1. (Opcional) Haga clic en **Cancelar** en el mensaje de confirmación para evitar la eliminación y volver a la lista de filtros.
1. Haga clic en **Eliminar** en el mensaje de confirmación para confirmar la eliminación.

   El filtro se elimina para usted y para todos los usuarios que tengan permisos para él.

