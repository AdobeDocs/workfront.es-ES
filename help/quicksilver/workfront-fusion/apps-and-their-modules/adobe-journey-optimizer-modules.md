---
filename: adobe-journey-optimizer-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Módulos de Adobe Journey Optimizer
description: En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL Adobe Journey Optimizer], así como conectarlo a múltiples aplicaciones y servicios de terceros.
author: Becky
exl-id: 2c1aea46-edbf-42a3-a6e9-f8aea042a48d
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1602'
ht-degree: 0%

---

# [!DNL Adobe Journey Optimizer] Módulos

<!--
Becky: pull from main, add to TOCs, then push to merge.
-->

En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL Adobe Journey Optimizer], así como conectarlo a múltiples aplicaciones y servicios de terceros. [!DNL Adobe Journey Optimizer] Los módulos de le permiten crear, leer, actualizar o eliminar registros, o realizar una llamada de API personalizada a [!DNL Adobe Journey Optimizer] API.


Si necesita instrucciones sobre cómo crear un escenario, consulte [Creación de un escenario](../../workfront-fusion/scenarios/create-a-scenario.md).

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
        <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p>
      </td>
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

Antes de usar el [!DNL Adobe Journey Optimizer] Conector de, debe asegurarse de que se cumplen los siguientes requisitos previos:

* Debe tener un activo [!DNL Adobe Journey Optimizer] cuenta.

## Cree una conexión con [!DNL Adobe Journey Optimizer]

Para crear una conexión para su [!DNL Adobe Journey Optimizer] módulos:

1. En cualquier [!DNL Adobe Journey Optimizer] , haga clic en **[!UICONTROL Añadir]** situado junto al cuadro Conexión.

1. Rellene los campos siguientes:

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[!UICONTROL Nombre de conexión]</td>
          <td>
            <p>Escriba un nombre para esta conexión.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL ID de cliente]</td>
          <td>Introduzca su [!DNL Adobe] [!UICONTROL ID de cliente]. Esto se puede encontrar en la sección [!UICONTROL Credentials details] del [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Secreto de cliente]</td>
          <td>Introduzca su [!DNL Adobe] [!UICONTROL Secreto de cliente]. Esto se puede encontrar en la sección [!UICONTROL Credentials details] del [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL ID de cuenta técnica]</td>
          <td>Introduzca su [!DNL Adobe] [!UICONTROL ID de cuenta técnica]. Esto se puede encontrar en la sección [!UICONTROL Credentials details] del [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL ID de organización]</td>
          <td>Introduzca su [!DNL Adobe] [!UICONTROL ID de organización]. Esto se puede encontrar en la sección [!UICONTROL Credentials details] del [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Meta ámbitos]</td>
          <td>
            Escriba los metaámbitos necesarios para la conexión.
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Clave privada]</td>
          <td>
            <p>Introduzca la clave privada que se generó cuando se crearon las credenciales en la [!DNL Adobe Developer Console]. </p>
            <p>Para extraer la clave privada o el certificado:</p>
            <ol>
              <li value="1">
                <p>Clic <b>[!UICONTROL Extraer]</b>.</p>
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
                <p>Clic <b>[!UICONTROL Guardar]</b> para extraer el archivo y volver a la configuración de conexión.</p>
              </li>
            </ol>
          </td>
        </tr>
      </tbody>
    </table>
1. Clic **[!UICONTROL Continuar]** para guardar la conexión y volver al módulo.

## [!DNL Adobe Journey Optimizer] módulos y sus campos

