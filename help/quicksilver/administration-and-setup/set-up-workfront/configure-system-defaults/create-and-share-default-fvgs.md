---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Crear, editar y compartir filtros, vistas y agrupaciones en todo el sistema
description: Puede crear filtros, vistas y agrupaciones predeterminados y, a continuación, ponerlos a disposición de los usuarios de su organización.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 32eb825c-ba50-4820-a659-adc924a6ae52
source-git-commit: 20ebcb74c79aea67ea7cb1ba083dfea623fe7c16
workflow-type: tm+mt
source-wordcount: '801'
ht-degree: 47%

---

# Crear, editar y compartir filtros, vistas y agrupaciones de todo el sistema

<!-- Audited: 5/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Puede crear filtros, vistas y agrupaciones y ponerlos a disposición de los usuarios de todo el sistema de su organización.

Al crear filtros, vistas y agrupaciones para todo el sistema como se describe en este artículo, los usuarios con los que los comparte pueden aprovecharlos al ver sus listas. Los usuarios pueden crear sus propios filtros, vistas y agrupaciones en función de los que cree, pero no pueden cambiarlos directamente.

Tenga en cuenta que los filtros, las vistas y las agrupaciones que crea en todo el sistema son diferentes de los predeterminados que Adobe Workfront crea automáticamente en el sistema. Estos filtros, vistas y agrupaciones predeterminados no se pueden editar ni eliminar.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquete</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licencia</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creación de filtros, vistas o agrupaciones

{{step-1-to-setup}}


1. Haga clic en **[!UICONTROL Interfaz]** y, a continuación, haga clic en una de las siguientes opciones: **[!UICONTROL Filtros]**, **[!UICONTROL Vistas]** o **[!UICONTROL Agrupaciones]**.

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


## Hacer que los filtros, vistas o agrupaciones estén disponibles para todos los usuarios {#make-filters-views-or-groupings-available-to-users}

Puede elegir mostrar u ocultar filtros, vistas o agrupaciones en el sistema. Los filtros visibles están disponibles para todos los usuarios en todo el sistema. Esta configuración actúa como un interruptor de activación/desactivación para todo el sistema, incluida la plantilla de diseño.

Si desea ocultar filtros, vistas o agrupaciones de usuarios específicos, le recomendamos que utilice una plantilla de diseño en lugar de desactivarlos en todo el sistema.

>[!NOTE]
>
>* Si un usuario utiliza activamente un filtro, una vista o una agrupación y, a continuación, un administrador lo desactiva, el usuario sigue teniendo acceso hasta que elija un nuevo filtro, vista o agrupación. Una vez que elijan una nueva, ya no podrán volver a la oculta.
>* Si todos los filtros, vistas y agrupaciones están restringidos a través de la plantilla de diseño o desactivados en todo el sistema, el usuario verá las opciones predeterminadas, ya que el sistema debe mostrar algo.

Para mostrar u ocultar filtros, vistas o agrupaciones:

{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Interfaz]** y, a continuación, haga clic en una de las siguientes opciones: **[!UICONTROL Filtros]**, **[!UICONTROL Vistas]** o **[!UICONTROL Agrupaciones]**.

1. (Condicional) Seleccione el filtro, vista o agrupación que desee poner a disposición de los usuarios y, a continuación, haga clic en **[!UICONTROL Habilitar en todo el sistema]**.

   ![](assets/enable-system-wide-fvg.png)

   >[!TIP]
   >
   >Si desea que el filtro, la vista o la agrupación estén disponibles para la mayoría de los usuarios, pero no para otros, puede utilizar la plantilla de diseño. Para obtener más información, consulte [Personalizar filtros, vistas y agrupaciones mediante una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. (Condicional) Seleccione el filtro, vista o agrupación que desee ocultar a los usuarios y, a continuación, haga clic en **[!UICONTROL Deshabilitar en todo el sistema]**. El filtro, la vista o la agrupación ahora están ocultos tanto para la plantilla de diseño como para los usuarios de todo el sistema.


## Compartir filtros, vistas o agrupaciones personalizadas con usuarios específicos

Estos pasos explican cómo compartir filtros, vistas y agrupaciones personalizadas con usuarios específicos mediante el cuadro de diálogo Compartir en el área de [!UICONTROL Interfaz] en [!UICONTROL Configuración]. Puede conceder acceso de visualización o administración a filtros, vistas y agrupaciones que usted u otros usuarios creen. No puede compartir valores predeterminados del sistema con los usuarios.


{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Interfaz]** y, a continuación, haga clic en una de las siguientes opciones: **[!UICONTROL Filtros]**, **[!UICONTROL Vistas]** o **[!UICONTROL Agrupaciones]**.

1. Seleccione el filtro, vista o agrupación que desee compartir y, a continuación, haga clic en el icono **[!UICONTROL Compartir]** ![Compartir icono](assets/share-icon.png).
1. Empiece a escribir el nombre de usuarios, equipos, funciones, grupos o empresas específicos con los que compartir el filtro, la vista o la agrupación y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.

   Para obtener más información acerca del uso compartido, vea [Información general sobre los permisos de uso compartido en objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Elija **Ver** o **Administrar** junto al nombre del usuario, equipo, rol, grupo o compañía. Para ajustar los permisos, haga clic en el icono del control deslizante y ajuste los permisos.

   ![ajustar permisos](assets/fine-tune-permissions.png)

1. Haga clic en **[!UICONTROL Guardar]**. Los usuarios que ha especificado ahora pueden interactuar con el filtro, la vista o la agrupación al ver el tipo de objeto con el que lo ha asociado.


## Eliminación de filtros, vistas y agrupaciones

{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Interfaz]** y, a continuación, haga clic en una de las siguientes opciones: **[!UICONTROL Filtros]**, **[!UICONTROL Vistas]** o **[!UICONTROL Agrupaciones]**.

1. Seleccione uno o más elementos de la lista y, a continuación, haga clic en el icono **[!UICONTROL Eliminar]** ![Eliminar icono](assets/delete.png).

1. En el cuadro de diálogo **Eliminar** que aparece, haga clic en **Sí, eliminarlo**.
