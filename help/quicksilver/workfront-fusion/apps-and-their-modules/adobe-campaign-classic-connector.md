---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de Adobe Campaign v7/v8
description: Con el [!DNL Adobe Campaign] módulos, puede iniciar un [!DNL Adobe Workfront Fusion] según los eventos de su [!DNL Adobe Campaign] crear, leer o actualizar acuerdos y otros registros, buscar registros con los criterios definidos y cargar documentos.
author: Becky
feature: Workfront Fusion
exl-id: 84e8fa35-0c3c-46bd-8886-88c6d8d9e1d5
source-git-commit: 7decc5cbf4bb2c3d4d1802dec1f369ca061f6b48
workflow-type: tm+mt
source-wordcount: '1434'
ht-degree: 0%

---

# [!DNL Adobe Campaign] módulos

Con el [!DNL Adobe Campaign] módulos, puede iniciar un [!DNL Adobe Workfront Fusion] según los eventos de su [!DNL Adobe Campaign v7/v8] Cuenta de, crear, leer o actualizar registros, buscar registros con los criterios establecidos y realizar llamadas de API personalizadas.

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

Debe añadir las direcciones IP de Fusion a [!DNL Adobe Campaign].

* Para obtener instrucciones sobre cómo añadir direcciones IP a la lista de permitidos de Campaign, consulte [Añadir direcciones IP a la lista de permitidos](https://experienceleague.adobe.com/en/docs/control-panel/using/sftp-management/ip-range-allow-listing#adding-ip-addresses-allow-list) en la documentación de Adobe Campaign.
* Para obtener una lista de direcciones IP que añadir a la lista de permitidos, consulte [Direcciones IP para acceder a Adobe Workfront Fusion](/help/quicksilver/workfront-fusion/get-started/ip-addresses-for-fusion.md).

## Connect [!DNL Adobe Campaign] hasta [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Se recomienda encarecidamente crear una conexión servidor a servidor. Adobe Campaign ha actualizado su API para aceptar solo conexiones de servidor a servidor. Si se está conectando a la versión 8 o superior de Campaign, debe **debe** crear una conexión servidor a servidor.
>
>Para obtener más información sobre los nuevos requisitos de conexión de Campaign, consulte [Migración de los operadores técnicos de Campaign a la consola de Adobe Developer](https://experienceleague.adobe.com/docs/campaign/technotes-ac/tn-new/ims-migration.html) en la documentación de Campaign.

1. En cualquier [!DNL Adobe Campaign] , haga clic en **[!UICONTROL Añadir]** junto al [!UICONTROL Conexión] field.
1. Rellene los campos siguientes:
   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[!UICONTROL Tipo de conexión]</td>
          <td>
            <p>Seleccione si va a crear una conexión básica o una conexión servidor a servidor.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Nombre de conexión]</td>
          <td>
            <p>Escriba un nombre para esta conexión.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL URL base]</td>
          <td>Introduzca la URL base que utiliza para conectarse a su [!DNL Adobe Campaign] ejemplo.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Nombre de usuario]</td>
          <td>Si está creando una conexión básica, introduzca su nombre de usuario de Adobe Campaign.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Contraseña]</td>
          <td>Si está creando una conexión básica, introduzca la contraseña de Adobe Campaign.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL ID de cliente]</td>
          <td>Si está creando una conexión servidor a servidor, escriba su [!DNL Adobe] [!UICONTROL ID de cliente]. Esto se puede encontrar en la sección [!UICONTROL Credentials details] del [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Secreto de cliente]</td>
          <td>Si está creando una conexión servidor a servidor, escriba su [!DNL Adobe] [!UICONTROL Secreto de cliente]. Esto se puede encontrar en la sección [!UICONTROL Credentials details] del [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Entorno]</td>
          <td>Seleccione si está conectado a un entorno de producción o de no producción.
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Tipo]</td>
          <td>Seleccione si desea conectarse a una cuenta de servicio o a una cuenta personal.
        </tr>
   </tbody>
    </table>
1. Clic **[!UICONTROL Continuar]** para crear la conexión y volver al módulo.

