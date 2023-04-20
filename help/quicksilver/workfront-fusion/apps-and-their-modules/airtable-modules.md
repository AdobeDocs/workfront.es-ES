---
filename: airtable-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Módulos de aire
description: Adobe Workfront Fusion requiere una licencia de Adobe Workfront Fusion además de una licencia de Adobe Workfront.
author: Becky
hidefromtoc: true
source-git-commit: 6955c979d504adb6514ae64bf5108174d7a90ce4
workflow-type: tm+mt
source-wordcount: '1863'
ht-degree: 2%

---


# Módulos de aire


Con la variable [!DNL Airtable] conector para [!DNL Adobe Workfront Fusion], puede iniciar un escenario basado en los eventos del [!DNL Airtable] cuenta, crea, carga y actualiza registros, busca registros y realiza llamadas API personalizadas a la API de tabla de reenvío.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p> </td> 
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

Debe tener una cuenta Airtable para utilizar la funcionalidad de este artículo.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see the tutorial .</p>
-->

## Conexión de la tabla de aire a Workfront Fusion {#connect-airtable-to-workfront-fusion}

<!--

1. Log in to your Airtable account.
1. Open your account overview and generate the API key.
-->
1. Abra Workfront Fusion y **Crear una conexión** del módulo deseado.
1. Introduzca un nombre para la conexión.
1. (Opcional) Haga clic en Mostrar configuración avanzada e introduzca su ID de cliente de tabla dinámica y Secreto de cliente.
1. Haga clic en el **Continuar** para crear la conexión y volver al módulo.

## Módulos de aire y sus campos

### Registros

