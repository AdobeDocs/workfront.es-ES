---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Administración de plantillas de Adobe Workfront Fusion
description: Si es administrador, tiene permiso para ver, modificar, cambiar el nombre, publicar, aprobar y eliminar plantillas creadas por otros usuarios. Puede realizar estas acciones desde la [!UICONTROL Plantillas] en el [!DNL Adobe Workfront Fusion Administration] .
author: Becky
feature: Workfront Fusion
exl-id: 63c14183-0d22-44f3-87e5-c311cfbf5540
source-git-commit: bcca026e193e66cfb92ab9a0fb1aaf1eeb6892fb
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] Administración de plantillas

Si es administrador, tiene permiso para ver, modificar, cambiar el nombre, publicar, aprobar y eliminar plantillas creadas por otros usuarios. Puede realizar estas acciones desde la [!UICONTROL Plantillas] en el [!DNL Adobe Workfront Fusion Administration] .

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] o superior</p> </td> 
  </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
    <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
   </tr>
  <tr> 
   <td role="rowheader">Licencia de [!UICONTROL Adobe Workfront Fusion**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p><p>[!UICONTROL [!DNL Workfront Fusion] para la automatización del trabajo] </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Debe ser administrador de Workfront Fusion de su organización.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Ver [!DNL Workfront Fusion] plantillas como administrador

Para ver una tabla de todas las plantillas creadas y sus estados:

1. Haga clic en **[!UICONTROL Administración]** en el panel de navegación izquierdo para abrir el [!UICONTROL Administración] .
1. Haga clic en **[!UICONTROL Plantillas]** en el panel de navegación izquierdo.

Hay tres columnas relacionadas con el estado de publicación de las plantillas. Una marca de verificación en una columna indica lo siguiente:

* **[!UICONTROL Publicado]**: Estas plantillas están visibles actualmente en el [!UICONTROL Plantillas de equipo] en la interfaz de usuario.
* **[!UICONTROL Aprobación solicitada]**: Estas plantillas están esperando su aprobación. Actualmente están visibles en el [!UICONTROL Plantillas de equipo] en la interfaz de usuario.
* **[!UICONTROL Aprobado]**: Estas plantillas se han aprobado. Actualmente están visibles en el [!UICONTROL Plantillas públicas] en la interfaz de usuario estándar.

>[!NOTE]
>
>Plantillas con la marca de verificación en ambos [!UICONTROL Aprobación solicitada] y en la [!UICONTROL Aprobado] ya se han aprobado y publicado, pero hay una versión más reciente esperando su aprobación.

## Editar [!DNL Workfront Fusion] plantillas como administrador

1. Haga clic en **[!UICONTROL Administración]** en el panel de navegación izquierdo para abrir el [!UICONTROL Administración] .
1. Haga clic en **[!UICONTROL Plantillas]** en el panel de navegación izquierdo.
1. Haga clic en **[!UICONTROL Detalle]** a la derecha de la plantilla que desea editar.

Ahora puede editar la plantilla, de forma similar a editarla como un usuario no administrador. Sin embargo, en la variable [!UICONTROL Opciones] en la esquina superior derecha, hay una opción adicional: el diagrama de SVG que le proporciona el código de SVG. Además, el proceso de publicación es el mismo que en el caso de un usuario estándar, consulte la sección Publicación y uso compartido de plantillas para obtener más información.

Para obtener información sobre las opciones de plantilla específicas que puede editar, consulte [Cree nuevas plantillas en [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md).

Para obtener información sobre la publicación de plantillas, consulte [Publicar y compartir [!DNL Adobe Workfront Fusion] plantillas](../../../workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md).

## Aprobar o desaprobar [!DNL Workfront Fusion] plantillas

La aprobación de una plantilla la hace visible en el [!UICONTROL Plantillas públicas] y disponibles para todos los usuarios. Al desaprobar una plantilla, esta se elimina del [!UICONTROL Plantillas públicas] y lo hace disponible solo para el equipo que lo creó.

1. Haga clic en **[!UICONTROL Administración]** en el panel de navegación izquierdo para abrir el [!UICONTROL Administración] .
1. Haga clic en **[!UICONTROL Plantillas]** en el panel de navegación izquierdo.
1. Si desea aprobar una plantilla, haga clic en **[!UICONTROL Aprobar]** a la derecha de la plantilla.
1. Si desea desaprobar una plantilla, haga clic en **[!UICONTROL Desaprobar]** a la derecha de la plantilla.

>[!NOTE]
>
>Si está aprobando la plantilla que se aprobó anteriormente y luego editó, la segunda aprobación sobrescribirá la plantilla original.

## Clonar un escenario como plantilla

Como administrador, puede clonar un escenario como plantilla.

Para obtener instrucciones sobre la clonación de un escenario como plantilla, consulte [Creación de una plantilla a partir de un escenario](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md#create-a-template-from-a-scenario) en [Cree nuevas plantillas en [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md)
