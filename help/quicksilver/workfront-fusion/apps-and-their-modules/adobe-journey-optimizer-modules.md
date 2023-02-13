---
filename: adobe-journey-optimizer-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Módulos de Adobe Journey Optimizer
description: En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL Adobe Journey Optimizer], así como conectarlo a varias aplicaciones y servicios de terceros.
author: Becky
exl-id: 2c1aea46-edbf-42a3-a6e9-f8aea042a48d
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1554'
ht-degree: 0%

---

# [!DNL Adobe Journey Optimizer] Módulos

<!--
Becky: pull from main, add to TOCs, then push to merge.
-->

En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL Adobe Journey Optimizer], así como conectarlo a varias aplicaciones y servicios de terceros. [!DNL Adobe Journey Optimizer] los módulos le permiten crear, leer, actualizar o eliminar registros, o realizar una llamada API personalizada al [!DNL Adobe Journey Optimizer] API.


Si necesita instrucciones para crear un escenario, consulte [Crear un escenario](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obtener información sobre los módulos, consulte [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
      <td>
        <p>[!UICONTROL Pro] o superior</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] licencia*</td>
      <td>
        <p>[!UICONTROL Plan], [!UICONTROL Work]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td>
      <td >
        <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Product</td>
      <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td>
    </tr>
  </tbody>
</table>


Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Requisitos previos

Antes de usar la variable [!DNL Adobe Journey Optimizer] , debe asegurarse de que se cumplen los siguientes requisitos previos:

* Debe tener un [!DNL Adobe Journey Optimizer] cuenta.

## Crear una conexión con [!DNL Adobe Journey Optimizer]

Para crear una conexión para su [!DNL Adobe Journey Optimizer] módulos:

1. En cualquier [!DNL Adobe Journey Optimizer] módulo, haga clic en **[!UICONTROL Agregar]** junto al cuadro Conexión.

1. Complete los campos siguientes:

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[!UICONTROL Connection name]</td>
          <td>
            <p>Introduzca un nombre para esta conexión.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client ID]</td>
          <td>Escriba la [!DNL Adobe] [!UICONTROL Client ID]. Esto se puede encontrar en la sección [!UICONTROL Credentials details] de [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client Secret]</td>
          <td>Escriba la [!DNL Adobe] [!UICONTROL Client Secret]. Esto se puede encontrar en la sección [!UICONTROL Credentials details] de [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL ID de cuenta técnica]</td>
          <td>Escriba la [!DNL Adobe] [!UICONTROL ID de cuenta técnica]. Esto se puede encontrar en la sección [!UICONTROL Credentials details] de [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL ID de organización]</td>
          <td>Escriba la [!DNL Adobe] [!UICONTROL ID de organización]. Esto se puede encontrar en la sección [!UICONTROL Credentials details] de [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Meta scopes]</td>
          <td>
            Introduzca los metaámbitos necesarios para la conexión.
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Clave privada]</td>
          <td>
            <p>Introduzca la clave privada que se generó cuando se crearon sus credenciales en el [!DNL Adobe Developer Console]. </p>
            <p>Para extraer la clave privada o el certificado:</p>
            <ol>
              <li value="1">
                <p>Haga clic en <b>[!UICONTROL Extract]</b>.</p>
              </li>
              <li value="2">
                <p>Seleccione el tipo de archivo que está extrayendo.</p>
              </li>
              <li value="3">
                <p>Seleccione el archivo que contiene la clave privada o el certificado.</p>
              </li>
              <li value="4">
                <p>Introduzca la contraseña del archivo.</p>
              </li>
              <li value="5">
                <p>Haga clic en <b>[!UICONTROL Guardar]</b> para extraer el archivo y volver a la configuración de conexión.</p>
              </li>
            </ol>
          </td>
        </tr>
      </tbody>
    </table>
1. Haga clic en **[!UICONTROL Continuar]** para guardar la conexión y volver al módulo.

## [!DNL Adobe Journey Optimizer] módulos y sus campos