Al configurar [!DNL Adobe Journey Optimizer] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, se añaden [!DNL Adobe Journey Optimizer] Los campos pueden mostrarse, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignación de información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Acciones](#actions)
* [Búsquedas](#searches)

### Acciones

* [[!UICONTROL Creación de un registro]](#create-a-record)
* [[!UICONTROL Realizar una llamada de API personalizada]](#make-a-custom-api-call)
* [[!UICONTROL Eliminación de un registro]](#delete-a-record)
* [[!UICONTROL Actualización de un registro]](#update-a-record)

#### [!UICONTROL Creación de un registro]

Este módulo de acción crea una ubicación, una regla de decisión, una etiqueta, una oferta personalizada, una colección o una oferta de reserva.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
     <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Journey Optimizer], consulte <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Cree una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Tipo de registro]
      </td>
      <td>
        Seleccione el tipo de registro que desea crear
        <ul>
        <li><b>[!UICONTROL Posición]</b>: continuar a <a href="#placement-fields" >Campos de [!UICONTROL Placement]</a>.</li>
        <li><b>[!UICONTROL Regla de decisión]</b>: continuar a <a href="#decision-rule-fields" >Campos de [!UICONTROL Regla de decisión]</a>.</li>
        <li><b>[!UICONTROL Decisión]</b>: continuar a <a href="#decision-fields" >Campos de [!UICONTROL Decision]</a>.</li>
        <li><b>[!UICONTROL Etiqueta]</b>: continuar a <a href="#tag-fields" >Campos de [!UICONTROL Tag]</a>.</li>
        <li><b>[!UICONTROL Colección]</b>: continuar a <a href="#collection-fields" >Campos de [!UICONTROL Collection]</a>.</li>
        <li><b>Oferta de reserva de [!UICONTROL]</b>: continuar a <a href="#fallback-offer-fields" >Campos de [!UICONTROL Oferta de reserva]</a>.</li>
        <li><b>[!UICONTROL Oferta personalizada]</b>: continuar a <a href="#personalized-offer-fields" >Campos de [!UICONTROL Oferta personalizada]</a>.</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Ubicación] campos

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Nombre]</td>
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
      <td role="rowheader">[!UICONTROL Nombre]</td>
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
        [!UICONTROL Condición]
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
      <td role="rowheader">[!UICONTROL Nombre]</td>
     <td>Introduzca o asigne un nombre para la regla de descripción.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Estado]</td>
      <td>Seleccione el estado de la decisión.
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Fecha de inicio]</td>
      <td><p>Introduzca o asigne la fecha de inicio de la decisión.</p><p>Para obtener una lista de los formatos de fecha admitidos, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipos en [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Fecha de finalización]</td>
      <td><p>Introduzca o asigne la fecha de finalización de la decisión.</p><p>Para obtener una lista de los formatos de fecha admitidos, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipos en [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Ubicaciones]</td>
      <td>Seleccione las ubicaciones que desea agregar a esta decisión
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Colección]</td>
      <td>Seleccione la colección de ofertas que contiene las ofertas que esta decisión tendrá en cuenta.
      </td>
    </tr>
   <tr>
      <td role="rowheader">Oferta de reserva de [!UICONTROL]</td>
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
      <td role="rowheader">[!UICONTROL Nombre]</td>
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
      <td role="rowheader">[!UICONTROL Nombre]</td>
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
        [!UICONTROL Elementos]
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
      <td role="rowheader">[!UICONTROL Nombre]</td>
     <td>Introduzca o asigne un nombre para la oferta de reserva.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Estado]
      </td>
      <td> Seleccione el estado de la oferta de reserva.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Posición]
      </td>
      <td>Introduzca o asigne la ubicación de la oferta de reserva.
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
      <td role="rowheader">[!UICONTROL Nombre]</td>
     <td>Introduzca o asigne un nombre para la regla de descripción.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Estado]</td>
      <td>Seleccione el estado de la decisión.
      </td>
    </tr>
    <tr>
      <td role="rowheader">Ubicación</td>
      <td>Seleccione la ubicación de la oferta personalizada.
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Fecha de inicio]</td>
      <td><p>Introduzca o asigne la fecha de inicio de la oferta personalizada.</p><p>Para obtener una lista de los formatos de fecha admitidos, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipos en [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Fecha de finalización]</td>
      <td><p>Introduzca o asigne la fecha de finalización de la oferta personalizada.</p><p>Para obtener una lista de los formatos de fecha admitidos, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipos en [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Reglas de decisión]</td>
      <td>Seleccione las reglas de decisión para añadir a esta oferta personalizada.
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Prioridad]</td>
      <td>Seleccione la prioridad de esta oferta. La prioridad afecta a si esta oferta se presentará en lugar de otra oferta.
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Restricción de límite]</td>
      <td>Introduzca o asigne el número de veces que se presentará esta oferta.
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Eliminación de un registro]

Este módulo de acción elimina un único registro de [!DNL Adobe Journey Optimizer].

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
     <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Journey Optimizer], consulte <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Cree una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Tipo de registro]
      </td>
      <td>
        Seleccione el tipo de registro que desea eliminar
        <ul>
        <li>[!UICONTROL Posición]</li>
        <li>[!UICONTROL Regla de decisión]</li>
        <li>[!UICONTROL Decisión]</li>
        <li>[!UICONTROL Etiqueta]</li>
        <li>[!UICONTROL Colección]</li>
        <li>Oferta de reserva de [!UICONTROL]</li>
        <li>[!UICONTROL Oferta personalizada]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Posición]/[!UICONTROL Regla de decisión]/[!UICONTROL Decisión]/[!UICONTROL Etiqueta]/[!UICONTROL Colección]/[!UICONTROL Oferta de reserva]/[!UICONTROL Oferta personalizada]
      </td>
      <td>
        Seleccione el registro que desea eliminar.
      </td>
    </tr>

</tbody>
</table>

#### [!UICONTROL Realizar una llamada de API personalizada]