## [!DNL Adobe Campaign] módulos y sus campos

Al configurar [!DNL Adobe Campaign] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, se añaden [!DNL Adobe Campaign] Los campos pueden mostrarse, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignación de información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Déclencheur](#triggers)
* [Acciones](#actions)
* [Búsquedas](#searches)

### Déclencheur

#### [!UICONTROL Ver registros]

Este módulo de déclencheur programado inicia un escenario cuando cambia un registro.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Campaign], consulte <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Cree una conexión con [!DNL Adobe Campaign]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td>Seleccione si desea inspeccionar registros nuevos, registros actualizados o ambos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recurso]</td> 
   <td>Seleccione el recurso que desea inspeccionar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos que se incluirán en la salida]</td> 
   <td>Seleccione los campos que desea incluir en la salida del módulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos personalizados para incluir en la salida]</td> 
   <td>Para cada campo personalizado que desee incluir en la salida, haga clic en <b>[!UICONTROL Agregar]</b> e introduzca el nombre del campo personalizado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de resultados devueltos]</td> 
   <td>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</td> 
  </tr> 
 </tbody> 
</table>


### Acciones

* [[!UICONTROL Creación de un registro]](#create-a-record)
* [[!UICONTROL Realizar una llamada de API personalizada]](#make-a-custom-api-call)
* [[!UICONTROL Eliminación de un registro]](#delete-record)
* [[!UICONTROL Realizar una acción]](#perform-an-action)
* [[!UICONTROL Leer un registro]](#-read-a-record)
* [[!UICONTROL Suscribirse o cancelar la suscripción]](#subscribe-or-unsubscribe)
* [[!UICONTROL Actualización de un registro]](#update-record)

#### [!UICONTROL Creación de un registro]

Este módulo de acción crea un nuevo registro en [!DNL Adobe Campaign].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td>
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Campaign], consulte <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Cree una conexión con [!DNL Adobe Campaign]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recurso]</td> 
   <td>Seleccione el tipo de [!DNL Adobe Campaign] registro que desea crear.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos] </td> 
   <td>Seleccione los campos para los que desea establecer valores cuando se cree el registro y, a continuación, rellene los valores de esos campos. Los campos varían según el tipo de registro seleccionado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos personalizados]</td> 
   <td> Para cada campo personalizado que desee agregar al nuevo registro, haga clic en <b>[!UICONTROL Agregar elemento]</b> e introduzca o asigne el nombre y el valor del campo. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Realizar una llamada de API personalizada]

Este módulo realiza una llamada de API personalizada a [!DNL Adobe Campaign] API

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Campaign], consulte <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Cree una conexión con [!DNL Adobe Campaign]</a> en este artículo.</td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Acción]</td>
      <td><p>Seleccione la acción que desea que realice la llamada de API.</p>
      <p>[!UICONTROL Ejecutar consulta]</p>
      <p>[!UICONTROL Write]</p>
      <p>[!UICONTROL Obtener entidad si es más reciente]</p>
      <p>[!UICONTROL Seleccionar todo]</p>
      <p>[!UICONTROL Push event]</p>
    </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Encabezados]</td>
      <td>
        <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p>
        <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] agrega automáticamente el encabezado de token de [!UICONTROL x-security].</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Cuerpo XML de [!UICONTROL]</td>
   <td> <p>Añada el contenido del cuerpo para la llamada de API en XML, sin el elemento session. </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL Eliminar registro]

Este módulo de acción elimina un único registro de [!DNL Adobe Campaign].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td>
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Campaign], consulte <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Cree una conexión con [!DNL Adobe Campaign]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recurso]</td> 
   <td>Seleccione el tipo de recurso que desea eliminar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Introduzca o asigne el ID del recurso que desea eliminar.</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL Realizar una acción]

Este módulo de acción realiza una acción seleccionada en un objeto del [!DNL Adobe Campaign] API.

