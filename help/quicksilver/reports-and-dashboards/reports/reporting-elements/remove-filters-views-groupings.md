---
product-area: reporting
navigation-topic: reporting-elements
title: Eliminación de filtros, vistas y agrupaciones
description: Puede quitar un filtro, una vista o una agrupación de listas e informes si los ha creado o si se han compartido con usted. No se pueden quitar filtros, vistas o agrupaciones predeterminados.
author: Lisa
feature: Reports and Dashboards
exl-id: 422d262e-e19d-4070-85f1-77ecb7430342
source-git-commit: b56e6591c7da166bd1548420b562b838cc7fe0f2
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 0%

---

# Eliminación de filtros, vistas y agrupaciones

<span class="preview">Tenga en cuenta que en el entorno de vista previa, la experiencia de filtro mejorada (anteriormente denominada &quot;beta&quot;) es ahora la predeterminada. Estos filtros mejorados ahora son &quot;estándar&quot; y la experiencia de filtrado más antigua es &quot;heredada&quot;.</span>

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
   <td role="rowheader"><strong>plan Adobe Workfront*</strong></td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe Workfront*</strong></td> 
   <td> <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Acceso de visualización o superior a filtros, vistas y agrupaciones</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Ver los permisos con acceso para compartir en el filtro, vista o agrupación que desee quitar</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Quitar un filtro, una vista o una agrupación mediante el generador estándar

Puede quitar un filtro, una vista o una agrupación para todas las listas de objetos mediante la interfaz del generador estándar.

### Consideraciones acerca de la eliminación de filtros, vistas y agrupaciones

La forma de eliminar un elemento de creación de informes depende de si lo creó inicialmente o se compartió con usted.

Cuando se elimina una agrupación, existen los siguientes escenarios:

* **Si ha creado la agrupación y la elimina**, la agrupación se eliminará del sistema de Workfront. La agrupación ya no está disponible para los usuarios con los que la haya compartido anteriormente.
* **Si la agrupación se compartió con usted y la elimina**, la agrupación solo se eliminará automáticamente. El usuario que lo creó originalmente y cualquier otro usuario con el que se haya compartido siguen teniendo acceso a la agrupación.

### Quitar un filtro, una vista o una agrupación mediante el generador estándar

1. Ir a una lista de objetos o a un informe.
1. (Condicional) En una lista, haga clic en **Filtrar**, **Ver**, o **Agrupación** y, a continuación, pase el ratón sobre el filtro, la vista o la agrupación que quiera eliminar y haga clic en **Más** icono ![](assets/more-icon.png), entonces **Eliminar**. Se elimina el filtro, la vista o la agrupación.
1. (Condicional) En un informe, haga clic en **Agrupación**, **Filtrar**, o **Ver** menú desplegable y seleccione **Quitar agrupación**, **Quitar filtro**, o **Quitar vista**.

   El **Mis agrupaciones**, **Mis filtros,** o **Mis vistas** aparece el cuadro de diálogo.

   Todos los elementos de informe que tenga derechos para eliminar están disponibles para su eliminación. Otros elementos de informes se muestran atenuados.

1. Haga clic en **x** junto a cualquier elemento de informe que desee eliminar.
1. (Condicional) Haga clic en **Sí, eliminarla** si seleccionó eliminar un filtro, vista o agrupación que creó y luego compartió con otros. Esto elimina el filtro, la vista o la agrupación del sistema de Workfront.

   >[!TIP]
   >
   >Al eliminar un filtro, una vista o una agrupación que haya creado sin compartirlo con otros, se elimina del sistema sin solicitar una confirmación.

1. Clic **Listo**.

## Eliminación o eliminación de un filtro con el generador beta

Puede quitar un filtro que se haya compartido con usted de las listas de proyectos, tareas o problemas mediante la interfaz del generador beta. La interfaz del generador beta no está disponible para ningún otro objeto, ni para vistas o agrupaciones.

También puede eliminar los filtros que posea de las listas de proyectos, tareas o problemas mediante la interfaz del generador beta.

Los filtros predeterminados del sistema no se pueden eliminar.

### Consideraciones acerca de la eliminación de filtros mediante el generador beta

Cuando se elimina o elimina un filtro, se dan los siguientes casos:

* Si el filtro se compartió con usted y lo elimina, solo se eliminará por usted. El usuario que lo creó originalmente y cualquier otro usuario con el que se haya compartido siguen teniendo acceso al filtro.
* Si es el propietario del filtro y lo elimina, el filtro se elimina del sistema de Workfront. El filtro ya no está disponible para ningún usuario con el que lo haya compartido anteriormente.
* Si es administrador de Workfront, puede eliminar el filtro y se eliminará de forma permanente para todos los usuarios, incluido el propietario.

### Eliminación de un filtro mediante el generador beta

1. Ir a una lista de proyectos, tareas o problemas.
1. Haga clic en **Filtrar** icono ![Icono de filtro](assets/filter-nwepng.png) y habilite el generador de beta si es necesario.
1. Pase el ratón sobre un filtro **Compartido conmigo**, haga clic en **Más** menú ![Icono Más](assets/more-icon-spectrum.png), luego haga clic en **Eliminar**.

   ![Quitar filtro](assets/new-filters-more-menu-remove-filter.png)

1. Seleccionar **Eliminar** en el mensaje de confirmación para eliminar el filtro de forma permanente.

### Eliminación de un filtro mediante el generador beta

1. Ir a una lista de proyectos, tareas o problemas.
1. Haga clic en **Filtrar** icono ![Icono de filtro](assets/filter-nwepng.png) y habilite el generador de beta si es necesario.
1. Pase el ratón sobre un filtro que tenga permisos para eliminar y haga clic en el **Más** menú ![Icono Más](assets/more-icon-spectrum.png), luego haga clic en **Eliminar**.

   ![Eliminar filtro](assets/new-filters-more-menu-options-with-delete.png)

1. (Opcional) Haga clic en **Cancelar** en el mensaje de confirmación para evitar la eliminación y volver a la lista de filtros.
1. Clic **Eliminar** en el mensaje de confirmación para confirmar la eliminación.

   El filtro se elimina en su nombre y en el de todos los usuarios que tenían permisos para utilizarlo.