Al configurar [!DNL Adobe Journey Optimizer] módulos, [!DNL Workfront Fusion] muestra los campos que se enumeran a continuación. Además de estos, se incluyen [!DNL Adobe Journey Optimizer] pueden mostrarse los campos, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón de asignación encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Acciones](#actions)
* [Búsquedas](#searches)

### Acciones

* [[!UICONTROL Crear un registro]](#create-a-record)
* [[!UICONTROL Realizar una llamada API personalizada]](#make-a-custom-api-call)
* [[!UICONTROL Eliminar un registro]](#delete-a-record)
* [[!UICONTROL Actualizar un registro]](#update-a-record)

#### [!UICONTROL Crear un registro]

Este módulo de acción crea una oferta de colocación, regla de decisión, etiqueta, oferta personalizada, recopilación o reserva.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Para obtener instrucciones sobre la creación de una conexión con [!DNL Adobe Journey Optimizer], consulte <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Crear una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Tipo de registro]
      </td>
      <td>
        Seleccione el tipo de registro que desea crear
        <ul>
        <li><b>[!UICONTROL Placement]</b>: Continúe con <a href="#placement-fields" >Campos [!UICONTROL Placement]</a>.</li>
        <li><b>[!UICONTROL Regla de decisión]</b>: Continúe con <a href="#decision-rule-fields" >Campos [!UICONTROL Regla de decisión]</a>.</li>
        <li><b>[!UICONTROL Decisión]</b>: Continúe con <a href="#decision-fields" >Campos [!UICONTROL Decisión]</a>.</li>
        <li><b>[!UICONTROL Etiqueta]</b>: Continúe con <a href="#tag-fields" >Campos [!UICONTROL Tag]</a>.</li>
        <li><b>[!UICONTROL Collection]</b>: Continúe con <a href="#collection-fields" >Campos [!UICONTROL Collection]</a>.</li>
        <li><b>[!UICONTROL Oferta de reserva]</b>: Continúe con <a href="#fallback-offer-fields" >Campos [!UICONTROL Fallback offer]</a>.</li>
        <li><b>[!UICONTROL Oferta personalizada]</b>: Continúe con <a href="#personalized-offer-fields" >Campos [!UICONTROL Oferta personalizada]</a>.</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Colocación] campos

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Introduzca o asigne un nombre para la ubicación.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Descripción]
      </td>
      <td>Introduzca o asigne una descripción para la ubicación.
      </td>
    </tr>
  </tbody>
</table>


##### [!UICONTROL Regla de decisión] campos

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Introduzca o asigne un nombre para la regla de descripción.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Descripción]
      </td>
      <td>Introduzca o asigne una descripción para la regla de decisión.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Condition]
      </td>
      <td>Introduzca o asigne la condición a la regla de decisión.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Decisión] campos

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Introduzca o asigne un nombre para la regla de descripción.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Status]</td>
      <td>Seleccione el estado de la decisión.
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Fecha de inicio]</td>
      <td><p>Introduzca o asigne la fecha de inicio para la decisión.</p><p>Para obtener una lista de los formatos de fecha admitidos, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipo en [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Fecha de finalización]</td>
      <td><p>Introduzca o asigne la fecha de finalización de la decisión.</p><p>Para obtener una lista de los formatos de fecha admitidos, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipo en [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Ubicaciones]</td>
      <td>Seleccione las ubicaciones que desee agregar a esta decisión
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Collection]</td>
      <td>Seleccione la colección de ofertas que contiene las ofertas que esta decisión tendrá en cuenta.
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Oferta de reserva]</td>
      <td>Seleccione la oferta de reserva que se presentará a los clientes que no coincidan con las reglas para esta decisión.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Etiqueta] campos

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Introduzca o asigne un nombre para la etiqueta.</td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Colección] campos

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Introduzca o asigne un nombre para la colección.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Tipo de filtro]
      </td>
      <td>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Elements]
      </td>
      <td>Seleccione las etiquetas que desea incluir en la colección.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Oferta de reserva] campos

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Introduzca o asigne un nombre para la oferta de reserva.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Status]
      </td>
      <td> Seleccione el estado de la oferta de reserva.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Placement]
      </td>
      <td>Introduzca o asigne la ubicación para la oferta de reserva.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Oferta personalizada] campos

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Introduzca o asigne un nombre para la regla de descripción.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Status]</td>
      <td>Seleccione el estado de la decisión.
      </td>
    </tr>
    <tr>
      <td role="rowheader">Colocación</td>
      <td>Seleccione la colocación de la oferta personalizada.
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Fecha de inicio]</td>
      <td><p>Introduzca o asigne la fecha de inicio de la oferta personalizada.</p><p>Para obtener una lista de los formatos de fecha admitidos, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipo en [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Fecha de finalización]</td>
      <td><p>Introduzca o asigne la fecha de finalización de la oferta personalizada.</p><p>Para obtener una lista de los formatos de fecha admitidos, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipo en [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Reglas de decisión]</td>
      <td>Seleccione las reglas de decisión que desee añadir a esta oferta personalizada.
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Priority]</td>
      <td>Seleccione la prioridad de esta oferta. La prioridad afecta a si se presentará esta oferta en lugar de otra oferta.
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Restricción]</td>
      <td>Introduzca o asigne el número de veces que se presentará esta oferta.
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Eliminar un registro]

Este módulo de acción elimina un registro único de [!DNL Adobe Journey Optimizer].

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Para obtener instrucciones sobre la creación de una conexión con [!DNL Adobe Journey Optimizer], consulte <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Crear una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Tipo de registro]
      </td>
      <td>
        Seleccione el tipo de registro que desea eliminar
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL Regla de decisión]</li>
        <li>[!UICONTROL Decisión]</li>
        <li>[!UICONTROL Etiqueta]</li>
        <li>[!UICONTROL Collection]</li>
        <li>[!UICONTROL Oferta de reserva]</li>
        <li>[!UICONTROL Oferta personalizada]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Placement]/[!UICONTROL decisions rule]/[!UICONTROL decisions]/[!UICONTROL Tag]/[!UICONTROL Collection]/[!UICONTROL Fallback offer]/[!UICONTROL Personalization offer]
      </td>
      <td>
        Seleccione el registro que desea eliminar.
      </td>
    </tr>

