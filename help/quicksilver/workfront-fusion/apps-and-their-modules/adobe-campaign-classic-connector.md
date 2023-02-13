---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Módulos de Adobe Campaign Classic
description: Con la variable [!DNL Adobe Campaign Classic] , puede iniciar un [!DNL Adobe Workfront Fusion] escenario basado en los eventos del [!DNL Adobe Campaign Classic] cuenta, cree, lea o actualice acuerdos y otros registros, busque registros usando los criterios establecidos y cargue documentos.
author: Becky
feature: Workfront Fusion
exl-id: 84e8fa35-0c3c-46bd-8886-88c6d8d9e1d5
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1146'
ht-degree: 1%

---

# [!DNL Adobe Campaign Classic] módulos

Con la variable [!DNL Adobe Campaign Classic] , puede iniciar un [!DNL Adobe Workfront Fusion] escenario basado en los eventos del [!DNL Adobe Campaign Classic] cuenta, cree, lea o actualice registros, busque registros con los criterios establecidos y realice llamadas API personalizadas.

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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Connect [!DNL Adobe Campaign Classic] a [!DNL Adobe Workfront Fusion]

1. En cualquier [!DNL Adobe Campaign Classic] módulo, haga clic en **[!UICONTROL Agregar]** junto a la variable [!UICONTROL Conexión] campo .
1. Introduzca la dirección URL base que utiliza para conectarse a su [!DNL Adobe Campaign Classic] instancia.
1. Introduzca su nombre de usuario y contraseña.
1. Haga clic en **[!UICONTROL Continuar]** para crear la conexión y volver al módulo .

## [!DNL Adobe Campaign Classic] módulos y sus campos

Al configurar [!DNL Adobe Campaign Classic] módulos, [!DNL Workfront Fusion] muestra los campos que se enumeran a continuación. Además de estos, se incluyen [!DNL Adobe Campaign Classic] pueden mostrarse los campos, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón de asignación encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Déclencheur](#triggers)
* [Acciones](#actions)
* [Búsquedas](#searches)

### Déclencheur

#### [!UICONTROL Registros de Watch]

Este módulo de déclencheur programado inicia un escenario cuando cambia un registro.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obtener instrucciones sobre la creación de una conexión con [!DNL Adobe Campaign Classic], consulte <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >Crear una conexión con [!DNL Adobe Campaign Classic]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td>Seleccione si desea buscar registros nuevos, registros actualizados o ambos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recurso]</td> 
   <td>Seleccione el recurso que desea buscar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields para incluir en la salida]</td> 
   <td>Seleccione los campos que desea incluir en la salida del módulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos personalizados para incluir en la salida]</td> 
   <td>Para cada campo personalizado que desee incluir en la salida, haga clic en <b>[!UICONTROL Agregar]</b> e introduzca el nombre del campo personalizado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de resultados devueltos]</td> 
   <td>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</td> 
  </tr> 
 </tbody> 
</table>


### Acciones

