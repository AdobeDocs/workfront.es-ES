---
filename: workday-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de Workday
description: En un escenario de Adobe Workfront Fusion, puede automatizar los flujos de trabajo que utilizan [!DNL Workday], así como conectarlo a múltiples aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion
exl-id: 535573e0-b6ad-43a2-b7cb-ed32d1dc8d16
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '1013'
ht-degree: 2%

---

# [!DNL Workday] módulos

En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL Workday], así como conectarlo a múltiples aplicaciones y servicios de terceros.

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

Para usar la variable [!DNL Workday] módulos, debe:

* Tener un [!DNL Workday] cuenta.

* Creación de una aplicación de OAuth en [!DNL Workday]. Para obtener instrucciones, consulte la [!DNL Workday] documentación.

## Connect [!DNL Workday] hasta [!DNL Workfront Fusion]

1. En cualquier [!DNL Workfront Fusion] , haga clic en [!UICONTROL Añadir] junto al [!UICONTROL Conexión] campo

2. Rellene los campos siguientes:

   <table style="table-layout:auto"> 
        <col/>
        <col/>
        <tbody>
            <tr>
                <td role="rowheader">
                    <p role="rowheader">[!UICONTROL Nombre de conexión]</p>
                </td>
                <td>Escriba un nombre para la conexión</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Workday host]</td>
                <td>Introduzca la dirección de su [!DNL Workday] host sin <code>https://</code>. Por ejemplo: <code>mycompany.workday.com</code>.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL URL de servicios]</td>
                <td>Introduzca la dirección de su [!DNL Workday] servicios web sin <code>https://</code>. Por ejemplo: <code>mycompany-services.workday.com</code>.</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Nombre de inquilino]</td>
                <td>Introduzca el inquilino para esto [!DNL Workday] cuenta. El inquilino es el identificador de su organización y se puede ver en la dirección URL que utiliza para iniciar sesión en Workday. Ejemplo: en la dirección <code>https://www.myworkday.com/mycompany</code>, el inquilino es <code>mycompany</code>.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL ID de cliente]</td>
                <td>Introduzca el ID de cliente para [!DNL Workday] aplicación que utiliza esta conexión. Esto se obtiene al crear la aplicación en [!DNL Workday].</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Secreto de cliente]</td>
                <td>Escriba el Secreto del cliente para [!DNL Workday] aplicación que utiliza esta conexión. Esto se obtiene al crear la aplicación en [!DNL Workday].</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Tiempo de espera de sesión (min)]</td>
                <td >Introduzca el número de minutos tras los cuales caduca el token de autorización.</td>
            </tr>
        </tbody>
    </table>


3. Clic [!UICONTROL Continuar] para guardar la conexión y volver al módulo

## [!DNL Workday] módulos y sus campos

Al configurar [!DNL Workday] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, se añaden [!DNL Workday] Los campos pueden mostrarse, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignación de información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Acción](#action)

* [Buscar](#search)


### Acción

* [[!UICONTROL Creación de un registro]](#create-a-record)

* [[!UICONTROL Eliminación de un registro]](#delete-a-record)

* [[!UICONTROL Realizar una llamada de API personalizada]](#make-a-custom-api-call)

* [[!UICONTROL Actualización de un registro]](#update-a-record)


#### [!UICONTROL Creación de un registro]

Este módulo de acción crea un único registro en [!DNL Workday].

<table style="table-layout:auto"> 
    <col/>
    <col/>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Conexión]</td>
            <td>Para obtener instrucciones acerca de cómo conectar su [!DNL Workday] cuenta de Workfront Fusion, consulte <a href="#Connect" class="MCXref xre[!DNL ]f" >Connect [!DNL Workday] hasta [!DNL Workfront Fusion]</a>.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Tipo de registro]</td>
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

#### [!UICONTROL Eliminación de un registro]

Este módulo de acción elimina un único registro de [!DNL Workday].

<table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Conexión]</td>
            <td>Para obtener instrucciones acerca de cómo conectar su [!DNL Workday] cuenta a [!DNL Workfront Fusion], consulte <a href="#Connect" class="MCXref xre[!DNL ]f" >Connect [!DNL Workday] hasta [!DNL Workfront Fusion]</a>.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Tipo de registro]</td>
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

Este módulo de acción le permite realizar una llamada autenticada personalizada a [!DNL Workday] API. De este modo, se puede crear una automatización del flujo de datos que el otro no puede realizar [!DNL Workday] módulos.

Al configurar este módulo, se muestran los campos siguientes.

El módulo devuelve el código de estado a, junto con los encabezados y el cuerpo de la llamada de API.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Connection]</p> </td> 
            <td>Para obtener instrucciones acerca de cómo conectar su [!DNL Workday] cuenta a [!DNL Workfront Fusion], consulte <a href="#Connect" class="MCXref xre[!DNL ]f" >Connect [!DNL Workday] hasta [!DNL Workfront Fusion]</a>.</td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Introduzca una ruta relativa a <code style="color: #ff1493;">https://&lt;tenantHostname>/api/&lt;serviceName>/&lt;version>/&lt;tenant></code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada de API. Para obtener más información, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p> <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p> <p>[!UICONTROL Workfront Fusion] agrega los encabezados de autorización automáticamente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadena de consulta]</td> 
   <td> <p>Añada la consulta para la llamada de API en forma de objeto JSON estándar.</p> <p>Por ejemplo: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cuerpo]</td> 
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Cuando se utilizan afirmaciones condicionales como <code>if</code> en su JSON, ponga las comillas fuera del enunciado condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actualización de un registro]

Este módulo de acción actualiza un único registro en [!DNL Workday].

<table style="table-layout:auto"> 
    <col/>
    <col/>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Conexión]</td>
            <td>Para obtener instrucciones acerca de cómo conectar su [!DNL Workday] cuenta de Workfront Fusion, consulte <a href="#Connect" class="MCXref xref" >[!UICONTROL Connect [!DNL Workday] a Workfront Fusion]</a></td>
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

* [[!UICONTROL Enumeración de registros]](#list-records)


#### [!UICONTROL Leer un registro]

Este módulo de acción lee un solo registro.

<table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Conexión]</td>
            <td>Para obtener instrucciones acerca de cómo conectar su [!DNL Workday] cuenta de Workfront Fusion, consulte <a href="#Connect" class="MCXref xref" >[!UICONTROL Connect [!DNL Workday] a Workfront Fusion]</a></td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Tipo de registro]</td>
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

#### [!UICONTROL Enumeración de registros]

Este módulo de búsqueda recupera una lista de registros del tipo especificado.

<table style="table-layout:auto"> 
      <col/>
      <col/>
      <tbody>
          <tr>
              <td role="rowheader">[!UICONTROL Conexión]</td>
              <td>Para obtener instrucciones acerca de cómo conectar su [!DNL Workday] cuenta a [!DNL Workfront Fusion], consulte <a href="#Connect" class="MCXref xref" >Connect [!DNL Workday] hasta [!DNL Workfront Fusion]</a></td>
          </tr>
          <tr>
              <td  role="rowheader">[!UICONTROL Tipo de registro]</td>
              <td>Seleccione el tipo de registro que desea recuperar.</td>
          </tr>
          <tr>
              <td role="rowheader">[!UICONTROL Límite]</td>
              <td >
                  <p>Introduzca o asigne el número máximo de registros que desea que el módulo recupere durante cada ciclo de ejecución de escenario.</p>
              </td>
          </tr>
      </tbody>
  </table>
