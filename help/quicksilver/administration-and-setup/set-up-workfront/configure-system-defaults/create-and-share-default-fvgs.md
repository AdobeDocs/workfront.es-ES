---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Crear, editar y compartir filtros, vistas y agrupaciones predeterminados
description: Puede crear filtros, vistas y agrupaciones predeterminadas y, a continuación, ponerlas a disposición de los usuarios de su organización.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 32eb825c-ba50-4820-a659-adc924a6ae52
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '820'
ht-degree: 0%

---

# Crear, editar y compartir filtros, vistas y agrupaciones predeterminados

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Puede crear filtros, vistas y agrupaciones predeterminadas y, a continuación, ponerlas a disposición de los usuarios de su organización.

Cuando se crean filtros, vistas y agrupaciones predeterminadas como se describe en este artículo, los usuarios con los que se comparten pueden aprovecharlas al ver sus listas. Los usuarios pueden crear sus propios filtros, vistas y agrupaciones en función de los que cree, pero no pueden cambiar directamente los que cree.

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
   <td> <p>Debe ser un [!DNL Workfront] administrador.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo [!DNL Workfront] El administrador puede modificar su nivel de acceso. Consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Crear filtros, vistas o agrupaciones predeterminadas

{{step-1-to-setup}}

1. Realice una de las siguientes acciones, en función de si está creando o editando un filtro, una vista o una agrupación:

   * Clic **[!UICONTROL Interfaz]** > **[!UICONTROL Filtros]**.

   * Clic **[!UICONTROL Interfaz] >** **[!UICONTROL Vistas]**.

   * Clic **[!UICONTROL Interfaz]** > **[!UICONTROL Agrupaciones]**.

1. Si va a crear un filtro, una vista o una agrupación, haga clic en **[!UICONTROL Añadir filtro]**, **[!UICONTROL Agregar vista]**, o **[!UICONTROL Agregar agrupación]**, a continuación, seleccione el tipo de objeto con el que desea asociar el nuevo filtro, vista o agrupación.

   O

   Si está editando un filtro, una vista o una agrupación existentes, selecciónelos y, a continuación, haga clic en **[!UICONTROL Editar]** icono ![Icono Editar](assets/edit-icon.png).

