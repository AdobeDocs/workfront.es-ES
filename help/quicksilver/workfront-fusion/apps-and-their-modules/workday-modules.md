---
filename: workday-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de Workday
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 535573e0-b6ad-43a2-b7cb-ed32d1dc8d16
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1080'
ht-degree: 55%

---

# Módulos de [!DNL Workday]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Módulos Workday](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/workday-modules.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

En un escenario de [!DNL Adobe Workfront Fusion], puede automatizar los flujos de trabajo que utilizan [!DNL Workday], así como conectarlo a varias aplicaciones y servicios de terceros.

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

Para usar los módulos [!DNL Workday], debe:

* Tener una cuenta de [!DNL Workday].

* Crear una aplicación OAuth en [!DNL Workday]. Para obtener instrucciones, consulte la documentación de [!DNL Workday].

## Información de API de Workday

El conector de Workday utiliza lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL básica</td> 
   <td>https://{{connection.servicesUrl}}/api</td> 
  </tr>
  <tr> 
   <td role="rowheader">Etiqueta de API</td> 
   <td>Versión 1.6.4</td> 
  </tr>
 </tbody> 
 </table>

## Conectar [!DNL Workday] a [!DNL Workfront Fusion]

1. En cualquier módulo de [!DNL Workfront Fusion], haga clic en [!UICONTROL Añadir] junto al campo [!UICONTROL Conexión]

2. Rellene los campos siguientes:

   <table style="table-layout:auto"> 
        <col/>
        <col/>
        <tbody>
            <tr>
                <td role="rowheader">
                    <p role="rowheader">[!UICONTROL Connection name]</p>
                </td>
                <td>Introduzca un nombre para la conexión</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Workday host]</td>
                <td>Escriba la dirección de su host [!DNL Workday] sin <code>https://</code>. Por ejemplo, <code>mycompany.workday.com</code></td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL URL de servicios]</td>
                <td>Escriba la dirección de los servicios web de [!DNL Workday] sin <code>https://</code>. Por ejemplo, <code>mycompany-services.workday.com</code></td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Nombre de inquilino]</td>
                <td>Escriba el inquilino de esta cuenta de [!DNL Workday]. El inquilino es el identificador de su organización y se puede ver en la dirección URL que utiliza para iniciar sesión en Workday. Ejemplo: en la dirección <code>https://www.myworkday.com/mycompany</code>, el usuario es <code>mycompany</code>.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Client ID]</td>
                <td>Escriba el Id. de cliente para la aplicación [!DNL Workday] que utiliza esta conexión. Esto se obtiene al crear la aplicación en [!DNL Workday].</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Client Secret]</td>
                <td>Escriba el Secreto de cliente para la aplicación [!DNL Workday] que utiliza esta conexión. Esto se obtiene al crear la aplicación en [!DNL Workday].</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Tiempo de espera de sesión (min)]</td>
                <td >Introduzca el número de minutos tras los cuales caduca el token de autorización.</td>
            </tr>
        </tbody>
    </table>


3. Haga clic en [!UICONTROL Continuar] para guardar la conexión y volver al módulo

## Módulos de [!DNL Workday] y sus campos

Al configurar módulos de [!DNL Workday], [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL Workday] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. El título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Acción](#action)

* [Buscar](#search)


### Acción

* [[!UICONTROL Create a record]](#create-a-record)

* [[!UICONTROL Eliminar un registro]](#delete-a-record)

* [[!UICONTROL Realizar una llamada de API personalizada]](#make-a-custom-api-call)

* [[!UICONTROL Actualizar un registro]](#update-a-record)


#### [!UICONTROL Crear un registro]

Este módulo de acción crea un único registro en [!DNL Workday].

<table style="table-layout:auto"> 
    <col/>
    <col/>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Connection]</td>
            <td>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL Workday] a Workfront Fusion, consulte <a href="#Connect" class="MCXref xre[!DNL ]f" >Conectar [!DNL Workday] a [!DNL Workfront Fusion]</a>.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Record Type]</td>
            <td>Seleccione el tipo de registro que desea crear.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td>Introduzca o asigne el ID del registro que desea crear.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL Id. de subrecurso]</td>
            <td >Introduzca o asigne el ID del subrecurso que desea crear.</td>
        </tr>
    </tbody>
</table>

#### [!UICONTROL Eliminar un registro]

Este módulo de acción elimina un único registro de [!DNL Workday].

<table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Connection]</td>
            <td>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Workday] a [!DNL Workfront Fusion], vea <a href="#Connect" class="MCXref xre[!DNL ]f" >Conectar [!DNL Workday] a [!DNL Workfront Fusion]</a>.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Record type]</td>
            <td>Seleccione el tipo de registro que desea eliminar.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL Tipo de registro específico]</td>
            <td>Seleccione el tipo de registro específico que desea eliminar. Se basan en el tipo de registro elegido.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Id. de subrecurso]</td>
            <td>Introduzca o asigne el ID del subrecurso que desea eliminar.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td >Introduzca o asigne el ID del registro que desea eliminar.</td>
        </tr>
    </tbody>