* [Crear un registro](#create-a-record)
* [Eliminar un registro](#delete-a-record)
* [Obtener un registro](#get-a-record)
* [Registros de búsqueda](#search-records)
* [Actualizar un registro](#update-a-record)
* [Actualizar un registro](#upsert-a-record)
* [Registros de Watch](#watch-records)
* [Respuestas de Watch](#watch-responses)
* [Realizar una llamada de API](#make-an-api-call)

#### Crear un registro {#create-a-record}

Este módulo de acción crea un nuevo registro.

Especifique los datos que desee en el registro y dónde desea que se almacenen.

El módulo devuelve todos los campos estándar asociados con el registro, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Conexión </td> 
   <td> <p>Para obtener instrucciones sobre la conexión de la cuenta de la tabla aérea a Workfront Fusion, consulte <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Conexión de la tabla de aire a Workfront Fusion</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>Base </td> 
   <td> <p>Seleccione la base a la que pertenecerá el nuevo registro.</p> </td> 
  </tr> 
  <tr> 
   <td>Tabla </td> 
   <td> <p>Seleccione la tabla a la que pertenecerá el nuevo registro.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Registro</p> </td> 
   <td> <p>Introduzca los valores del nuevo registro. Los campos disponibles se basan en la tabla seleccionada.</p> <!--<p>For more information on field types, search for "Supported field types" in the Airtable documentation.</p> 
    <ul> 
     <li> <p><strong>Text</strong>: string</p> <p>A single line of text.</p> </li> 
     <li> <p><strong>Long text</strong>: string</p> <p>Multiple lines of text, which may contain "mention tokens", for example:</p><pre>&lt;airtable:mention id="menE1i9oBaGX3DseR"&gt;@Alex&lt;/airtable:mention&gt;</pre> </li> 
     <li><strong>Attachment</strong> : Add the attachment. Airtable will download the file from the provided <code>url</code> and keep its own copy of it. If the File name field is left empty, Airtable generates the name automatically.</li> 
     <li><strong>Checkbox</strong>: Select one of the options.</li> 
     <li><strong>Multiple select</strong>: Select multiple options in the checklist.</li> 
     <li><strong>Single select</strong>: Select one option from the drop-down menu.</li> 
     <li><strong>Collaborator</strong>: Enter the email that uniquely identifies a user in Airtable who this base is shared with.</li> 
     <li><strong>Date</strong>: UTC date, for example, 2019-09-05 (ISO 8601 formatted date)</li> 
     <li>Phone number:</li> 
     <li><strong>Emails</strong>: A valid email address.</li> 
     <li><strong>URL</strong>: A valid URL (for example, airtable.com or https://airtable.com/universe).</li> 
     <li><strong>Number</strong>: Enter a number.</li> 
     <li><strong>Currency</strong>: Currency value.</li> 
     <li><strong>Percent</strong>: A percentage value. Must be higher than or equal to 0.</li> 
     <li><strong>Duration</strong>: Enter the duration time. If you need help, see the information about the duration field type in the Airtable support documentation. </li> 
     <li><strong>Rating</strong>: Enter the number. For example, "3 stars" is 3. A rating cannot be 0.</li> 
     <li><strong>Link</strong>: Enter the linked records IDs from the table. The order of record IDs will be reversed compared to what you see in the app.</li> 
     <li><strong>Rollup</strong>: Computed value: COUNT(values)</li> 
     <li><strong>Lookup</strong>: Array of long text fields</li> 
     <li><strong>Autonumber</strong>: Automatically incremented unique counter for each record.</li> 
     <li> <p><strong>Barcode</strong>: The barcode object may contain the following two properties, both of which are optional.</p> <p>Barcode data (text)</p> <p>Barcode symbology, for example, "upce" or "code39" (type)</p> </li> 
    </ul> --></td> 
  </tr> 
  <tr> 
   <td>Vínculos inteligentes</td> 
   <td> <p>Active esta opción para introducir nombres en lugar de ID de registro en campos que se vinculan a otra tabla. El registro se crea automáticamente en la tabla vinculada si no hay coincidencia.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Eliminar un registro {#delete-a-record}

Este módulo de acción elimina un registro en particular.

Especifique el ID y las ubicaciones del registro.

El módulo devuelve el ID del registro y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Conexión </td> 
   <td> <p>Para obtener instrucciones sobre la conexión de la cuenta de la tabla aérea a Workfront Fusion, consulte <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Conexión de la tabla de aire a Workfront Fusion</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>Base </td> 
   <td> <p>Seleccione la base que contiene el registro que desea eliminar.</p> </td> 
  </tr> 
  <tr> 
   <td>Tabla </td> 
   <td> <p>Seleccione la tabla que contiene el registro que desea eliminar.</p> </td> 
  </tr> 
  <tr> 
   <td>ID de registro</td> 
   <td> <p>Introduzca o asigne el ID de tabla aérea único del registro que desea que elimine el módulo. Puede recuperar el ID, por ejemplo, utilizando el módulo Buscar registros .</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Obtener un registro {#get-a-record}

Este módulo de acción recupera los detalles del registro.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Conexión </td> 
   <td> <p>Para obtener instrucciones sobre la conexión de la cuenta de la tabla aérea a Workfront Fusion, consulte <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Conexión de la tabla de aire a Workfront Fusion</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>Base </td> 
   <td> <p>Seleccione la base que contiene la tabla con el registro que desea recuperar.</p> </td> 
  </tr> 
  <tr> 
   <td>Tabla</td> 
   <td> <p> Seleccione la tabla que contiene el registro para el que desea recuperar detalles.</p> </td> 
  </tr> 
  <tr> 
   <td>ID de registro</td> 
   <td> <p> Introduzca o asigne el ID del registro para el que desea recuperar los detalles.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Registros de búsqueda {#search-records}

Este módulo de búsqueda busca registros en un objeto de la tabla dinámica que coincidan con la consulta de búsqueda especificada.

Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Conexión </td> 
   <td> <p>Para obtener instrucciones sobre la conexión de la cuenta de la tabla aérea a Workfront Fusion, consulte <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Conexión de la tabla de aire a Workfront Fusion</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>Base </td> 
   <td> <p>Seleccione la base que desee buscar registros.</p> </td> 
  </tr> 
  <tr> 
   <td>Tabla </td> 
   <td> <p>Seleccione la tabla en la que desea buscar registros.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Fórmula</p> </td> 
   <td> <p>Fórmula utilizada para filtrar registros. La fórmula se evalúa para cada registro y si el resultado no es <code>0</code>, <code>false</code>, <code>""</code>, <code>NaN</code>, <code>[]</code>o <code>#Error!</code> el registro se incluye en la respuesta.</p> <p>Si se combina con la variable <code>view</code>, solo se devuelven los registros de esa vista que satisfacen la fórmula.</p> <p>Por ejemplo, para incluir solo registros donde Name no esté vacío, pase:<code> NOT({Name} = '')</code></p> <p>Para obtener más información, busque información sobre referencias de campo de fórmula en la documentación de soporte de tabla de aire.</p> </td> 
  </tr> 
  <tr> 
   <td>Ordenar </td> 
   <td> <p>Seleccione la dirección de clasificación y el campo por el que desea ordenar los resultados.</p> </td> 
  </tr> 
  <tr> 
   <td>Vista </td> 
   <td> <p>Seleccione la vista que desee buscar para registros.</p> </td> 
  </tr> 
  <tr> 
   <td>Límite</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Actualizar un registro {#update-a-record}

Este módulo de acción actualiza un registro en particular.

Especifique el ID del registro y los nuevos datos que desea que contenga.

El módulo devuelve todos los campos estándar asociados con el registro, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Conexión </td> 
   <td> <p>Para obtener instrucciones sobre la conexión de la cuenta de la tabla aérea a Workfront Fusion, consulte <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Conexión de la tabla de aire a Workfront Fusion</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>Base </td> 
   <td> <p>Seleccione la base que contiene el registro que desea actualizar.</p> </td> 
  </tr> 
  <tr> 
   <td>Tabla </td> 
   <td> <p>Seleccione la tabla que contiene el registro que desea actualizar.</p> </td> 
  </tr> 
  <tr> 
   <td>ID de registro </td> 
   <td> <p>Introduzca o asigne el ID de tabla aérea único del registro que desea que actualice el módulo. Puede recuperar el ID, por ejemplo, utilizando el módulo Buscar registros .</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Registro</p> </td> 
   <td> <p>Introduzca los valores del nuevo registro. Los campos disponibles dependen de la tabla seleccionada.</p> <!--<p>In order to delete the content of the field, use the erase function. </p>  <p>Field types (via airtable.com/api):</p> 
    <ul> 
     <li> <p><strong>Text</strong>: string</p> <p>A single line of text.</p> </li> 
     <li> <p><strong>Long text</strong>: string</p> <p>The string can contain multiple lines of text with "mention tokens." For example:</p><pre>&lt;airtable:mention id="menE1i9oBaGX3DseR"&gt;@Alex&lt;/airtable:mention&gt;</pre> </li> 
     <li><strong>Attachment</strong>: Add the attachment. Airtable will download the file from the provided url and keep its own copy of it. If the File name field is left empty, Airtable will generate the name automatically.</li> 
     <li><strong>Checkbox</strong>: Select one of the options.</li> 
     <li><strong>Multiple select</strong>: Select multiple options in the checklist.</li> 
     <li><strong>Single select</strong>: Select one option from the drop-down menu.</li> 
     <li><strong>Collaborator</strong>: Enter the email that uniquely identifies a user in Airtable who this base is shared with.</li> 
     <li><strong>Date</strong>: UTC date, for example, 2019-09-05. (ISO 8601 formatted date)</li> 
     <li><strong>Phone number</strong>: A telephone number, for example, (415) 555-9876.</li> 
     <li><strong>Email</strong>valid email address.</li> 
     <li><strong>URL</strong>: lid URL such as airtable.com or https://airtable.coiverse.</li> 
     <li><strong>Number</strongnter a number.</li> 
     <li><strong>Currency</stro Currency value.</li> 
     <li><strong>Percent</stronA percentage value; must be equal to or more than 0i> 
     <li><strong>Duration</strong>: Enter the duration time. If you need help, see the information about the duration field type in the Airtable support documentation.</li> 
     <li><strong>Rating</strong>: Enter the number. For example, "3 stars" is 3. A rating cannot be 0.</li> 
     <li><strong>Link</strong>: Enter the linked records IDs from the table. The order of record IDs is reversed compared to what you see in the app.</li> 
     <li><strong>Rollup</strong>: Computed value: COUNT(values)</li> 
     <li><strong>Lookup</strong>: Array of long text fields</li> 
     <li><strong>Autonumber</strong>: Automatically incremented unique counter for each record.</li> 
     <li> <p><strong>Barcode</strong>: The barcode object may contain the following two properties, both of which are optional.</p> <p>Barcode data (text)</p> <p>Barcode symbology, for example, "upce" or "code39" (type)</p> </li> 
    </ul> --></td> 
  </tr> 
  <tr> 
   <td>Vínculos inteligentes</td> 
   <td> <p>Introduzca nombres en lugar de ID de registro en campos que se vinculan a otra tabla. El registro se crea automáticamente en la tabla vinculada si no hay coincidencia.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Actualizar un registro

Este módulo de acción actualiza o inserta un registro en particular.

Especifique el ID del registro y los nuevos datos que desea que contenga.

El módulo devuelve todos los campos estándar asociados con el registro, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Conexión </td> 
   <td> <p>Para obtener instrucciones sobre la conexión de la cuenta de la tabla aérea a Workfront Fusion, consulte <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Conexión de la tabla de aire a Workfront Fusion</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>Base </td> 
   <td> <p>Seleccione la base que contiene el registro que desea actualizar.</p> </td> 
  </tr> 
  <tr> 
   <td>Tabla </td> 
   <td> <p>Seleccione la tabla que contiene el registro que desea actualizar.</p> </td> 
  </tr> 
  <tr> 
   <td>ID de registro </td> 
   <td> <p>Si va a actualizar un registro, introduzca o asigne el ID de tabla de lanzamiento único del registro que desea que actualice el módulo. Puede recuperar el ID, por ejemplo, utilizando el módulo Buscar registros .</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Registro</p> </td> 
   <td> <p>Introduzca los valores del nuevo registro. Los campos disponibles dependen de la tabla seleccionada.</p> <!-- <p>In order to delete the content of the field, use the erase function. </p>  <p>Field types (via airtable.com/api):</p> 
    <ul> 
     <li> <p><strong>Text</strong>: string</p> <p>A single line of text.</p> </li> 
     <li> <p><strong>Long text</strong>: string</p> <p>The string can contain multiple lines of text with "mention tokens." For example:</p><pre>&lt;airtable:mention id="menE1i9oBaGX3DseR"&gt;@Alex&lt;/airtable:mention&gt;</pre> </li> 
     <li><strong>Attachment</strong>: Add the attachment. Airtable will download the file from the provided url and keep its own copy of it. If the File name field is left empty, Airtable will generate the name automatically.</li> 
     <li><strong>Checkbox</strong>: Select one of the options.</li> 
     <li><strong>Multiple select</strong>: Select multiple options in the checklist.</li> 
     <li><strong>Single select</strong>: Select one option from the drop-down menu.</li> 
     <li><strong>Collaborator</strong>: Enter the email that uniquely identifies a user in Airtable who this base is shared with.</li> 
     <li><strong>Date</strong>: UTC date, for example, 2019-09-05. (ISO 8601 formatted date)</li> 
     <li><strong>Phone number</strong>: A telephone number, for example, (415) 555-9876.</li> 
     <li><strong>Email</strong>valid email address.</li> 
     <li><strong>URL</strong>: lid URL such as airtable.com or https://airtable.coiverse.</li> 
     <li><strong>Number</strongnter a number.</li> 
     <li><strong>Currency</stro Currency value.</li> 
     <li><strong>Percent</stronA percentage value; must be equal to or more than 0i> 
     <li><strong>Duration</strong>: Enter the duration time. If you need help, see the information about the duration field type in the Airtable support documentation.</li> 
     <li><strong>Rating</strong>: Enter the number. For example, "3 stars" is 3. A rating cannot be 0.</li> 
     <li><strong>Link</strong>: Enter the linked records IDs from the table. The order of record IDs is reversed compared to what you see in the app.</li> 
     <li><strong>Rollup</strong>: Computed value: COUNT(values)</li> 
     <li><strong>Lookup</strong>: Array of long text fields</li> 
     <li><strong>Autonumber</strong>: Automatically incremented unique counter for each record.</li> 
     <li> <p><strong>Barcode</strong>: The barcode object may contain the following two properties, both of which are optional.</p> <p>Barcode data (text)</p> <p>Barcode symbology, for example, "upce" or "code39" (type)</p> </li> 
    </ul> --></td> 
  </tr> 
  <tr> 
   <td>Vínculos inteligentes</td> 
   <td> <p>Introduzca nombres en lugar de ID de registro en campos que se vinculan a otra tabla. El registro se crea automáticamente en la tabla vinculada si no hay coincidencia.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Registros de Watch {#watch-records}

Este módulo de déclencheur inicia un escenario cuando se crea o actualiza un registro en la tabla especificada.

>[!NOTE]
>
>Para utilizar este módulo, el campo Hora de creación o Hora de última modificación debe crearse en la tabla.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Conexión </td> 
   <td> <p>Para obtener instrucciones sobre la conexión de la cuenta de la tabla aérea a Workfront Fusion, consulte <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Conexión de la tabla de aire a Workfront Fusion</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>Base </td> 
   <td> <p>Seleccione la base que desee ver para los registros nuevos.</p> </td> 
  </tr> 
  <tr> 
   <td>Tabla </td> 
   <td> <p>Seleccione la tabla que desee ver para los registros nuevos.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Configuración del déclencheur</p> </td> 
   <td> <p>Campo de déclencheur</p> <p>A <code>Created Time</code> o <code>Last Modified Time</code> campo que se utiliza para ordenar registros. Si no tiene un <code>Created Time</code> o <code>Last Modified Time</code> en el esquema, debe crear uno. </p> <p>Campo Etiqueta</p> <p>Campo que se utiliza como etiqueta para un registro, por ejemplo, en el cuadro de diálogo Elegir dónde iniciar.</p> </td> 
  </tr> 
  <tr> 
   <td>Límite</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo vea durante cada ciclo de ejecución del escenario.</p> </td> 
  </tr> 
  <tr> 
   <td>Vista</td> 
   <td> <p>Seleccione la vista que desee utilizar.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Fórmula</p> </td> 
   <td> <p>Fórmula utilizada para filtrar registros. La fórmula se evalúa para cada registro y si el resultado no es <code>0</code>, <code>false</code>, <code>""</code>, <code>NaN</code>, <code>[]</code>o <code>#Error!</code> el registro se incluye en la respuesta.</p> <p>Si se combina con la variable <code>view</code>, solo se devuelven los registros de esa vista que satisfacen la fórmula.</p> <p>Por ejemplo, para incluir solo registros donde Name no esté vacío, pase:<code> NOT({Name} = '')</code></p> <p>Para obtener más información, consulte la información sobre referencias de campo de fórmula en la documentación de soporte de tabla de aterrizaje.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Respuestas de Watch

Este módulo de déclencheur inicia un escenario cuando se envía un formulario.

>[!NOTE]
>
>Esta funcionalidad solo está disponible para Airtable Pro Plan de pago.

La URL del enlace web debe generarse en Workfront Fusion y agregarse a la configuración del formulario en la tabla de aterrizaje.

1. Añada el módulo Watch New Responses al escenario de Workfront Fusion .
1. Genere y copie la URL del enlace web.

   Para obtener instrucciones, consulte [Déclencheur instantáneos (enlaces web) en Adobe Workfront Fusion](../../workfront-fusion/webhooks/instant-triggers-webhooks.md).

1. Inicie sesión en su cuenta de Airtable.
1. Abra la Base y la tabla que desee utilizar para el formulario y cree una vista Formulario.
1. Defina el formulario como sea necesario, desplácese hacia abajo en el formulario y active la opción Redireccionar a dirección URL después de enviar el formulario .
1. Introduzca la URL de Weblock generada en el paso 2 del cuadro de diálogo mostrado y añada ?record_id={record_id} justo después de la URL de weblock para incluir el ID de registro en la salida del módulo y, a continuación, haga clic en Guardar. La URL resultante, por ejemplo, tendrá este aspecto:
1. Vuelva al escenario de Workfront Fusion y ejecute el módulo Watch Responses solo para cargar campos de la tabla de aire y poder asignar esos campos a los demás módulos.
1. Envíe el formulario en Airtable donde la opción Redireccionar a URL después de enviar el formulario está habilitada y se ha añadido la URL de Weblock (paso 6 anterior).

   El módulo Respuestas de Watch se activa y se cargan los datos deseados.

1. Añada el módulo Airtable > Get a Record justo después del módulo Airtable > Watch Responses y asigne el record_id al campo Record ID .

Ahora, cada vez que se envía el formulario, se activa el módulo Watch Responses del escenario de Workfront Fusion y el módulo Get a Record devuelve los detalles del formulario enviado.

#### Realizar una llamada de API

#### Llamada de API personalizada

Este módulo de acción le permite realizar una llamada autenticada personalizada al [!DNL Airtable] API. De este modo, puede crear una automatización del flujo de datos que no se pueda lograr con la otra [!DNL Airtable] módulos.

La acción se basa en el tipo de entidad (tipo de objeto Allocadia) que especifique.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Conexión</p> </td> 
   <td> <p>Para obtener instrucciones sobre la conexión de la cuenta de la tabla aérea a Workfront Fusion, consulte <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Conexión de la tabla de aire a Workfront Fusion</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td>Especifique una ruta relativa a <code>https://api.airtable.com/}</code>. Ejemplo: <code>v0/{base}/{table}</code> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Método</td> 
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada a la API. Para obtener más información, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Encabezados</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p> <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] añade los encabezados de autorización por usted.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Cadena de consulta</td> 
   <td> <p>Añadir la consulta para la llamada de API en forma de Clave y Valor</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Cuerpo</td> 
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Al utilizar afirmaciones condicionales como <code>if</code> en su JSON, ponga las comillas fuera de la afirmación condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
