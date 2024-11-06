---
product-area: reporting
navigation-topic: reporting-elements
title: Compartir un filtro, una vista o una agrupación
description: Puede compartir filtros, vistas y agrupaciones a las que tenga acceso para ver con otros usuarios.
author: Nolan
feature: Reports and Dashboards
exl-id: 63a6db90-d52c-4147-a442-7904ef9e9d49
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '1178'
ht-degree: 1%

---

# Compartir un filtro, una vista o una agrupación

<!-- Audited: 11/2024 -->

<!--(NOTE: CONSIDER SPLITTING THIS in three articles for each reporting element?)
(NOTE: This is linked from the TOC article in WF Basics > permissions section)-->

El administrador de Adobe Workfront concede a los usuarios acceso para ver o editar objetos cuando asignan niveles de acceso. Para obtener más información acerca de la concesión de acceso a objetos, vea [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Junto con el nivel de acceso que se concede a los usuarios, también puede concederles permisos para ver o editar objetos específicos que ha creado o tiene acceso para compartir. Para obtener más información sobre los niveles de acceso y los permisos, vea [Cómo funcionan juntos los niveles de acceso y los permisos](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Puede compartir filtros, vistas y agrupaciones a las que tenga acceso para ver con otros usuarios.

Cuando se comparte un filtro, una vista o una agrupación con usted, puede aplicar ese filtro, esa vista o esa agrupación a sus listas. En función del acceso que se le conceda, puede modificarlo y compartirlo con otros usuarios.

Para obtener información sobre cómo crear un filtro, una vista o una agrupación, vea los siguientes artículos:

* [Resumen de filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Resumen de vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Información general sobre agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plan Adobe Workfront*</strong></td> 
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
   <td> <p>Acceso de visualización o superior a filtros, vistas y agrupaciones</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td><p>Ver o permisos superiores con acceso para compartir en una vista, filtro o agrupación</p></td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Compartir un filtro, una vista o una agrupación

<!--(NOTE: when the beta filters/ groupings come out either consider splitting this in different kinds of FVGs or splitting this article in FVGs for showing sharing on each one of them??)-->

El uso compartido de filtros en listas de selección es diferente en función de la interfaz que utilice para compartir el filtro: estándar o heredado. Para obtener información acerca de los tipos de interfaces de generación de filtros, vea [Crear o editar filtros en Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

Solo puede compartir vistas y agrupaciones en la interfaz heredada.

### Uso compartido de filtros mediante la interfaz del generador estándar

Puede compartir un filtro en la interfaz estándar desde listas de proyectos, tareas, problemas, portafolios, programas, usuarios, plantillas o grupos. La interfaz del generador estándar para filtros no está disponible para ningún otro objeto, ni para vistas o agrupaciones.

Compartir un filtro mediante la interfaz del generador estándar:

1. Ir a una lista de proyectos, tareas o problemas.
1. Haga clic en el icono **Filtro** ![Icono de filtro](assets/filter-nwepng.png).

   ![Generador de filtros estándar](assets/new-filters-all-filter-types.png)

1. Revise las siguientes listas de filtros:

   <table style="table-layout:auto">
   <col>
   <col>
   <tbody>
   <tr>
   <td role="rowheader"><strong>Marcado como favorito</strong></td>
   <td>Filtros que ha marcado como favoritos. Al marcar como favorito un filtro, su ubicación original se muestra debajo del nombre del filtro y se oculta de la lista original a menos que lo quite como favorito.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Guardado</strong></td>
   <td>Filtros que ha creado y guardado usted mismo. De forma predeterminada, esta lista muestra los filtros guardados en orden de los guardados más recientemente, pero los nombres de los filtros se pueden arrastrar para reordenar manualmente la lista.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Valores predeterminados del sistema</strong></td>
   <td>filtros predeterminados del sistema de Workfront, así como filtros que el administrador de Workfront agregó a su lista de filtros, ya sea en el nivel de sistema o en la plantilla de diseño.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Compartido conmigo</strong></td>
   <td>Filtros que otros han creado y compartido con usted o que se comparten en todo el sistema.</td>
   </tr>
   </tbody>
   </table>

1. Pase el ratón sobre un filtro al que tenga acceso para ver y compartir al menos. Luego, haga clic en el menú **Más** ![Menú más](assets/more-icon-spectrum.png) y, a continuación, haga clic en **Compartir**.

   ![Más opciones de menú](assets/new-filters-more-menu-options-with-delete.png)

   Se muestra el cuadro Compartir filtros.

1. Empiece a escribir los nombres de los usuarios, equipos, roles, grupos o empresas con los que desea compartir en el campo **Dar acceso a**.

   ![Cuadro para compartir filtros](assets/new-filters-share-filter.png)

1. (Opcional) Haga clic en la flecha que señala hacia la derecha junto al nombre de una entidad para editar sus permisos en el filtro y, a continuación, habilite la opción **Ver** o **Administrar**. **Vista** es la opción predeterminada.

   ![Permisos para compartir](assets/new-filters-sharing-permissions.png)

1. (Opcional) Habilite o deshabilite los permisos adicionales para una entidad mediante uno de los procedimientos siguientes:

   1. Haga clic en **Ver** y deshabilite la opción **Compartir**. Está activada de forma predeterminada.
   1. Haga clic en **Administrar** y deshabilite la opción **Compartir** o **Eliminar**. Están habilitadas de forma predeterminada.

      >[!NOTE]
      >
      >Si activa Administrar acceso con la opción Eliminar, estos usuarios podrán eliminar el filtro de todos los usuarios, aunque no sean propietarios del filtro.

   >[!TIP]
   >
   >Los usuarios no pueden recibir un permiso superior a su nivel de acceso. Si no tienen acceso a Editar filtros en su nivel de acceso, no pueden recibir permisos para administrar un filtro. Workfront deshabilita la opción Administrar para estos usuarios y la opción aparece atenuada.

1. Haga clic en **Compartir**. El filtro se comparte con las entidades especificadas.

   >[!TIP]
   >
   >Al compartir con grupos, se conceden permisos de filtrado a los miembros del grupo y de todos los subgrupos.

   Los filtros que compartió se muestran en la sección **Compartido conmigo** del panel de filtros para esas entidades.

   ![Filtros compartidos conmigo](assets/new-filters-shared-with-me.png)

### Uso compartido de filtros, vistas y agrupaciones mediante la interfaz heredada

El uso compartido de filtros, vistas y agrupaciones en la interfaz heredada es idéntico.

1. Ir a una lista de objetos o a un informe.
1. (Condicional) En una lista, haga clic en el icono **Filtro**, **Vista** o **Agrupación** y, a continuación, pase el ratón sobre el filtro, la vista o la agrupación que desee compartir; haga clic en el icono **Más** ![Más iconos](assets/more-icon.png) y después en **Compartir**.

   En un informe, haga clic en el menú desplegable **Filtro**, **Vista** o **Agrupación** y, a continuación, seleccione el filtro, la vista o la agrupación que desee compartir.

1. (Condicional) Si comparte datos de un informe, vuelve a hacer clic en el menú desplegable **Filtro**, **Vista** o **Agrupación** y, a continuación, haz clic en **Compartir filtro**, **Compartir vista** o **Compartir agrupación**.\
   Se muestra el cuadro de diálogo **Filtrar acceso**, **Ver acceso** o **Acceso de agrupación**.

   ![Compartir filtro](assets/share-filter-people-box-nwe-350x458.png)

1. Complete cualquiera de las siguientes opciones, según con quién desee compartir:

   **Para compartir con usuarios, equipos, roles, grupos o compañías individuales:** En el campo proporcionado, empiece a escribir el nombre del usuario, equipo, rol, grupo o compañía con el que desea compartir y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.\
   Repita este proceso para compartir el acceso con varios usuarios, equipos, funciones, grupos o empresas.

   >[!TIP]
   >
   >Al compartir con grupos, se conceden permisos para filtrar, ver o agrupar a los miembros del grupo y de todos los subgrupos.

   **Para compartir con todos los usuarios del sistema:** Haz clic en el icono **Configuración** y, a continuación, haz clic en **Hacer esto visible en todo el sistema**.\
   El administrador debe seleccionar la opción Compartir en todo el sistema para que esta opción esté disponible. Para obtener más información, vea los artículos [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) y [Compartir informes, paneles y calendarios](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

1. (Condicional) Si comparte contenido con usuarios, equipos, roles, grupos o empresas individuales, haga clic en el menú desplegable para definir el nivel de acceso que desea conceder.

   Puede seleccionar las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Verlo</strong></td> 
      <td> <p>Seleccione esta opción para permitir que los destinatarios del recurso compartido utilicen únicamente el filtro, la vista o la agrupación compartidos. Si se selecciona esta opción, los destinatarios no pueden realizar ninguna modificación en el elemento compartido.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Administrarlo</strong></td> 
      <td> <p>Seleccione esta opción para permitir que los destinatarios del recurso compartido utilicen y modifiquen el filtro, la vista o la agrupación compartidos.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Compártalo.</strong></td> 
      <td> <p>Haga clic en <strong>Configuración avanzada</strong> y, a continuación, active o desactive la opción <strong>Compartir</strong>, en función de si desea que los destinatarios puedan compartir con otros.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar**.

   Los usuarios con los que has compartido el filtro, la vista o la agrupación pueden acceder a ella haciendo clic en el menú desplegable **Filtro**, **Vista** o **Agrupación** o en el icono y desplazándose hacia abajo hasta la sección **Compartido conmigo**.


