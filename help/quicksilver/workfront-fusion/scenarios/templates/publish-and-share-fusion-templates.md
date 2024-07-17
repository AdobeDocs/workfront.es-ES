---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Publish y compartir [!DNL Adobe Workfront Fusion] plantillas
description: Al crear una plantilla, esta estará disponible para todos los integrantes del equipo. Si desea compartir la plantilla con alguien que no pertenezca a su equipo, primero debe publicarla.
author: Becky
feature: Workfront Fusion
exl-id: aaa59a1e-aa16-41f5-9f56-ce0615c1b685
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 0%

---

# Publish y compartir [!DNL Adobe Workfront Fusion] plantillas

Al crear una plantilla, esta estará disponible para todos los integrantes del equipo. Si desea compartir la plantilla con alguien que no pertenezca a su equipo, primero debe publicarla.

Para obtener información sobre cómo crear una plantilla, consulte [Crear nuevas plantillas en Adobe Workfront Fusion](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md).

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] o superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de [!UICONTROL Adobe Workfront Fusion]**</td> 
  <td>
   <p>Requisito de licencia actual: no se requiere licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo], [!UICONTROL [!DNL Workfront Fusion] para automatización de trabajo]</p>
   </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Requisito de producto actual: si tiene el plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], su organización debe adquirir [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en el plan [!DNL Workfront] de [!UICONTROL Ultimate].</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] y [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Requisitos previos

Se debe crear una plantilla para poder compartirla.

## Publish y [!DNL Adobe Workfront Fusion] plantilla

1. En el panel de navegación izquierdo, haga clic en **[!UICONTROL Plantillas]**.
1. Haga clic en la ficha **[!UICONTROL Plantillas de equipo]**.
1. Haga clic en el nombre de la plantilla.
1. Haga clic en el botón **[!UICONTROL Publish]** en la esquina superior derecha de la pantalla.

## Compartir una plantilla [!DNL Workfront Fusion]

Después de publicar una plantilla, puede compartirla.

1. (Condicional) Si desea un vínculo que se pueda compartir, haga clic en **[!UICONTROL Compartir vínculo público]**.

   >[!NOTE]
   >
   >Puede compartir este vínculo con quien desee. La plantilla en sí permanece en la ficha [!UICONTROL Plantillas de equipo] y no es pública.

1. (Condicional) Si desea que la plantilla se haga pública, envíela al administrador para que la apruebe haciendo clic en **[!UICONTROL Solicitar aprobación]**.

   >[!NOTE]
   >
   >* Una vez aprobada la plantilla, se publica. [!UICONTROL Las plantillas públicas] están visibles en la ficha [!UICONTROL Plantillas públicas] para todos los usuarios de [!DNL Workfront Fusion], independientemente de la organización o del equipo.
   >* No se notifica al administrador acerca de la recepción de la plantilla para que la revise por correo electrónico. Si la aprobación es urgente, póngase en contacto directamente con el administrador.


## Estados de plantilla

Puede comprobar el estado en la página de la plantilla bajo el nombre de la plantilla

Los siguientes estados están disponibles:

* **[!UICONTROL Privada]**: esta plantilla solo está visible para el autor de la plantilla y su equipo.
* **[!UICONTROL Publicada]**: Esta plantilla solo es visible para el autor de la plantilla y su equipo. Puede enviar plantillas publicadas para su aprobación y copiar un vínculo que se puede compartir.
* **[!UICONTROL Aprobada]**: esta plantilla está visible para todos los usuarios de Workfront Fusion en la ficha [!UICONTROL Plantillas públicas]. Para copiar un vínculo que se puede compartir, haga clic en [!UICONTROL Opciones] en la esquina superior derecha de la pantalla.

También puede comprobar el estado desde la ficha [!UICONTROL Plantillas de equipo]. Si se publica una plantilla, aparecerá un icono a la derecha del nombre de la plantilla.

* **Icono en forma de ojo**: la plantilla está publicada, solo es visible para el equipo y no se envió la solicitud de aprobación.
* **Icono de marca de verificación amarilla**: la plantilla está publicada, solo es visible para el equipo y se envió la solicitud de aprobación.
* **Icono de marca de verificación verde**: La plantilla está publicada y es pública. Es visible para cualquier usuario de Workfront Fusion en la pestaña [!UICONTROL Plantillas públicas]. También sigue visible en la ficha [!UICONTROL Plantillas de equipo], y el autor de la plantilla o el miembro de su equipo aún pueden editarla.

Las plantillas sin iconos tienen el estado [!UICONTROL Privado]. No se publican y solo son visibles para el equipo.
