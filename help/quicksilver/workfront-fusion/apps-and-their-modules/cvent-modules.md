---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos Cvent
description: En un [!DNL Adobe Workfront Fusion] En este escenario, se pueden automatizar los flujos de trabajo que utilizan Cvent, así como conectarlo a varias aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion
exl-id: c95b9764-29a5-4d8c-8e6d-68a3969129e0
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1044'
ht-degree: 1%

---

# [!DNL Cvent] módulos

En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL Cvent], así como conectarlo a múltiples aplicaciones y servicios de terceros.

Si necesita instrucciones sobre cómo crear un escenario, consulte [Creación de un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obtener información sobre los módulos, consulte [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td>
   <p>Requisito de licencia actual: No [!DNL Workfront Fusion] requisito de licencia.</p>
   <p>O</p>
   <p>Requisito de licencia heredada: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p>
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
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Requisitos previos

Para usar [!DNL Cvent] módulos, debe tener un [!DNL Cvent] cuenta.

## Connect [!DNL Cvent] hasta [!DNL Adobe Workfront Fusion] {#connect-cvent-to-adobe-workfront-fusion}

>[!NOTE]
>
>El [!DNL Cvent] Los módulos de trabajan a través de [!UICONTROL JABÓN] API. Para crear una conexión con [!DNL Cvent], debe asegurarse de lo siguiente:
>
>* Tiene [!UICONTROL JABÓN] acceso a la [!DNL Cvent] API.
>* El [!DNL Workfront Fusion] Se han añadido direcciones IP a la lista de permitidos de su organización.
>
>  Para obtener una lista de [!DNL Workfront Fusion] Direcciones IP, consulte [Direcciones IP para acceder a [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)


Puede crear una conexión con su [!DNL Cvent] cuenta directamente desde dentro de un [!DNL Cvent] módulo.

1. En cualquier [!DNL Cvent] , haga clic en **[!UICONTROL Añadir]** junto al [!UICONTROL Conexión] field.
1. Seleccione la región a la que desea conectarse.

   * [!UICONTROL América del Norte]
   * [!UICONTROL Europa]
   * [!UICONTROL Espacio aislado]

1. Clic **[!UICONTROL Continuar]** para crear la conexión y volver al módulo.

## [!DNL Cvent] módulos y sus campos

Al configurar [!DNL Cvent] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, se añaden [!DNL Cvent] Los campos pueden mostrarse, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignación de información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Acciones](#actions)
* [Búsquedas](#searches)

### Acciones

* [[!UICONTROL Llamada de API personalizada]](#create-meeting-request)
* [[!UICONTROL Leer un registro]](#read-a-record)
* [[!UICONTROL Registrar invitado]](#register-invitee)
* [[!UICONTROL Añadir invitado]](#add-invitee)
* [[!UICONTROL Eliminar contacto]](#delete-contact)
* [[!UICONTROL Actualizar contacto]](#update-contact)
* [[!UICONTROL Crear convocatoria de reunión]](#create-meeting-request)

#### [!UICONTROL Llamada de API personalizada]

Este módulo de acción le permite realizar una llamada autenticada personalizada a [!DNL Cvent] API. De este modo, se puede crear una automatización del flujo de datos que el otro no puede realizar [!DNL Cvent] módulos.

Al configurar este módulo, se muestran los campos siguientes.

El módulo devuelve el código de estado a, junto con los encabezados y el cuerpo de la llamada de API.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Cvent] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] hasta [!DNL Adobe Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Operación</td> 
   td&gt; <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada de API. Para obtener más información, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Cvent] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] hasta [!DNL Adobe Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo de registro]</p> </td> 
   <td>Seleccione el tipo de elemento del registro que desea leer.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contacto] / [!UICONTROL Evento] / [!UICONTROL ID de invitación]</td> 
   <td> <p>Escriba o asigne el identificador del elemento que desea leer.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salidas]</td> 
   <td> <p>Seleccione los campos que desea incluir en la salida del módulo. Los campos están disponibles en función del tipo de elemento seleccionado.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Registrar invitado]

Este módulo de acción registra a un invitado para un evento.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Cvent] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] hasta [!DNL Adobe Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>ID de invitado</p> </td> 
   <td> <p>Introduzca o asigne el ID de la persona invitada que desea registrar para un evento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID de evento</td> 
   <td> <p>Introduzca o asigne el ID del evento para el que desea registrar al invitado.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Añadir invitado]

Este módulo de acción invita a un contacto a un evento.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Cvent] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] hasta [!DNL Adobe Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID de contacto]</p> </td> 
   <td> <p>Introduzca o asigne el ID del contacto que desea agregar a un evento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de evento]</td> 
   <td> <p>Introduzca o asigne el ID del evento al que desea agregar el contacto.</p> </td> 
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
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Cvent] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] hasta [!DNL Adobe Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de contacto]</td> 
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
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Cvent] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] hasta [!DNL Adobe Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID de contacto]</p> </td> 
   <td> <p>Introduzca o asigne el ID del contacto que desea actualizar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos]</td> 
   <td> <p>Seleccione los campos para los que desea introducir información y rellene los valores deseados para esos campos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos personalizados]</td> 
   <td> <p>Seleccione los campos para los que desea introducir información y rellene los valores deseados para esos campos.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear convocatoria de reunión]

Este módulo de acción agrega una convocatoria de reunión a su cuenta.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Cvent] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] hasta [!DNL Adobe Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID de formulario]</p> </td> 
   <td> <p>Escriba o asigne el identificador del formulario que desea utilizar para crear la nueva convocatoria de reunión.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos de convocatoria de reunión]</td> 
   <td> <p>Seleccione los campos de convocatoria de reunión para los que desea escribir información y, a continuación, rellene los valores deseados para esos campos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos de solicitud de eventos]</td> 
   <td> <p>Seleccione los campos de solicitud de evento para los que desea introducir información y, a continuación, rellene los valores deseados para esos campos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL RFP campos de solicitud]</td> 
   <td> <p>Seleccione los campos de solicitud de propuesta para los que desea introducir información y, a continuación, rellene los valores deseados para esos campos.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Búsquedas

#### [!UICONTROL Enumeración de registros]

Este módulo de búsqueda recupera información sobre todos los registros de un tipo específico.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Cvent] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] hasta [!DNL Adobe Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo de registro]</p> </td> 
   <td> <p>Seleccione el tipo de registro que desea enumerar.</p> 
    <ul> 
     <li> <p>Todos los eventos de su [!DNL Cvent] account</p> </li> 
     <li> <p>Todas las sesiones de un evento</p> </li> 
     <li> <p>Todos los invitados a un evento</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de evento]</td> 
   <td> <p>Si está enumerando invitados o sesiones, introduzca o asigne el ID del evento al que están asociados dichos invitados o sesiones.</p> </td> 
  </tr> 
 </tbody> 
</table>