* [[!UICONTROL Crear un registro]](#create-a-record)
* [[!UICONTROL Realizar una llamada API personalizada]](#make-a-custom-api-call)
* [[!UICONTROL Eliminar un registro]](#delete-record)
* [[!UICONTROL Realizar una acción]](#perform-an-action)
* [[!UICONTROL Leer un registro]](#-read-a-record)
* [[!UICONTROL Suscribirse o cancelar la suscripción]](#subscribe-or-unsubscribe)
* [[!UICONTROL Actualizar un registro]](#update-record)

#### [!UICONTROL Crear un registro]

Este módulo de acción crea un nuevo registro en [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Para obtener instrucciones sobre la creación de una conexión con [!DNL Adobe Campaign Classic], consulte <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >Crear una conexión con [!DNL Adobe Campaign Classic]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recurso]</td> 
   <td>Seleccione el tipo de [!DNL Adobe Campaign Classic] registro que desea crear.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields] </td> 
   <td>Seleccione los campos para los que desea establecer valores cuando se cree el registro y, a continuación, rellene los valores de esos campos. Los campos varían según el tipo de registro seleccionado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos personalizados]</td> 
   <td> Para cada campo personalizado que desee agregar al nuevo registro, haga clic en <b>[!UICONTROL Agregar elemento]</b> e introduzca o asigne el nombre y el valor del campo. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Realizar una llamada API personalizada]

Este módulo realiza una llamada API personalizada a la variable [!DNL Adobe Campaign Classic] API

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Para obtener instrucciones sobre la creación de una conexión con [!DNL Adobe Campaign Classic], consulte <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >Crear una conexión con [!DNL Adobe Campaign Classic]</a> en este artículo.</td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Action]</td>
      <td><p>Seleccione la acción que desea que realice la llamada de API.</p>
      <p>[!UICONTROL Ejecutar consulta]</p>
      <p>[!UICONTROL Escritura]</p>
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
        <p>[!DNL Workfront Fusion] agrega automáticamente el encabezado del token [!UICONTROL x-security].</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL XML Body]</td>
   <td> <p>Añada el contenido del cuerpo para la llamada de API en XML, sin el elemento de sesión. </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL Eliminar registro]

Este módulo de acción elimina un registro único de [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Para obtener instrucciones sobre la creación de una conexión con [!DNL Adobe Campaign Classic], consulte <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >Crear una conexión con [!DNL Adobe Campaign Classic]</a> en este artículo.</td> 
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

Este módulo de acción realiza una acción seleccionada en un objeto de [!DNL Adobe Campaign Classic] API.

Para obtener información sobre acciones y campos específicos, consulte [[!DNL Adobe Campaign] - Documentación de API](https://experienceleague.adobe.com/developer/campaign-api/api/p-14.html).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Para obtener instrucciones sobre la creación de una conexión con [!DNL Adobe Campaign Classic], consulte <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >Crear una conexión con [!DNL Adobe Campaign Classic]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Action]</td> 
   <td><p>Seleccione la acción que se realizará en el objeto.</p>
   <ul>
   <li><p><b>[!DNL List]</b></p><p> Para ver los campos disponibles, consulte <a href="#search" class="MCXref xref" >[!UICONTROL Buscar]</a> en este artículo. </p></li>
     <li><p><b>[!UICONTROL Get]</b></p><p> Para ver los campos disponibles, consulte <a href="#search" class="MCXref xref" >[!UICONTROL Buscar]</a> en este artículo. </p></li> 
   <li><p><b>[!UICONTROL Crear]</b></p><p> Para ver los campos disponibles, consulte <a href="#create-a-record" class="MCXref xref" >[!UICONTROL Crear un registro]</a> en este artículo. </p></li>
   <li><p><b>[!UICONTROL Update]</b></p><p> Para ver los campos disponibles, consulte <a href="#update-record" class="MCXref xref" >[!UICONTROL Actualizar un registro]</a> en este artículo. </p></li>
   <li><p><b>[!UICONTROL Eliminar]</b></p><p> Para ver los campos disponibles, consulte <a href="#delete-record" class="MCXref xref" >[!UICONTROL Eliminar un registro]</a> en este artículo. </p></li>
   </ul>
   </td>
</tr> 
 </tbody> 
</table>

#### [!UICONTROL Leer un registro]

Este módulo de acción lee un registro de [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Para obtener instrucciones sobre la creación de una conexión con [!DNL Adobe Campaign Classic], consulte <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >Crear una conexión con [!DNL Adobe Campaign Classic]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recurso]</td> 
   <td>Seleccione el tipo de [!DNL Adobe Campaign Classic] registro que desea leer.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>Introduzca la asignación del ID del registro que desea leer.</td> 
  </tr> 
 <tr> 
   <td role="rowheader">[!UICONTROL Fields para incluir en la salida] </td> 
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
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Para obtener instrucciones sobre la creación de una conexión con [!DNL Adobe Campaign Classic], consulte <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >Crear una conexión con [!DNL Adobe Campaign Classic]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Suscribirse o cancelar la suscripción]</td> 
   <td>Seleccione si desea suscribirse o darse de baja del servicio informativo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Service name]</td> 
   <td>Seleccione el servicio al que desee suscribirse o cancelar la suscripción.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dirección de correo electrónico del destinatario] </td> 
   <td>Introduzca o asigne la dirección de correo electrónico del usuario al que desea suscribirse o darse de baja del servicio informativo.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actualizar registro]

Este módulo de acción actualiza un registro único de [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Para obtener instrucciones sobre la creación de una conexión con [!DNL Adobe Campaign Classic], consulte <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >Crear una conexión con [!DNL Adobe Campaign Classic]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recurso]</td> 
   <td>Seleccione el tipo de [!DNL Adobe Campaign Classic] registro que desea crear.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>Introduzca la asignación del ID del registro que desea actualizar.</td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL Fields] </td> 
   <td>Seleccione los campos para los que desea actualizar los valores y rellene los valores de dichos campos. Los campos varían según el tipo de registro seleccionado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos personalizados]</td> 
   <td> Para cada campo personalizado que desee actualizar, haga clic en <b>[!UICONTROL Agregar elemento]</b> e introduzca o asigne el nombre y el valor del campo. </td> 
  </tr> 
 </tbody> 
</table>

### Búsquedas

#### [!UICONTROL Buscar]

Este módulo de búsqueda devuelve registros basados en los criterios especificados.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Para obtener instrucciones sobre la creación de una conexión con [!DNL Adobe Campaign Classic], consulte <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >Crear una conexión con [!DNL Adobe Campaign Classic]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recurso]</td> 
   <td>Seleccione el tipo de [!DNL Adobe Campaign Classic] registro que desea crear.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite] </td> 
   <td>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</td> 
  </tr> 
 </tbody> 
</table>