</table>


### [!UICONTROL Realizar una llamada de API personalizada]

Este módulo de acción le permite realizar una llamada autenticada personalizada a la API [!DNL Workday]. De este modo, puede crear una automatización del flujo de datos imposibles de realizar por los otros [!DNL Workday] módulos.

Al configurar este módulo, se muestran los campos siguientes.

El módulo devuelve el código de estado, junto con los encabezados y el cuerpo de la llamada de API.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Connection]</p> </td> 
            <td>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Workday] a [!DNL Workfront Fusion], vea <a href="#Connect" class="MCXref xre[!DNL ]f" >Conectar [!DNL Workday] a [!DNL Workfront Fusion]</a>.</td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Escriba una ruta relativa a <code style="color: #ff1493;">https://&lt;tenantHostname>/api/&lt;serviceName>/&lt;version>/&lt;tenant></code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Seleccione el método de petición HTTP que necesita para configurar la llamada de la API. Para obtener más información, vea <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de petición HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p> <p>Por ejemplo: <code>{"Content-type":"application/json"}</code></p> <p>[!UICONTROL Workfront Fusion] añade los encabezados de autorización automáticamente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Añada la consulta para la llamada de API en forma de objeto JSON estándar.</p> <p>Por ejemplo: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Cuando utilice afirmaciones condicionales como <code>if</code> en su JSON, coloque las comillas fuera de la afirmación condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actualizar un registro]

Este módulo de acción actualiza un único registro en [!DNL Workday].

<table style="table-layout:auto"> 
    <col/>
    <col/>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Connection]</td>
            <td>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL Workday] a Workfront Fusion, consulte <a href="#Connect" class="MCXref xref" >[!UICONTROL Connect [!DNL Workday] to Workfront Fusion]</a></td>
        </tr>
        <tr>
            <td  role="rowheader">Tipo de registro</td>
            <td>Seleccione el tipo de registro t[!UICONTROL ] que desea actualizar.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td>Introduzca o asigne el ID del registro que desea actualizar.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL Id. de subrecurso]</td>
            <td >Introduzca o asigne el ID del subrecurso que desea actualizar.</td>
        </tr>
    </tbody>
</table>

### Buscar

* [[!UICONTROL Leer un registro]](#read-a-record)

* [[!UICONTROL List records]](#list-records)


#### [!UICONTROL Leer un registro]

Este módulo de acción lee un solo registro.

<table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Connection]</td>
            <td>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL Workday] a Workfront Fusion, consulte <a href="#Connect" class="MCXref xref" >[!UICONTROL Connect [!DNL Workday] to Workfront Fusion]</a></td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Record type]</td>
            <td>Seleccione el tipo de registro que desea eliminar.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL Tipo de registro específico]</td>
            <td>Seleccione el tipo de registro específico que desea leer. Se basan en el tipo de registro elegido.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td >Introduzca o asigne el ID del registro que desea eliminar.</td>
        </tr>
    </tbody>
</table>

#### [!UICONTROL List records]

Este módulo de búsqueda recupera una lista de registros del tipo especificado.

<table style="table-layout:auto"> 
      <col/>
      <col/>
      <tbody>
          <tr>
              <td role="rowheader">[!UICONTROL Connection]</td>
              <td>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Workday] a [!DNL Workfront Fusion], vea <a href="#Connect" class="MCXref xref" >Conectar [!DNL Workday] a [!DNL Workfront Fusion]</a></td>
          </tr>
          <tr>
              <td  role="rowheader">[!UICONTROL Record Type]</td>
              <td>Seleccione el tipo de registro que desea recuperar.</td>
          </tr>
          <tr>
              <td role="rowheader">[!UICONTROL Limit]</td>
              <td >
                  <p>Introduzca o asigne el número máximo de registros que desea que el módulo recupere durante cada ciclo de ejecución de escenario.</p>
              </td>
          </tr>
      </tbody>
  </table>