</tbody>
</table>

#### [!UICONTROL Realizar una llamada API personalizada]

Este módulo realiza una llamada API personalizada a la variable [!DNL Adobe Journey Optimizer] API

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Para obtener instrucciones sobre la creación de una conexión con [!DNL Adobe Journey Optimizer], consulte <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Crear una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Introduzca una ruta relativa a {baseURL} que comience por<code>/</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Método]</p>
      </td>
      <td>
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada a la API. Para obtener más información, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Encabezados]</td>
      <td>
        <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p>
        <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion añade automáticamente encabezados de autorización y encabezados de clave x-api.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Cadena de consulta]  </td>
      <td>
        <p>Introduzca la cadena de consulta de solicitud.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Al utilizar afirmaciones condicionales como <code>if</code> en su JSON, ponga las comillas fuera de la afirmación condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Límite]  </td>
      <td>
        <p>Introduzca el número máximo de resultados que desea que el módulo devuelva en un ciclo de ejecución.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Eliminar un registro]

Este módulo de acción elimina un registro único de [!DNL Adobe Journey Optimizer].

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Para obtener instrucciones sobre la creación de una conexión con [!DNL Adobe Journey Optimizer], consulte <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Crear una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Tipo de registro]
      </td>
      <td>
        Seleccione el tipo de registro que desea eliminar
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL Regla de decisión]</li>
        <li>[!UICONTROL Decisión]</li>
        <li>[!UICONTROL Etiqueta]</li>
        <li>[!UICONTROL Collection]</li>
        <li>[!UICONTROL Oferta de reserva]</li>
        <li>[!UICONTROL Oferta personalizada]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Placement]/[!UICONTROL decisions rule]/[!UICONTROL decisions]/[!UICONTROL Tag]/[!UICONTROL Collection]/[!UICONTROL Fallback offer]/[!UICONTROL Personalization offer]
      </td>
      <td>
        Seleccione el registro que desea eliminar.
      </td>
    </tr>

</tbody>
</table>

#### [!UICONTROL Actualizar un registro]

Este módulo de acción crea una oferta de colocación, decisión, regla de decisión, etiqueta, oferta personalizada, recopilación o reserva.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Para obtener instrucciones sobre la creación de una conexión con [!DNL Adobe Journey Optimizer], consulte <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Crear una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Tipo de registro]
      </td>
      <td>
        Seleccione el tipo de registro que desea actualizar
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL Regla de decisión]</li>
        <li>[!UICONTROL Decisión]</li>
        <li>[!UICONTROL Etiqueta]</li>
        <li>[!UICONTROL Collection]</li>
        <li>[!UICONTROL Oferta de reserva]</li>
        <li>[!UICONTROL Oferta personalizada]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Placement]/[!UICONTROL decisions rule]/[!UICONTROL decisions]/[!UICONTROL Tag]/[!UICONTROL Collection]/[!UICONTROL Fallback offer]/[!UICONTROL Personalization offer]
      </td>
      <td>
        Seleccione el registro que desea actualizar.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Fields]
      </td>
      <td>Para cada campo que desee actualizar:
      <ol>
      <li>Haga clic en <b>[!UICONTROL Agregar]</b>.</li>
      <li>Seleccione si desea agregar, reemplazar o quitar valores.</li>
      <li>Introduzca el campo que desea actualizar.</li>
      <li>Introduzca el nuevo valor para el campo.</li>
      </td>
    </tr>

</tbody>
</table>


### Búsquedas

#### [!UICONTROL Registros de lista]

Este módulo de búsqueda enumera los registros del tipo seleccionado y devuelve los resultados según los criterios especificados.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Para obtener instrucciones sobre la creación de una conexión con [!DNL Adobe Journey Optimizer], consulte <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Crear una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Tipo de registro]</p>
      </td>
      <td>
        <p>Seleccione el tipo de registro que desea enumerar.</p>
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL Regla de decisión]</li>
        <li>[!UICONTROL Decisión]</li>
        <li>[!UICONTROL Etiqueta]</li>
        <li>[!UICONTROL Collection]</li>
        <li>[!UICONTROL Oferta de reserva]</li>
        <li>[!UICONTROL Oferta personalizada]</li>
       </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Query operator]</p>
      </td>
      <td>
        <p>Seleccione un operador para aplicar a los parámetros de la consulta</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Fields]</td>
      <td><p>Si desea limitar la búsqueda a campos específicos, introduzca los campos. Para cada campo al que desee limitar la búsqueda, haga clic en [!UICONTROL Agregar elemento] e introduzca el nombre del campo.</p><p>Las expresiones de ruta adoptan la forma de rutas separadas por puntos, como <code>_instance.xdm:name</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Order by] </td>
      <td>Introduzca o asigne la propiedad por la que desea ordenar los resultados.
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dirección del pedido]</td>
   <td>Seleccione si desea ordenar los resultados en dirección ascendente o descendente.
    </td>
     </tr>
  </tbody>
</table>
