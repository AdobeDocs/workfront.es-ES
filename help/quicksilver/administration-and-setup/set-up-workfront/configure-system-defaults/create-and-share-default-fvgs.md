---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Crear, editar y compartir filtros, vistas y agrupaciones predeterminadas
description: Puede crear filtros, vistas y agrupaciones predeterminados y, a continuación, ponerlos a disposición de los usuarios de su organización.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 32eb825c-ba50-4820-a659-adc924a6ae52
source-git-commit: 75c4abfa9aebf1d07a851486391291cddc94f1a9
workflow-type: tm+mt
source-wordcount: '822'
ht-degree: 0%

---

# Crear, editar y compartir filtros, vistas y agrupaciones predeterminadas

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Puede crear filtros, vistas y agrupaciones predeterminados y, a continuación, ponerlos a disposición de los usuarios de su organización.

Cuando crea filtros, vistas y agrupaciones predeterminados como se describe en este artículo, los usuarios con los que los comparta pueden aprovecharlos al ver sus listas. Los usuarios pueden crear sus propios filtros, vistas y agrupaciones en función de los que haya creado, pero no pueden cambiar directamente los que haya creado.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser [!DNL Workfront] administrador.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Crear filtros, vistas o agrupaciones predeterminadas

{{step-1-to-setup}}

1. Realice una de las siguientes acciones, en función de si está creando o editando un filtro, una vista o una agrupación:

   * Haga clic en **[!UICONTROL Interfaz]** > **[!UICONTROL Filtros]**.

   * Haga clic en **[!UICONTROL Interfaz] >** **[!UICONTROL Vistas]**.

   * Haga clic en **[!UICONTROL Interfaz]** > **[!UICONTROL Agrupaciones]**.

1. Si está creando un filtro, una vista o una agrupación, haga clic en **[!UICONTROL Agregar filtro]**, **[!UICONTROL Agregar vista]** o **[!UICONTROL Agregar agrupación]** y, a continuación, seleccione el tipo de objeto con el que desee asociar el nuevo filtro, vista o agrupación.

   O

   Si está editando un filtro, una vista o una agrupación existentes, selecciónelo y haga clic en el botón **[!UICONTROL Editar]** icono ![Icono Editar](assets/edit-icon.png).