Para obtener información sobre acciones y campos específicos, consulte [[!DNL Adobe Campaign] - Documentación de API](https://experienceleague.adobe.com/developer/campaign-api/api/p-14.html).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td>
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Campaign], consulte <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Cree una conexión con [!DNL Adobe Campaign]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Acción]</td> 
   <td><p>Seleccione la acción que se realizará en el objeto.</p>
   <ul>
   <li><p><b>[!DNL List]</b></p><p> Para ver los campos disponibles, consulte <a href="#search" class="MCXref xref" >[!UICONTROL Buscar]</a> en este artículo. </p></li>
     <li><p><b>[!UICONTROL Get]</b></p><p> Para ver los campos disponibles, consulte <a href="#search" class="MCXref xref" >[!UICONTROL Buscar]</a> en este artículo. </p></li> 
   <li><p><b>[!UICONTROL Crear]</b></p><p> Para ver los campos disponibles, consulte <a href="#create-a-record" class="MCXref xref" >[!UICONTROL Crear un registro]</a> en este artículo. </p></li>
   <li><p><b>[!UICONTROL Actualización]</b></p><p> Para ver los campos disponibles, consulte <a href="#update-record" class="MCXref xref" >[!UICONTROL Actualizar un registro]</a> en este artículo. </p></li>
   <li><p><b>[!UICONTROL Eliminar]</b></p><p> Para ver los campos disponibles, consulte <a href="#delete-record" class="MCXref xref" >[!UICONTROL Eliminar un registro]</a> en este artículo. </p></li>
   </ul>
   </td>
</tr> 
 </tbody> 
</table>

#### [!UICONTROL Leer un registro]

Este módulo de acción lee un registro de [!DNL Adobe Campaign].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td>
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Campaign], consulte <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Cree una conexión con [!DNL Adobe Campaign]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recurso]</td> 
   <td>Seleccione el tipo de [!DNL Adobe Campaign] registro que desea leer.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>Introduzca del mapa el ID del registro que desea leer.</td> 
  </tr> 
 <tr> 
   <td role="rowheader">[!UICONTROL Campos que se incluirán en la salida] </td> 
   <td>Seleccione los campos que desea incluir en la salida del módulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos personalizados para incluir en la salida]</td> 
   <td>Para cada campo personalizado que desee incluir en la salida, haga clic en <b>[!UICONTROL Agregar]</b> e introduzca el nombre del campo personalizado.</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL Suscribirse o cancelar la suscripción]

Este módulo de acción suscribe o cancela la suscripción de un usuario a un servicio de información.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td>
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Campaign], consulte <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Cree una conexión con [!DNL Adobe Campaign]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Suscribirse o cancelar la suscripción]</td> 
   <td>Seleccione si desea suscribirse o darse de baja del servicio informativo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre de servicio]</td> 
   <td>Seleccione el servicio al que desea suscribirse o cancelar la suscripción.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dirección de correo electrónico del destinatario] </td> 
   <td>Introduzca o asigne la dirección de correo electrónico del usuario al que desea suscribirse o cancelar la suscripción al servicio informativo.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actualizar registro]

Este módulo de acción actualiza un único registro en [!DNL Adobe Campaign].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td>
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Campaign], consulte <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Cree una conexión con [!DNL Adobe Campaign]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recurso]</td> 
   <td>Seleccione el tipo de [!DNL Adobe Campaign] registro que desea crear.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>Introduzca del mapa el ID del registro que desea actualizar.</td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL Campos] </td> 
   <td>Seleccione los campos para los que desea actualizar los valores y rellene los valores de esos campos. Los campos varían según el tipo de registro seleccionado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos personalizados]</td> 
   <td> Para cada campo personalizado que desee actualizar, haga clic en <b>[!UICONTROL Agregar elemento]</b> e introduzca o asigne el nombre y el valor del campo. </td> 
  </tr> 
 </tbody> 
</table>

### Búsquedas

#### [!UICONTROL Búsqueda]

Este módulo de búsqueda devuelve registros basados en los criterios especificados.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td>
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Campaign], consulte <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Cree una conexión con [!DNL Adobe Campaign]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recurso]</td> 
   <td>Seleccione el tipo de [!DNL Adobe Campaign] registro que desea crear.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite] </td> 
   <td>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</td> 
  </tr> 
 </tbody> 
</table>
