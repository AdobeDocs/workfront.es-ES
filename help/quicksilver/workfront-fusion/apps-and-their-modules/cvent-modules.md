---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos Cvent
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: c95b9764-29a5-4d8c-8e6d-68a3969129e0
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1111'
ht-degree: 89%

---

# Módulos de [!DNL Cvent]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Módulos Cvent](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/cvent-modules.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

En un escenario de [!DNL Adobe Workfront Fusion], puede automatizar los flujos de trabajo que utilizan [!DNL Cvent], así como conectarlo a varias aplicaciones y servicios de terceros.

Si necesita instrucciones para crear un escenario, consulte [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obtener información acerca de los módulos, consulte [Módulos de  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Requisitos de acceso

Para utilizar la funcionalidad de este artículo debe tener el siguiente acceso:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] o superior</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td>
   <p>Requisito de licencia actual: no se requiere ninguna licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Producto</td> 
   <td>
   <p>Requisito de producto actual: si tiene el plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], su organización debe adquirir [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en el plan [!DNL Workfront] de [!UICONTROL Ultimate].</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] y [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr>
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Requisitos previos

Para usar módulos [!DNL Cvent], debe tener una cuenta de [!DNL Cvent].

## Información de Cvent API

El conector Cvent utiliza lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Versión de API</td> 
   <td> V200611.ASMX </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Etiqueta de API</td> 
   <td>Versión 1.7.14</td> 
  </tr>
 </tbody> 
 </table>

## Conectar [!DNL Cvent] a [!DNL Adobe Workfront Fusion] {#connect-cvent-to-adobe-workfront-fusion}

>[!NOTE]
>
>Los módulos de [!DNL Cvent] funcionan a través de una API [!UICONTROL SOAP].  Para crear una conexión con [!DNL Cvent] debe asegurarse de lo siguiente:
>
>* Dispone de acceso [!UICONTROL SOAP] a la API de [!DNL Cvent].
>* Se han añadido las direcciones IP de [!DNL Workfront Fusion] a la lista de permitidos de su organización.
>
>  Para obtener una lista de direcciones IP de [!DNL Workfront Fusion], consulte [Direcciones IP para acceder a [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)


Puede crear una conexión con su cuenta de [!DNL Cvent] directamente desde un módulo de [!DNL Cvent].

1. En cualquier módulo de [!DNL Cvent], haga clic en **[!UICONTROL Añadir]** junto al campo [!UICONTROL Conexión].
1. Seleccione la región a la que desea conectarse.

   * [!UICONTROL América del Norte]
   * [!UICONTROL Europa]
   * [!UICONTROL Zona protegida]

1. Haga clic en **[!UICONTROL Continuar]** para crear la conexión y volver al módulo.

## Módulos de [!DNL Cvent] y sus campos

Al configurar módulos de [!DNL Cvent], [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL Cvent] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. El título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Acciones](#actions)
* [Búsquedas](#searches)

### Acciones

* [[!UICONTROL Llamada de API personalizada]](#create-meeting-request)
* [[!UICONTROL Leer un registro]](#read-a-record)
* [[!UICONTROL Registrar Invitado]](#register-invitee)
* [[!UICONTROL Añadir Invitado]](#add-invitee)
* [[!UICONTROL Eliminar contacto]](#delete-contact)
* [[!UICONTROL Actualizar contacto]](#update-contact)
* [[!UICONTROL Crear solicitud de reunión]](#create-meeting-request)

#### [!UICONTROL Llamada de API personalizada]

Este módulo de acción le permite realizar una llamada autenticada personalizada a la API [!DNL Cvent]. De este modo, puede crear una automatización del flujo de datos imposibles de realizar por los otros [!DNL Cvent] módulos.

Al configurar este módulo, se muestran los campos siguientes.

El módulo devuelve el código de estado, junto con los encabezados y el cuerpo de la llamada de API.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar la cuenta de [!DNL Cvent] a [!DNL Workfront Fusion], consulte <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Cvent] a [!DNL Adobe Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Operación</td> 
   td&gt; <p>Seleccione el método de petición HTTP que necesita para configurar la llamada de la API. Para obtener más información, vea <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de petición HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Cuerpo (XML)</td> 
   <td> <p>Introduzca o asigne el cuerpo de la llamada de API. Esto debe incluir únicamente el XML. El módulo incluirá automáticamente los encabezados de autenticación. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Leer un registro]

Este módulo de acción lee información sobre un registro específico.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Cvent] a [!DNL Workfront Fusion], consulte <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Cvent] a [!DNL Adobe Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Record type]</p> </td> 
   <td>Seleccione el tipo de elemento del registro que quiera leer.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contact] / [!UICONTROL Event] / [!UICONTROL Invitee ID]</td> 
   <td> <p>Escriba o asigne el identificador del elemento que quiera leer.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Seleccione los campos que desea incluir en la salida del módulo. Los campos están disponibles en función del tipo de elemento seleccionado.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Registrar invitado]

Este módulo de acción registra a un invitado a un evento.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Cvent] a [!DNL Workfront Fusion], consulte <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Cvent] a [!DNL Adobe Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>ID de invitado</p> </td> 
   <td> <p>Introduzca o asigne el ID de la persona invitada que quiera registrar a un evento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID de evento</td> 
   <td> <p>Introduzca o asigne el ID del evento para el que quiera registrar al invitado.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Añadir Invitado]

Este módulo de acción invita a un contacto a un evento.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Cvent] a [!DNL Workfront Fusion], consulte <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Cvent] a [!DNL Adobe Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Contact ID]</p> </td> 
   <td> <p>Introduzca o asigne el ID del contacto que quiera añadir a un evento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event ID]</td> 
   <td> <p>Introduzca o asigne el ID del evento al que quiera añadir el contacto.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar contacto]