1. Configure el filtro, la vista o la agrupación.

   Para obtener información sobre las opciones disponibles, consulte uno de los siguientes artículos:

   * [Información general sobre filtros en [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [Información general sobre vistas en [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [Información general sobre las agrupaciones en [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

1. Haga clic en **[!UICONTROL Guardar]** cerca de la esquina inferior izquierda.

Puede hacer que el filtro, la vista o la agrupación estén disponibles para los usuarios del sistema. Para obtener más información sobre cómo compartir filtros, vistas o agrupaciones con otros usuarios, consulte la sección [Poner filtros, vistas o agrupaciones a disposición de los usuarios](#make-filters-views-or-groupings-available-to-users) en este artículo.


## Mostrar u ocultar filtros, vistas o agrupaciones disponibles en la plantilla Diseño

Puede elegir mostrar u ocultar filtros, vistas o agrupaciones de la plantilla de diseño. Hay filtros visibles disponibles para todos los usuarios de todo el sistema. Puede utilizar una plantilla de diseño para ocultar filtros visibles para usuarios o grupos específicos.

>[!NOTE]
>
>Si un usuario utiliza activamente un filtro, una vista o una agrupación y, a continuación, un administrador lo deshabilita, el usuario seguirá teniendo acceso hasta que elija un nuevo filtro, una vista o una agrupación. Después de elegir un nuevo filtro, vista o agrupación, ya no podrán volver al filtro, la vista o la agrupación ocultos.

Para mostrar u ocultar filtros, vistas o agrupaciones disponibles en la plantilla de diseño:

1. Haga clic en **[!UICONTROL Interfaz]** y, a continuación, haga clic en una de las siguientes opciones: **[!UICONTROL Filtros]**, **[!UICONTROL Vistas]** o **[!UICONTROL Agrupaciones]**.

1. (Condicional) Seleccione el filtro, la vista o la agrupación que desea poner a disposición de los usuarios y haga clic en **[!UICONTROL Habilitar en todo el sistema]**.

   ![](assets/enable-system-wide-fvg.png)

   >[!TIP]
   >
   >Si desea mantener el filtro, la vista o la agrupación disponibles para la mayoría de los usuarios, pero ocultarlo para otros, puede utilizar la plantilla Diseño. Para obtener más información, consulte [Personalización de filtros, vistas y grupos mediante una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. (Condicional) Seleccione el filtro, la vista o la agrupación que desea ocultar a los usuarios y haga clic en **[!UICONTROL Deshabilitar en todo el sistema]**. Una vez desactivado, el filtro, la vista o la agrupación se ocultarán en la plantilla de diseño, así como en los usuarios de todo el sistema.


## Poner filtros, vistas o agrupaciones a disposición de todos los usuarios {#make-filters-views-or-groupings-available-to-users}

En estos pasos se explica cómo hacer que los filtros, las vistas y las agrupaciones estén disponibles desde el [!UICONTROL Compartir] en el [!UICONTROL Interfaz] área [!UICONTROL Configuración]. Esta configuración funciona como un conmutador de encendido/apagado para todo el sistema, incluida la plantilla de diseño.

{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Interfaz]** y, a continuación, haga clic en una de las siguientes opciones: **[!UICONTROL Filtros]**, **[!UICONTROL Vistas]** o **[!UICONTROL Agrupaciones]**.

1. Seleccione el filtro, la vista o la agrupación que desea poner a disposición de los usuarios y, a continuación, haga clic en el botón **[!UICONTROL Compartir]** icono ![Icono Compartir](assets/share-icon.png) para abrir el [!UICONTROL Acceso a filtros], [!UICONTROL Ver acceso]o [!UICONTROL Acceso a grupos] formulario.
1. (Condicional) Para que el filtro, la vista o la agrupación estén disponibles para todos los usuarios del sistema, haga clic en el botón **[!UICONTROL Engranaje]** menú desplegable ![](assets/gear-menu-for-sharing-items.png)y haga clic en **[!UICONTROL Hacer que esto sea visible en todo el sistema]**. Todos los usuarios del sistema ahora pueden ver el filtro, la vista o la agrupación.

   O

   Empiece a escribir el nombre de usuarios, equipos, funciones, grupos o empresas específicos con los que compartir el filtro, la vista o la agrupación y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.

   Para obtener más información sobre el uso compartido, consulte [Información general sobre cómo compartir permisos en objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Haga clic en **[!UICONTROL Guardar]**.

   Los usuarios especificados ahora pueden ver el filtro, la vista o la agrupación predeterminados al ver el tipo de objeto con el que se asoció.

## Eliminar filtros, vistas y agrupaciones

{{step-1-to-setup}}

1. Realice una de las siguientes acciones, en función de si va a eliminar un filtro, una vista o una agrupación:

   * Haga clic en **[!UICONTROL Interfaz]** > **[!UICONTROL Filtros]**

   * Haga clic en **[!UICONTROL Interfaz]** > **[!UICONTROL Vistas]**

   * Haga clic en **[!UICONTROL Interfaz]** > **[!UICONTROL Agrupaciones]**

1. Seleccione uno o varios elementos de la lista y haga clic en el botón **[!UICONTROL Eliminar]** icono ![Icono Eliminar](assets/delete.png).
1. Consulte uno de los siguientes artículos para obtener información detallada sobre cómo configurar un filtro, una vista o una agrupación.

   * [Información general sobre filtros en [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [Información general sobre vistas en [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [Información general sobre las agrupaciones en [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)
