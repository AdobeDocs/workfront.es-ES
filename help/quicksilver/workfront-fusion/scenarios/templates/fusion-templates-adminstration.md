---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Administración de plantillas de Adobe Workfront Fusion
description: Si es administrador, tiene permiso para ver, modificar, cambiar el nombre, publicar, aprobar y eliminar plantillas creadas por otros usuarios. Puede realizar estas acciones desde la página [!UICONTROL Plantillas] en el área  [!DNL Adobe Workfront Fusion Administration] .
author: Becky
feature: Workfront Fusion
exl-id: 63c14183-0d22-44f3-87e5-c311cfbf5540
source-git-commit: 2b67b5fb951b5ae7867144c444411ebd1c299e75
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 0%

---

# Administración de plantillas [!DNL Adobe Workfront Fusion]

Si es administrador, tiene permiso para ver, modificar, cambiar el nombre, publicar, aprobar y eliminar plantillas creadas por otros usuarios. Puede realizar estas acciones desde la página [!UICONTROL Plantillas] en el área [!DNL Adobe Workfront Fusion Administration].

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
   <p>Requisito de licencia actual: no se requiere licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo], [!UICONTROL [!DNL Workfront Fusion] para automatización de trabajo]</p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Requisito de producto actual: si tiene el plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], su organización debe adquirir [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en el plan [!DNL Workfront] de [!UICONTROL Ultimate].</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] y [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Debe ser administrador de Workfront Fusion para su organización.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Ver [!DNL Workfront Fusion] plantillas como administrador de [!DNL Workfront Fusion]

Para ver una tabla de todas las plantillas creadas y sus estados:

1. Haga clic en **[!UICONTROL Administración]** en el panel de navegación izquierdo para abrir el área de [!UICONTROL Administración].

   >[!NOTE]
   >
   >El área de Administración solo está visible para los administradores de Workfront Fusion.

1. Haga clic en **[!UICONTROL Plantillas]** en el panel de navegación izquierdo.

Existen tres columnas relacionadas con el estado de publicación de las plantillas. Una marca de verificación en una columna indica lo siguiente:

* **[!UICONTROL Publicadas]**: estas plantillas están visibles actualmente en la ficha [!UICONTROL Plantillas de equipo] de la interfaz de usuario.
* **[!UICONTROL Aprobación solicitada]**: estas plantillas están esperando su aprobación. Actualmente están visibles en la ficha [!UICONTROL Plantillas de equipo] de la interfaz de usuario.
* **[!UICONTROL Aprobadas]**: estas plantillas se aprobaron. Actualmente están visibles en la ficha [!UICONTROL Plantillas públicas] de la interfaz de usuario estándar.

>[!NOTE]
>
>Las plantillas con la marca de verificación en la columna [!UICONTROL Aprobación solicitada] y en la columna [!UICONTROL Aprobado] ya se han aprobado y se han hecho públicas, pero hay una versión más reciente de ellas esperando su aprobación.

## Editar [!DNL Workfront Fusion] plantillas como administrador

1. Haga clic en **[!UICONTROL Administración]** en el panel de navegación izquierdo para abrir el área de [!UICONTROL Administración].
1. Haga clic en **[!UICONTROL Plantillas]** en el panel de navegación izquierdo.
1. Haga clic en **[!UICONTROL Detalle]** a la derecha de la plantilla que desee editar.

Ahora puede editar la plantilla, de forma similar a la edición de una plantilla como usuario no administrador. Sin embargo, en [!UICONTROL Opciones], en la esquina superior derecha, hay una opción adicional: el diagrama del SVG que le proporciona el código del SVG. Además, el proceso de publicación es el mismo que en el caso de un usuario estándar, consulte la sección Publicación y uso compartido de plantillas para obtener más información.

Para obtener información acerca de las opciones de plantilla específicas que puede editar, vea [Crear nuevas plantillas en [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md).

Para obtener información sobre cómo publicar plantillas, consulte [Publish y compartir [!DNL Adobe Workfront Fusion] plantillas](../../../workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md).

## Aprobar o desaprobar [!DNL Workfront Fusion] plantillas

La aprobación de una plantilla la hace visible en la ficha [!UICONTROL Plantillas públicas] y disponible para todos los usuarios. Al desaprobar una plantilla, esta se eliminará de la ficha [!UICONTROL Plantillas públicas] y estará disponible solamente para el equipo que la creó.

1. Haga clic en **[!UICONTROL Administración]** en el panel de navegación izquierdo para abrir el área de [!UICONTROL Administración].
1. Haga clic en **[!UICONTROL Plantillas]** en el panel de navegación izquierdo.
1. Si desea aprobar una plantilla, haga clic en **[!UICONTROL Aprobar]** a la derecha de la plantilla.
1. Si desea desaprobar una plantilla, haga clic en **[!UICONTROL Desaprobar]** a la derecha de la plantilla.

>[!NOTE]
>
>Si está aprobando la plantilla que se aprobó anteriormente y luego se edita, la segunda aprobación sobrescribirá la plantilla original.

## Clonar un escenario como plantilla

Como administrador, tiene la capacidad de clonar un escenario como plantilla.

Para obtener instrucciones sobre cómo clonar un escenario como plantilla, consulte [Crear una plantilla a partir de un escenario](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md#create-a-template-from-a-scenario) en [Crear nuevas plantillas en [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md)