Este módulo de acción elimina un solo contacto en Cvent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Cvent] a [!DNL Workfront Fusion], consulte <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Cvent] a [!DNL Adobe Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contact ID]</td> 
   <td> <p>Introduzca o asigne el ID del contacto que desea eliminar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actualizar contacto]

Este módulo de acción actualiza un contacto existente mediante su ID.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Cvent] a [!DNL Workfront Fusion], consulte <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Cvent] a [!DNL Adobe Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Contact ID]</p> </td> 
   <td> <p>Introduzca o asigne el ID del contacto que desea actualizar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields]</td> 
   <td> <p>Seleccione los campos para los que desea introducir información y rellene los valores deseados para esos campos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Custom fields]</td> 
   <td> <p>Seleccione los campos para los que desea introducir información y rellene los valores deseados para esos campos.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear solicitud de reunión]

Este módulo de acción añade una convocatoria de reunión a su cuenta.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones sobre la conexión de su cuenta de [!DNL Cvent] a [!DNL Workfront Fusion], consulte <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Cvent] a [!DNL Adobe Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Form ID]</p> </td> 
   <td> <p>Escriba o asigne el ID del formulario que desea utilizar para crear la nueva convocatoria de reunión.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Meeting Request Fields]</td> 
   <td> <p>Seleccione los campos de convocatoria de reunión para los que desea escribir información y, a continuación, rellene los valores deseados para esos campos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event Request Fields]</td> 
   <td> <p>Seleccione los campos de solicitud de evento para los que desea introducir información y, a continuación, rellene los valores deseados para esos campos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL RFP Request Fields]</td> 
   <td> <p>Seleccione los campos de solicitud de propuesta para los que desea introducir información y, a continuación, rellene los valores deseados para esos campos.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Búsquedas

#### [!UICONTROL Enumerar registros]

Este módulo de búsqueda recupera información sobre todos los registros de un tipo específico.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Cvent] a [!DNL Workfront Fusion], consulte <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Cvent] a [!DNL Adobe Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Record type]</p> </td> 
   <td> <p>Seleccione el tipo de registro que desea enumerar.</p> 
    <ul> 
     <li> <p>Todos los eventos de su cuenta de [!DNL Cvent]</p> </li> 
     <li> <p>Todas las sesiones de un evento</p> </li> 
     <li> <p>Todos los invitados a un evento</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event ID]</td> 
   <td> <p>Si está enumerando invitados o sesiones, introduzca o asigne el ID del evento al que están asociados dichos invitados o sesiones.</p> </td> 
  </tr> 
 </tbody> 
</table>
