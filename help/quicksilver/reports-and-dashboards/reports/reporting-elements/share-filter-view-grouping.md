---
product-area: reporting
navigation-topic: reporting-elements
title: Compartir un filtro, una vista o una agrupación
description: Puede compartir filtros, vistas y agrupaciones a las que tenga acceso para ver con otros usuarios.
author: Lisa
feature: Reports and Dashboards
exl-id: 63a6db90-d52c-4147-a442-7904ef9e9d49
source-git-commit: 8ac8981a40f051f11eef231397cd231ae1d8ddff
workflow-type: tm+mt
source-wordcount: '1332'
ht-degree: 0%

---

# Compartir un filtro, una vista o una agrupación

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: CONSIDER SPLITTING THIS in three articles for each reporting element?)</p>
<p>(NOTE: This is linked from the TOC article in WF Basics > permissions section)&nbsp;</p>
</div>
-->

El administrador de Adobe Workfront concede a los usuarios acceso para ver o editar objetos cuando asignen niveles de acceso. Para obtener más información sobre la concesión de acceso a objetos, consulte [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Junto con el nivel de acceso al que se concede a los usuarios, también puede concederles permisos para ver o editar objetos específicos que haya creado o que tengan acceso para compartir. Para obtener más información sobre los niveles de acceso y los permisos, consulte [Cómo funcionan juntos los niveles de acceso y los permisos](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Puede compartir filtros, vistas y agrupaciones a las que tenga acceso para ver con otros usuarios.

Cuando se comparte un filtro, una vista o una agrupación con usted, puede aplicar ese filtro, esa vista o esa agrupación a sus listas. Según el acceso que se le haya concedido, es posible que pueda modificarlo y compartirlo con otros usuarios.

Para obtener información sobre cómo crear un filtro, una vista o una agrupación, consulte los siguientes artículos:

* [Información general sobre filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Información general sobre las vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Información general sobre las agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
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
   <td> <p>Ver o permisos superiores con acceso para compartir en una vista, filtro o agrupación</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Compartir un filtro, una vista o una agrupación

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: when the beta filters/ groupings come out either consider splitting this in different kinds of FVGs or splitting this article in FVGs for showing sharing on each one of them??)</p>
-->

Puede compartir filtros en listas seleccionadas mediante las siguientes interfaces:

* Interfaz estándar
* Interfaz del generador beta

El uso compartido de filtros en listas seleccionadas es diferente en función de la interfaz que utilice para compartir el filtro. Para obtener información sobre los tipos de interfaces de generación de filtros, consulte [Crear o editar filtros en Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

Solo puede compartir vistas y agrupaciones en la interfaz estándar.

* [Uso compartido de filtros, vistas y agrupaciones mediante la interfaz estándar](#share-with-standard-interface)
* [Uso compartido de filtros con la interfaz del generador de beta](#share-with-beta-builder-interface)

### Uso compartido de filtros, vistas y agrupaciones mediante la interfaz estándar {#share-with-standard-interface}

El uso compartido de filtros, vistas y agrupaciones en la interfaz estándar es idéntico.

1. Vaya a una lista de objetos o a un informe.
1. (Condicional) En una lista, haga clic en el **Filtro**, **Ver** o **Agrupación** y, a continuación, pase el ratón sobre el filtro, la vista o la agrupación que desee compartir. **Más** icono ![Más icono](assets/more-icon.png), luego **Compartir**.

   En un informe, haga clic en el **Filtro**, **Ver** o **Agrupación** menú desplegable y, a continuación, seleccione el filtro, la vista o la agrupación que desee compartir.

1. (Condicional) Si comparte desde un informe, haga clic en el **Filtro**, **Ver** o **Agrupación** menú desplegable de nuevo y, a continuación, haga clic en **Compartir filtro**, **Compartir vista** o **Compartir grupo**.\
   La variable **Acceso a filtros**, **Ver acceso** o **Acceso a grupos** se abre.

   ![Filtro Compartir](assets/share-filter-people-box-nwe-350x458.png)

1. Complete cualquiera de las siguientes opciones, en función de con quién desee compartir:

   **Para compartir con usuarios, equipos, funciones, grupos o empresas individuales:** En el campo proporcionado, empiece a escribir el nombre del usuario, equipo, función, grupo o empresa con los que desee compartir y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.\
   Repita este proceso para compartir el acceso con varios usuarios, equipos, funciones, grupos o empresas.

   >[!TIP]
   >
   >El uso compartido con grupos proporciona permisos para el filtro, la vista o la agrupación a los miembros del grupo y de todos los subgrupos.


   **Para compartir con todos los usuarios del sistema:** Haga clic en el **Configuración** y, a continuación, haga clic en **Hacer que esto sea visible en todo el sistema**.\
   El administrador debe seleccionar la opción Compartir todo el sistema para que esta opción esté disponible. Para obtener más información, consulte los artículos [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) y [Compartir informes, tableros y calendarios](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

1. (Condicional) Si está compartiendo con usuarios, equipos, funciones, grupos o empresas individuales, haga clic en el menú desplegable para definir el nivel de acceso que desea conceder.

   Puede seleccionar entre las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Verlo</strong></td> 
      <td> <p>Seleccione esta opción para permitir que los destinatarios del recurso compartido solo utilicen el filtro, la vista o la agrupación compartidos. Cuando se selecciona esta opción, los destinatarios no pueden realizar ninguna modificación en el elemento compartido.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Administrarlo</strong></td> 
      <td> <p>Seleccione esta opción para permitir que los destinatarios del recurso compartido utilicen y modifiquen el filtro, la vista o la agrupación compartidos.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Compártala</strong></td> 
      <td> <p>Haga clic en <strong>Configuración avanzada</strong>y, a continuación, seleccione o borre la <strong>Compartir</strong> , en función de si desea que los destinatarios puedan compartir con otros.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar**.

   Los usuarios con los que haya compartido el filtro, la vista o la agrupación pueden acceder a él haciendo clic en el botón **Filtro**, **Ver** o **Agrupación** menú desplegable o icono y desplazarse hacia abajo hasta el **Compartido conmigo** para obtener más información.

### Uso compartido de filtros con la interfaz del generador de beta {#share-with-beta-builder-interface}

Al compartir filtros de listas de proyectos, tareas o problemas, puede compartirlos mediante la interfaz del generador beta en lugar de la interfaz estándar.

La interfaz del generador de beta no está disponible para ningún otro objeto de Workfront.

No se pueden crear filtros en la interfaz del generador de beta al crear informes.

Uso compartido de un filtro mediante la interfaz del generador beta:

1. Vaya a una lista de proyectos, tareas o problemas.
1. Haga clic en el **Filtro** icono ![Icono de filtro](assets/filter-nwepng.png)y, a continuación, active la variable **Configuración beta** ![Configuración beta](assets/beta-toggle-white-on-existing-filters.png) para acceder al generador beta. Está desactivado de forma predeterminada.

   A continuación, acepte el acuerdo beta si es necesario.

   Se abrirá la interfaz del generador de filtros beta.

   >[!TIP]
   >
   >El encabezado de la interfaz del generador cambia a azul cuando se activa el generador beta. Una vez que habilite la interfaz del generador beta, Workfront la mantendrá habilitada para todas las áreas en las que esté disponible.

   ![Generador de filtros beta](assets/new-filters-all-filter-types.png)

1. Revise las siguientes listas de filtros:

   <table style="table-layout:auto">
   <col>
   <col>
   <tbody>
   <tr>
   <td role="rowheader"><strong>Marcado como favorito</strong></td>
   <td>Filtros que ha marcado como favoritos. Cuando marque como favorito un filtro, su ubicación original se muestra debajo del nombre del filtro y se oculta en la lista original a menos que lo elimine como favorito.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Guardado</strong></td>
   <td>Filtros que ha creado y guardado usted mismo.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Valores predeterminados del sistema</strong></td>
   <td>Los filtros predeterminados del sistema de Workfront, así como los filtros que el administrador de Workfront agregó a su lista de filtros, ya sea en el nivel del sistema o en la plantilla de diseño.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Compartido conmigo</strong></td>
   <td>Filtros que otros usuarios crearon y compartieron con usted o que se comparten en todo el sistema.</td>
   </tr>
   </tbody>
   </table>

1. Pase el ratón sobre un filtro al que tenga acceso para ver y compartir al menos, y luego haga clic en el botón **Más** menú ![Más menú](assets/more-icon-spectrum.png)y haga clic en **Compartir**.

   ![Más opciones de menú](assets/new-filters-more-menu-options-with-delete.png)

   Se muestra el cuadro Compartir filtros .

1. Active la configuración Ver todo el sistema. Esto da permiso a cualquier usuario de Workfront para ver el filtro.

   >[!IMPORTANT]
   >
   >Utilice esta configuración con precaución. Añadir muchos filtros para todos los usuarios saturará la experiencia de filtrado y dificultará la búsqueda de filtros.

   O Empiece a escribir los nombres de los usuarios, equipos, roles, grupos o empresas con los que desee compartir en la **Dar acceso a** campo .

   ![Cuadro de uso compartido de filtros](assets/new-filters-share-filter.png)

1. (Opcional) Haga clic en la flecha que apunta a la derecha junto al nombre de una entidad para editar sus permisos para el filtro y, a continuación, active la opción **Ver** o **Administrar** . **Ver** es el valor predeterminado.

   ![Permisos de uso compartido](assets/new-filters-sharing-permissions.png)

1. (Opcional) Habilite o deshabilite los permisos adicionales para una entidad haciendo una de las siguientes acciones:

   1. Haga clic en **Ver** y deshabilite **Compartir** . Está activada de forma predeterminada.
   1. Haga clic en **Administrar** y deshabilite **Compartir** o **Eliminar** . Están activados de forma predeterminada.

      >[!NOTE]
      >
      >Si habilita Administrar acceso con la opción Eliminar , estos usuarios podrán eliminar el filtro de todos los usuarios, aunque no sean propietarios del filtro.
   >[!TIP]
   >
   >Los usuarios no pueden recibir permisos superiores a su nivel de acceso. Si no tienen acceso a los filtros de edición en su nivel de acceso, no pueden recibir permisos para administrar un filtro. Workfront deshabilita la opción Administrar para estos usuarios y la opción está atenuada.

1. Haga clic en **Compartir**. El filtro se comparte con las entidades especificadas.

   >[!TIP]
   >
   >Compartir con grupos da permisos al filtro para los miembros del grupo y de todos los subgrupos.

   Los filtros que ha compartido se muestran en la **Compartido conmigo** del panel de filtro para esas entidades.

   ![Filtros compartidos conmigo](assets/new-filters-shared-with-me.png)