Este módulo realiza una llamada de API personalizada a [!DNL Adobe Journey Optimizer] API

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Conexión]</td>
     <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Journey Optimizer], consulte <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Cree una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Ruta]</p>
      </td>
      <td>
        <p>Introduzca una ruta relativa a {baseURL} comenzando por<code>/</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Método]</p>
      </td>
      <td>
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada de API. Para obtener más información, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Encabezados]</td>
      <td>
        <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p>
        <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion añade automáticamente encabezados de autorización y encabezados x-api-key.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Cadena de consulta]  </td>
      <td>
        <p>Introduzca la cadena de consulta de solicitud.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Cuerpo]</td>
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Cuando se utilizan afirmaciones condicionales como <code>if</code> en su JSON, ponga las comillas fuera del enunciado condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Límite]  </td>
      <td>
        <p>Introduzca el número máximo de resultados que desea que devuelva el módulo en un ciclo de ejecución.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Eliminar un registro]

Este módulo de acción elimina un único registro de [!DNL Adobe Journey Optimizer].

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Conexión]</td>
     <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Journey Optimizer], consulte <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Cree una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Tipo de registro]
      </td>
      <td>
        Seleccione el tipo de registro que desea eliminar
        <ul>
        <li>[!UICONTROL Posición]</li>
        <li>[!UICONTROL Regla de decisión]</li>
        <li>[!UICONTROL Decisión]</li>
        <li>[!UICONTROL Etiqueta]</li>
        <li>[!UICONTROL Colección]</li>
        <li>Oferta de reserva de [!UICONTROL]</li>
        <li>[!UICONTROL Oferta personalizada]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Posición]/[!UICONTROL Regla de decisión]/[!UICONTROL Decisión]/[!UICONTROL Etiqueta]/[!UICONTROL Colección]/[!UICONTROL Oferta de reserva]/[!UICONTROL Oferta personalizada]
      </td>
      <td>
        Seleccione el registro que desea eliminar.
      </td>
    </tr>

</tbody>
</table>

#### [!UICONTROL Actualización de un registro]

Este módulo de acción crea una ubicación, decisión, regla de decisión, etiqueta, oferta personalizada, colección u oferta de reserva.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Conexión]</td>
     <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Journey Optimizer], consulte <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Cree una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Tipo de registro]
      </td>
      <td>
        Seleccione el tipo de registro que desea actualizar
        <ul>
        <li>[!UICONTROL Posición]</li>
        <li>[!UICONTROL Regla de decisión]</li>
        <li>[!UICONTROL Decisión]</li>
        <li>[!UICONTROL Etiqueta]</li>
        <li>[!UICONTROL Colección]</li>
        <li>Oferta de reserva de [!UICONTROL]</li>
        <li>[!UICONTROL Oferta personalizada]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Posición]/[!UICONTROL Regla de decisión]/[!UICONTROL Decisión]/[!UICONTROL Etiqueta]/[!UICONTROL Colección]/[!UICONTROL Oferta de reserva]/[!UICONTROL Oferta personalizada]
      </td>
      <td>
        Seleccione el registro que desea actualizar.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Campos]
      </td>
      <td>Para cada campo que desee actualizar:
      <ol>
      <li>Clic <b>[!UICONTROL Agregar]</b>.</li>
      <li>Seleccione si desea agregar, reemplazar o quitar valores.</li>
      <li>Introduzca el campo que desea actualizar.</li>
      <li>Introduzca el nuevo valor para el campo.</li>
      </td>
    </tr>

</tbody>
</table>


### Búsquedas

#### [!UICONTROL Enumeración de registros]

Este módulo de búsqueda enumera los registros del tipo seleccionado y devuelve los resultados según los criterios especificados.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Conexión]</td>
     <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Journey Optimizer], consulte <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Cree una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Tipo de registro]</p>
      </td>
      <td>
        <p>Seleccione el tipo de registro que desea enumerar.</p>
        <ul>
        <li>[!UICONTROL Posición]</li>
        <li>[!UICONTROL Regla de decisión]</li>
        <li>[!UICONTROL Decisión]</li>
        <li>[!UICONTROL Etiqueta]</li>
        <li>[!UICONTROL Colección]</li>
        <li>Oferta de reserva de [!UICONTROL]</li>
        <li>[!UICONTROL Oferta personalizada]</li>
       </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Operador de consulta]</p>
      </td>
      <td>
        <p>Seleccione un operador para aplicarlo a los parámetros de la consulta</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Campos]</td>
      <td><p>Si desea limitar la búsqueda a campos específicos, introduzca los campos. Para cada campo al que desee limitar la búsqueda, haga clic en [!UICONTROL Agregar elemento] e introduzca el nombre del campo.</p><p>Las expresiones de ruta tienen la forma de rutas separadas por puntos, como <code>_instance.xdm:name</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ordenar por] </td>
      <td>Introduzca o asigne la propiedad según la cual desea ordenar los resultados.
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dirección del pedido]</td>
   <td>Seleccione si desea ordenar los resultados en dirección ascendente o descendente.
    </td>
     </tr>
  </tbody>
</table>
