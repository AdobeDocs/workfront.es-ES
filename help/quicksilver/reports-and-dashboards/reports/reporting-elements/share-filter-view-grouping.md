---
product-area: reporting
navigation-topic: reporting-elements
title: Compartir un filtro, una vista o una agrupación
description: Puede compartir filtros, vistas y agrupaciones a las que tenga acceso para ver con otros usuarios.
author: Nolan
feature: Reports and Dashboards
exl-id: 63a6db90-d52c-4147-a442-7904ef9e9d49
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '1249'
ht-degree: 1%

---

# Compartir un filtro, una vista o una agrupación

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: CONSIDER SPLITTING THIS in three articles for each reporting element?)</p>
<p>(NOTE: This is linked from the TOC article in WF Basics > permissions section)&nbsp;</p>
</div>
-->

El administrador de Adobe Workfront concede a los usuarios acceso para ver o editar objetos cuando asignan niveles de acceso. Para obtener más información sobre la concesión de acceso a objetos, consulte [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Junto con el nivel de acceso que se concede a los usuarios, también puede concederles permisos para ver o editar objetos específicos que ha creado o tiene acceso para compartir. Para obtener más información sobre los niveles de acceso y los permisos, consulte [Cómo funcionan juntos los niveles de acceso y los permisos](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Puede compartir filtros, vistas y agrupaciones a las que tenga acceso para ver con otros usuarios.

Cuando se comparte un filtro, una vista o una agrupación con usted, puede aplicar ese filtro, esa vista o esa agrupación a sus listas. En función del acceso que se le conceda, puede modificarlo y compartirlo con otros usuarios.

Para obtener información sobre cómo crear un filtro, una vista o una agrupación, vea los siguientes artículos:

* [Resumen de filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Información general sobre vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Información general sobre agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

## Requisitos de acceso

Debe tener lo siguiente:

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
   <td> <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Acceso de visualización o superior a filtros, vistas y agrupaciones</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Ver o permisos superiores con acceso para compartir en una vista, filtro o agrupación</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Compartir un filtro, una vista o una agrupación

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: when the beta filters/ groupings come out either consider splitting this in different kinds of FVGs or splitting this article in FVGs for showing sharing on each one of them??)</p>
-->

El uso compartido de filtros en listas de selección es diferente en función de la interfaz que utilice para compartir el filtro: estándar o heredado. Para obtener información sobre los tipos de interfaces de generación de filtros, consulte [Creación o edición de filtros en Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

Solo puede compartir vistas y agrupaciones en la interfaz heredada.

### Uso compartido de filtros mediante la interfaz del generador estándar

Puede compartir un filtro en la interfaz estándar desde listas de proyectos, tareas, problemas, portafolios, programas, usuarios, plantillas o grupos. La interfaz del generador estándar para filtros no está disponible para ningún otro objeto, ni para vistas o agrupaciones.

Compartir un filtro mediante la interfaz del generador estándar:

1. Ir a una lista de proyectos, tareas o problemas.
1. Haga clic en **Filtrar** icono ![Icono de filtro](assets/filter-nwepng.png).

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

1. Pase el ratón sobre un filtro al que tenga acceso y, al menos, vea y comparta y, a continuación, haga clic en **Más** menú ![Menú Más](assets/more-icon-spectrum.png), luego haga clic en **Compartir**.

   ![Más opciones del menú](assets/new-filters-more-menu-options-with-delete.png)

   Se muestra el cuadro Compartir filtros.

1. Habilite la **Ver todo el sistema** configuración. Esto otorga permiso a los usuarios de Workfront para ver el filtro.

   >[!IMPORTANT]
   >
   >Utilice esta configuración con precaución. Añadir muchos filtros para todos los usuarios saturará la experiencia de filtrado y hará que los filtros sean más difíciles de encontrar.

   O Empiece a escribir los nombres de los usuarios, equipos, roles, grupos o empresas con los que desea compartir en **Conceder acceso a** field.

   ![Cuadro para compartir filtros](assets/new-filters-share-filter.png)

1. (Opcional) Haga clic en la flecha que señala a la derecha junto al nombre de una entidad para editar sus permisos en el filtro y, a continuación, habilite el **Ver** o **Administrar** opción. **Ver** es el valor predeterminado.

   ![Compartir permisos](assets/new-filters-sharing-permissions.png)

1. (Opcional) Habilite o deshabilite los permisos adicionales para una entidad mediante uno de los procedimientos siguientes:

   1. Clic **Ver** y deshabilite la **Compartir** opción. Está activada de forma predeterminada.
   1. Clic **Administrar** y deshabilite las **Compartir** o el **Eliminar** opción. Están habilitadas de forma predeterminada.

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

   Los filtros que ha compartido se muestran en **Compartido conmigo** del panel de filtro para esas entidades.

   ![Filtros compartidos conmigo](assets/new-filters-shared-with-me.png)

### Uso compartido de filtros, vistas y agrupaciones mediante la interfaz heredada

El uso compartido de filtros, vistas y agrupaciones en la interfaz heredada es idéntico.

1. Ir a una lista de objetos o a un informe.
1. (Condicional) En una lista, haga clic en **Filtrar**, **Ver**, o **Agrupación** y, a continuación, pase el ratón sobre el filtro, la vista o la agrupación que desee compartir y haga clic en **Más** icono ![Icono Más](assets/more-icon.png), entonces **Compartir**.

   En un informe, haga clic en **Filtrar**, **Ver**, o **Agrupación** menú desplegable y, a continuación, seleccione el filtro, vista o agrupación que desee compartir.

1. (Condicional) Si comparte datos de un informe, haga clic en **Filtrar**, **Ver**, o **Agrupación** menú desplegable de nuevo y haga clic en **Compartir filtro**, **Compartir vista**, o **Compartir agrupación**.\
   El **Filtrar acceso**, **Ver acceso**, o **Acceso de agrupación** aparece el cuadro de diálogo.

   ![Compartir filtro](assets/share-filter-people-box-nwe-350x458.png)

1. Complete cualquiera de las siguientes opciones, según con quién desee compartir:

   **Para compartir con usuarios, equipos, funciones, grupos o empresas individuales:** En el campo proporcionado, empiece a escribir el nombre del usuario, equipo, función, grupo o compañía con el que desea compartir y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.\
   Repita este proceso para compartir el acceso con varios usuarios, equipos, funciones, grupos o empresas.

   >[!TIP]
   >
   >Al compartir con grupos, se conceden permisos para filtrar, ver o agrupar a los miembros del grupo y de todos los subgrupos.

   **Para compartir con todos los usuarios del sistema:** Haga clic en **Configuración** y haga clic en **Hacer esto visible en todo el sistema**.\
   El administrador debe seleccionar la opción Compartir en todo el sistema para que esta opción esté disponible. Para obtener más información, consulte los artículos [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) y [Uso compartido de informes, tableros y calendarios](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

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
      <td> <p>Clic <strong>Configuración avanzada</strong>, luego seleccione o borre la <strong>Compartir</strong> , en función de si desea que los destinatarios puedan compartir con otros.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar**.

   Los usuarios con los que ha compartido el filtro, la vista o la agrupación pueden acceder a ella haciendo clic en el **Filtrar**, **Ver**, o **Agrupación** menú desplegable o icono y desplácese hacia abajo hasta el **Compartido conmigo** sección.


