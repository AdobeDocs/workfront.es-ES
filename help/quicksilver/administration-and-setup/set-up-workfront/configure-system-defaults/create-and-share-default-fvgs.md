---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Crear, editar y compartir filtros, vistas y agrupaciones predeterminados
description: Puede crear filtros, vistas y agrupaciones predeterminados y, a continuación, ponerlos a disposición de los usuarios de su organización.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 32eb825c-ba50-4820-a659-adc924a6ae52
source-git-commit: 3827e834a71084f14a99cb27aadefd97327b02d7
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 99%

---

# Crear, editar y compartir filtros, vistas y agrupaciones predeterminados

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Puede crear filtros, vistas y agrupaciones predeterminados y, a continuación, ponerlos a disposición de los usuarios de su organización.

Cuando se crean filtros, vistas y agrupaciones predeterminados como se describe en este artículo, los usuarios con los que se comparten pueden aprovecharlos al ver sus listas. Los usuarios pueden crear sus propios filtros, vistas y agrupaciones en función de los que cree usted, pero no pueden cambiar directamente los que cree.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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
   <td><p>Nuevo: [!UICONTROL Standard]</p>
   O
   <p>Actual: [!UICONTROL Plan]</p>
   </td> 
  </tr>
  <tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Crear filtros, vistas o agrupaciones predeterminados

{{step-1-to-setup}}

1. Realice una de las siguientes acciones, en función de si está creando o editando un filtro, una vista o una agrupación:

   * Haga clic en **[!UICONTROL Interfaz]** > **[!UICONTROL Filtros]**.

   * Haga clic en **[!UICONTROL Interfaz]** > **[!UICONTROL Vistas]**.

   * Haga clic en **[!UICONTROL Interfaz]** > **[!UICONTROL Agrupaciones]**.

1. Si está creando un filtro, una vista o una agrupación, haga clic en **[!UICONTROL Agregar filtro]**, **[!UICONTROL Agregar vista]** o **[!UICONTROL Agregar agrupación]** y, a continuación, seleccione el tipo de objeto con el que desea asociar el nuevo filtro, vista o agrupación.

   O

   Si está editando un filtro, una vista o una agrupación existentes, selecciónelo y luego haga clic en el icono **[!UICONTROL Editar]** ![Editar icono](assets/edit-icon.png).

