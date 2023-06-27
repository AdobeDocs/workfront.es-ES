---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Administración de plantillas de Adobe Workfront Fusion
description: Si es administrador, tiene permiso para ver, modificar, cambiar el nombre, publicar, aprobar y eliminar plantillas creadas por otros usuarios. Puede realizar estas acciones desde el [!UICONTROL Plantillas] página en la [!DNL Adobe Workfront Fusion Administration] área.
author: Becky
feature: Workfront Fusion
exl-id: 63c14183-0d22-44f3-87e5-c311cfbf5540
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] Administración de plantillas

Si es administrador, tiene permiso para ver, modificar, cambiar el nombre, publicar, aprobar y eliminar plantillas creadas por otros usuarios. Puede realizar estas acciones desde el [!UICONTROL Plantillas] página en la [!DNL Adobe Workfront Fusion Administration] área.

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
    <td> <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p> </td> 
   </tr>
  <tr> 
   <td role="rowheader">Licencia de [!UICONTROL Adobe Workfront Fusion]**</td> 
  <td>
   <p>Requisito de licencia actual: No [!DNL Workfront Fusion] requisito de licencia.</p>
   <p>O</p>
   <p>Requisito de licencia heredada: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo], [!UICONTROL [!DNL Workfront Fusion] para automatización de trabajo]</p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Requisito actual del producto: si tiene [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Debe ser administrador de Workfront Fusion para su organización.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Ver [!DNL Workfront Fusion] plantillas como administrador

Para ver una tabla de todas las plantillas creadas y sus estados:

1. Clic **[!UICONTROL Administration]** en el panel de navegación izquierdo para abrir [!UICONTROL Administration] área.
1. Clic **[!UICONTROL Plantillas]** en el panel de navegación izquierdo.

Existen tres columnas relacionadas con el estado de publicación de las plantillas. Una marca de verificación en una columna indica lo siguiente:

* **[!UICONTROL Publicado]**: estas plantillas están visibles actualmente en [!UICONTROL Plantillas de equipo] en la interfaz de usuario de.
* **[!UICONTROL Aprobación solicitada]**: estas plantillas están esperando su aprobación. Actualmente están visibles en [!UICONTROL Plantillas de equipo] en la interfaz de usuario de.
* **[!UICONTROL Aprobado]**: estas plantillas se han aprobado. Actualmente están visibles en [!UICONTROL Plantillas públicas] en la interfaz de usuario estándar.

>[!NOTE]
>
>Plantillas con la marca de verificación en ambas [!UICONTROL Aprobación solicitada] y en la columna [!UICONTROL Aprobado] Las columnas ya se han aprobado y se han hecho públicas, pero hay una versión más reciente de ellas a la espera de su aprobación.

## Editar [!DNL Workfront Fusion] plantillas como administrador

1. Clic **[!UICONTROL Administration]** en el panel de navegación izquierdo para abrir [!UICONTROL Administration] área.
1. Clic **[!UICONTROL Plantillas]** en el panel de navegación izquierdo.
1. Clic **[!UICONTROL Detalle]** a la derecha de la plantilla que desee editar.

Ahora puede editar la plantilla, de forma similar a la edición de una plantilla como usuario no administrador. Sin embargo, en el [!UICONTROL Opciones] en la esquina superior derecha, hay una opción adicional: el diagrama SVG que proporciona el código del SVG. Además, el proceso de publicación es el mismo que en el caso de un usuario estándar, consulte la sección Publicación y uso compartido de plantillas para obtener más información.

Para obtener información sobre las opciones de plantilla específicas que puede editar, consulte [Creación de nuevas plantillas en [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md).

Para obtener información sobre la publicación de plantillas, consulte [Publicación y uso compartido [!DNL Adobe Workfront Fusion] templates](../../../workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md).

## Aprobar o desaprobar [!DNL Workfront Fusion] templates

La aprobación de una plantilla la hace visible en el [!UICONTROL Plantillas públicas] y disponible para todos los usuarios. Al desaprobar una plantilla, esta se elimina del [!UICONTROL Plantillas públicas] y lo hace disponible solo para el equipo que lo creó.

1. Clic **[!UICONTROL Administration]** en el panel de navegación izquierdo para abrir [!UICONTROL Administration] área.
1. Clic **[!UICONTROL Plantillas]** en el panel de navegación izquierdo.
1. Si desea aprobar una plantilla, haga clic en **[!UICONTROL Aprobar]** a la derecha de la plantilla.
1. Si desea desaprobar una plantilla, haga clic en **[!UICONTROL Desaprobar]** a la derecha de la plantilla.

>[!NOTE]
>
>Si está aprobando la plantilla que se aprobó anteriormente y luego se edita, la segunda aprobación sobrescribirá la plantilla original.

## Clonar un escenario como plantilla

Como administrador, tiene la capacidad de clonar un escenario como plantilla.

Para obtener instrucciones sobre cómo clonar un escenario como plantilla, consulte [Creación de una plantilla a partir de un escenario](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md#create-a-template-from-a-scenario) in [Creación de nuevas plantillas en [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md)