1. Configure el filtro, la vista o la agrupación.

   Para obtener información sobre las opciones disponibles, consulte uno de los siguientes artículos:

   * [Resumen de filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [Información general de vistas en [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [Información general sobre agrupaciones en [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

1. Clic **[!UICONTROL Guardar]** cerca de la esquina inferior izquierda.

Puede poner el filtro, la vista o la agrupación a disposición de los usuarios de su sistema. Para obtener más información sobre cómo compartir filtros, vistas o agrupaciones con otros usuarios, consulte la sección [Hacer que los filtros, vistas o agrupaciones estén disponibles para los usuarios](#make-filters-views-or-groupings-available-to-users) en este artículo.


## Mostrar u ocultar los filtros, vistas o agrupaciones disponibles en la plantilla de diseño

Puede elegir mostrar u ocultar filtros, vistas o agrupaciones desde la plantilla de diseño. Los filtros visibles están disponibles para todos los usuarios en todo el sistema. Puede utilizar una plantilla de diseño para ocultar filtros visibles para usuarios o grupos específicos.

>[!NOTE]
>
>Si un usuario utiliza activamente un filtro, una vista o una agrupación y, a continuación, un administrador lo desactiva, el usuario sigue teniendo acceso hasta que elija un nuevo filtro, una vista o una agrupación. Después de elegir un nuevo filtro, vista o agrupación, ya no podrán volver al filtro, vista o agrupación ocultos.

Para mostrar u ocultar los filtros, vistas o agrupaciones disponibles en la plantilla de diseño:

1. Clic **[!UICONTROL Interfaz]** y, a continuación, haga clic en una de las siguientes opciones: **[!UICONTROL Filtros]**, **[!UICONTROL Vistas]**, o **[!UICONTROL Agrupaciones]**.

1. (Condicional) Seleccione el filtro, vista o agrupación que desea poner a disposición de los usuarios y haga clic en **[!UICONTROL Habilitar en todo el sistema]**.

   ![](assets/enable-system-wide-fvg.png)

   >[!TIP]
   >
   >Si desea que el filtro, la vista o la agrupación sigan estando disponibles para la mayoría de los usuarios, pero no desea que lo vean otros usuarios, puede utilizar la plantilla de diseño. Para obtener más información, consulte [Personalización de filtros, vistas y agrupaciones mediante una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. (Condicional) Seleccione el filtro, vista o agrupación que desea ocultar a los usuarios y haga clic en **[!UICONTROL Deshabilitar en todo el sistema]**. Una vez desactivado, el filtro, la vista o la agrupación se ocultarán de la plantilla de diseño, así como de los usuarios de todo el sistema.


## Hacer que los filtros, vistas o agrupaciones estén disponibles para todos los usuarios {#make-filters-views-or-groupings-available-to-users}

Estos pasos explican cómo hacer que los filtros, las vistas y las agrupaciones estén disponibles en [!UICONTROL Compartir] diálogo en el [!UICONTROL Interfaz] área en [!UICONTROL Configurar]. Esta configuración actúa como un interruptor de activación/desactivación para todo el sistema, incluida la plantilla de diseño.

{{step-1-to-setup}}

1. Clic **[!UICONTROL Interfaz]** y, a continuación, haga clic en una de las siguientes opciones: **[!UICONTROL Filtros]**, **[!UICONTROL Vistas]**, o **[!UICONTROL Agrupaciones]**.

1. Seleccione el filtro, la vista o la agrupación que desee poner a disposición de los usuarios y, a continuación, haga clic en **[!UICONTROL Compartir]** icono ![Icono Compartir](assets/share-icon.png) para abrir [!UICONTROL Filtrar acceso], [!UICONTROL Ver acceso], o [!UICONTROL Acceso de agrupación] formulario.
1. (Condicional) Para que el filtro, la vista o la agrupación estén disponibles para todos los usuarios del sistema, haga clic en **[!UICONTROL Engranaje]** menú desplegable ![](assets/gear-menu-for-sharing-items.png), luego haga clic en **[!UICONTROL Hacer esto visible en todo el sistema]**. Ahora todos los usuarios del sistema pueden ver el filtro, la vista o la agrupación.

   O

   Empiece a escribir el nombre de usuarios, equipos, funciones, grupos o empresas específicos con los que compartir el filtro, la vista o la agrupación y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.

   Para obtener más información sobre cómo compartir, consulte [Información general sobre los permisos de uso compartido en objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Haga clic en **[!UICONTROL Guardar]**.

   Los usuarios que ha especificado ahora pueden ver el filtro, la vista o la agrupación predeterminados al ver el tipo de objeto con el que lo asoció.

## Eliminación de filtros, vistas y agrupaciones

{{step-1-to-setup}}

1. Realice una de las siguientes acciones, en función de si va a eliminar un filtro, una vista o una agrupación:

   * Clic **[!UICONTROL Interfaz]** > **[!UICONTROL Filtros]**

   * Clic **[!UICONTROL Interfaz]** > **[!UICONTROL Vistas]**

   * Clic **[!UICONTROL Interfaz]** > **[!UICONTROL Agrupaciones]**

1. Seleccione uno o varios elementos en la lista y, a continuación, haga clic en **[!UICONTROL Eliminar]** icono ![Icono Eliminar](assets/delete.png).
1. Consulte uno de los siguientes artículos para obtener información detallada sobre cómo configurar un filtro, una vista o una agrupación.

   * [Resumen de filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [Información general de vistas en [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [Información general sobre agrupaciones en [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)