1. Configure el filtro, la vista o la agrupación.

   Para obtener información sobre las opciones disponibles, consulte uno de los siguientes artículos:

   * [Información general de los filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [Información general de las vistas en [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [Información general sobre agrupaciones en [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

1. Haga clic en **[!UICONTROL Guardar]** cerca de la esquina inferior izquierda.

Puede poner el filtro, la vista o la agrupación a disposición de los usuarios de su sistema. Para obtener más información acerca de cómo compartir filtros, vistas o agrupaciones con otros usuarios, vea la sección [Hacer que los filtros, las vistas o las agrupaciones estén disponibles para los usuarios](#make-filters-views-or-groupings-available-to-users) en este artículo.


## Mostrar u ocultar los filtros, vistas o agrupaciones disponibles en la plantilla de diseño

Puede elegir mostrar u ocultar filtros, vistas o agrupaciones en la plantilla de diseño. Los filtros visibles están disponibles para todos los usuarios en todo el sistema. Puede utilizar una plantilla de diseño para ocultar filtros visibles para usuarios o grupos específicos.

>[!NOTE]
>
>Si un usuario utiliza activamente un filtro, una vista o una agrupación y, a continuación, un administrador lo desactiva, el usuario sigue teniendo acceso hasta que elija un nuevo filtro, vista o agrupación. Después de elegir un nuevo filtro, vista o agrupación, ya no se podrá volver al filtro, vista o agrupación oculto.

Para mostrar u ocultar los filtros, vistas o agrupaciones disponibles en la plantilla de diseño:

1. Haga clic en **[!UICONTROL Interfaz]** y, a continuación, haga clic en una de las siguientes opciones: **[!UICONTROL Filtros]**, **[!UICONTROL Vistas]** o **[!UICONTROL Agrupaciones]**.

1. (Condicional) Seleccione el filtro, vista o agrupación que desee poner a disposición de los usuarios y, a continuación, haga clic en **[!UICONTROL Habilitar en todo el sistema]**.

   ![](assets/enable-system-wide-fvg.png)

   >[!TIP]
   >
   >Si desea que el filtro, la vista o la agrupación siga estando disponible para la mayoría de los usuarios, pero no desea que otros usuarios lo vean, puede utilizar la plantilla de diseño. Para obtener más información, vea [Personalizar filtros, vistas y agrupaciones mediante una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. (Condicional) Seleccione el filtro, vista o agrupación que desea ocultar a los usuarios y, a continuación, haga clic en **[!UICONTROL Deshabilitar en todo el sistema]**. Una vez desactivado, el filtro, la vista o la agrupación se ocultarán de la plantilla de diseño, así como de los usuarios de todo el sistema.


## Hacer que los filtros, vistas o agrupaciones estén disponibles para todos los usuarios {#make-filters-views-or-groupings-available-to-users}

Estos pasos explican cómo hacer que los filtros, las vistas y las agrupaciones estén disponibles en el cuadro de diálogo [!UICONTROL Compartir] del área de [!UICONTROL Interfaz] en [!UICONTROL Configuración]. Esta configuración actúa como un interruptor de activación/desactivación para todo el sistema, incluida la plantilla de diseño.

{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Interfaz]** y, a continuación, haga clic en una de las siguientes opciones: **[!UICONTROL Filtros]**, **[!UICONTROL Vistas]** o **[!UICONTROL Agrupaciones]**.

1. Seleccione el filtro, la vista o la agrupación que desee poner a disposición de los usuarios y, a continuación, haga clic en el icono **[!UICONTROL Compartir]** ![Icono de compartir](assets/share-icon.png) para abrir el formulario [!UICONTROL Filtrar acceso], [!UICONTROL Ver acceso] o [!UICONTROL Agrupar acceso].
1. (Condicional) Para que el filtro, la vista o la agrupación estén disponibles para todos los usuarios del sistema, haga clic en el menú desplegable del **[!UICONTROL engranaje]** ![](assets/gear-menu-for-sharing-items.png) y, a continuación, haga clic en **[!UICONTROL Hacer esto visible en todo el sistema]**. Ahora todos los usuarios del sistema pueden ver el filtro, la vista o la agrupación.

   O

   Empiece a escribir el nombre de usuarios, equipos, funciones, grupos o empresas específicos con los que compartir el filtro, la vista o la agrupación y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.

   Para obtener más información acerca del uso compartido, vea [Información general sobre los permisos de uso compartido en objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Haga clic en **[!UICONTROL Guardar]**.

   Los usuarios que ha especificado ahora pueden ver el filtro, la vista o la agrupación predeterminados al ver el tipo de objeto con el que los asoció.

## Eliminación de filtros, vistas y agrupaciones

{{step-1-to-setup}}

1. Realice una de las siguientes acciones, en función de si va a eliminar un filtro, una vista o una agrupación:

   * Haga clic en **[!UICONTROL Interface]** > **[!UICONTROL Filters]**

   * Haga clic en **[!UICONTROL Interface]** > **[!UICONTROL Views]**

   * Haga clic en **[!UICONTROL Interfaz]** > **[!UICONTROL Agrupaciones]**

1. Seleccione uno o más elementos de la lista y, a continuación, haga clic en el icono **[!UICONTROL Eliminar]** ![Eliminar icono](assets/delete.png).
1. Consulte uno de los siguientes artículos para obtener información detallada sobre cómo configurar un filtro, una vista o una agrupación.

   * [Información general sobre filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [Información general sobre vistas en  [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [Información general sobre agrupaciones en  [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)
