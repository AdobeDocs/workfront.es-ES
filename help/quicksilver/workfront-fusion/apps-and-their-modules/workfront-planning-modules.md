---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de Adobe Workfront Planning
description: Con el [!DNL Adobe Workfront Planning] módulos, puede iniciar un [!DNL Adobe Workfront Fusion] según los eventos de su [!DNL Adobe] Cuenta de Workfront Planning, cree, lea o actualice acuerdos y otros registros, busque registros con los criterios definidos y cargue documentos.
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
exl-id: 892fdaf3-935e-4e66-a01c-9e9b6e0daf3e
source-git-commit: e067c5ff34c31060ca6fd392289d845f53a5ef3a
workflow-type: tm+mt
source-wordcount: '1116'
ht-degree: 0%

---

# [!DNL Adobe Workfront Planning] módulos

Con el [!DNL Adobe Workfront Planning] , puede almacenar en déclencheur un escenario cuando se produzcan eventos en Workfront Planning. También puede crear, leer, actualizar y eliminar registros, o realizar una llamada de API personalizada a su [!DNL Adobe Workfront Planning] cuenta.

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

## Cree una conexión con [!DNL Adobe Workfront Planning]

Puede crear una conexión con su [!DNL Workfront Planning] cuenta directamente desde dentro de un [!DNL Workfront Fusion] módulo.

1. En cualquier [!DNL Workfront Planning] módulo de la aplicación, haga clic en **[!UICONTROL Añadir]** junto al [!UICONTROL Conexión] cuadro.
1. Escriba un nombre para esta conexión.
1. Seleccione si desea conectarse a un entorno de producción o de no producción.
1. Seleccione si desea conectarse a una cuenta de servicio o a una cuenta personal.
1. Clic **[!UICONTROL Inicio de sesión de SAML]** para crear la conexión y volver al módulo.

## [!DNL Adobe Workfront Planning] módulos y sus campos

### Ver eventos

Este módulo de déclencheur inicia un escenario cuando se crea, actualiza o elimina un registro, tipo de registro o espacio de trabajo en Workfront Planning.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Webhook]</td>
      <td>Seleccione el webhook que desee utilizar o haga clic en Agregar para crear uno nuevo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Workfront Planning], consulte <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Cree una conexión con [!DNL Adobe Workfront Planning]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo de objeto]</td>
      <td>Seleccione si desea ver registros, tipos de registros o espacios de trabajo.</td>
    </tr>
     <tr data-mc-conditions=""> 
      <td> <p>[!UICONTROL Filtros de eventos]</p> </td> 
      <td> <p>Puede establecer filtros para inspeccionar sólo los registros que cumplan los criterios seleccionados.</p> <p>Para cada filtro, introduzca el campo que desea que evalúe el filtro, el operador y el valor que desea que permita el filtro. Puede utilizar más de un filtro añadiendo reglas AND.</p> <p>Nota: No puede editar filtros en filtros existentes [!DNL Workfront] webhooks. Para configurar diferentes filtros para [!DNL Workfront] Suscripciones de eventos, elimine el webhook actual y cree uno nuevo.</p> <p>Para obtener más información sobre los filtros de eventos, consulte <a href="/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#event-subscription-filters-in-the-workfront--watch-events-modules" class="MCXref xref">Filtros de suscripción de evento en la [!DNL Workfront] &gt; Módulos de [!UICONTROL Watch Events]</a> en el artículo módulos de Workfront.</p> </td> 
     </tr> 
    <tr>
      <td role="rowheader">[!UICONTROL Objetos que ver]</td>
      <td>Seleccione si desea ver las nuevas. registros actualizados, nuevos y actualizados o eliminados.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Excluir actualizaciones realizadas por esta conexión]</p>
      </td>
      <td>Habilite esta opción para evitar que el escenario se active cuando la conexión utilizada por este módulo realice un cambio. Esto evita que se active otra instancia del escenario si este realiza una acción de activación.</td> 
      </tr>
  </tbody>
</table>

### Eliminación de un tipo de registro

Este módulo de acción elimina un solo tipo de registro en Workfront Planning por su ID.

>[!WARNING]
>
>Al eliminar un tipo de registro en Workfront Planning también se eliminan todos los registros de la tabla de tipo de registro.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Workfront Planning], consulte <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Cree una conexión con [!DNL Adobe Workfront Planning]</a> en este artículo.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL ID de tipo de registro]</p>
      </td>
      <td>Introduzca o asigne el ID del campo que desea eliminar.</td> 
      </tr>
  </tbody>
</table>

### Realizar una llamada de API personalizada

Este módulo realiza una llamada de API personalizada a [!DNL Adobe Workfront Planning] API.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Workfront Planning], consulte <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Cree una conexión con [!DNL Adobe Workfront Planning]</a> en este artículo.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Ruta]</p>
      </td>
      <td>
        <p>Introduzca una ruta relativa a https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/</p>
      </td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL API version]</p>
      </td>
      <td>
        <p>Seleccione la versión de la API que desee utilizar. Si no selecciona ninguna versión, se utilizará la más reciente de forma predeterminada.</p>
      </td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Ruta de API override]</p>
      </td>
      <td>
        <p>Introduzca una ruta relativa a https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Método]</p>
      </td>
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada de API. Para obtener más información, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Encabezados]</td>
      <td>
        <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p>
        <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] agrega encabezados de autorización automáticamente.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Cadena de consulta]  </td>
      <td>
        <p>Para cada par clave/valor que desee agregar a la cadena de consulta, haga clic en <b>Añadir elemento</b> e introduzca la clave y el valor.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Cuerpo]</td>
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Cuando se utilizan afirmaciones condicionales como <code>if</code> en su JSON, ponga las comillas fuera del enunciado condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

<!--

### Delete a field

This action module deletes a single field in Workfront Planning by its ID.

>[!WARNING]
>
>Deleting a field in Workfront Planning deletes it and any data in it from every object of that record type in Workfront Planning.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Workfront Planning], see <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Create a connection to [!DNL Adobe Workfront Planning]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Field ID]</p>
      </td>
      <td>Enter or map the ID of the record type you want to delete.</td> 
      </tr>
  </tbody>
</table>

### Get a field 


This action module retrieves a single field in Workfront Planning by its ID.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Workfront Planning], see <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Create a connection to [!DNL Adobe Workfront Planning]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Field ID]</p>
      </td>
      <td>Enter or map the ID of the field you want to delete.</td> 
      </tr>
  </tbody>
</table>

-->

### Creación de un registro

Esta acción crea un único registro en Workfront Planning.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Workfront Planning], consulte <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Cree una conexión con [!DNL Adobe Workfront Planning]</a> en este artículo.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL ID de tipo de registro]</p>
      </td>
      <td>Introduzca o asigne el tipo de registro que desea crear. Los tipos de registro disponibles se basan en su cuenta de Workfront Planning.</td> 
      </tr>
     <tr>
      <td role="rowheader">
        <p>Otros campos</p>
      </td>
      <td>Estos campos se basan en el tipo de registro seleccionado.</td> 
      </tr>
     <tr>
  </tbody>
</table>

### Eliminación de un registro

Este módulo de acción elimina el registro especificado en Workfront Planning.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Workfront Planning], consulte <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Cree una conexión con [!DNL Adobe Workfront Planning]</a> en este artículo.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL ID de registro]</p>
      </td>
      <td>Introduzca o asigne el ID del registro que desea eliminar.</td> 
      </tr>
  </tbody>
</table>

<!--

### Get all records

This action module retrieves all records from an [!DNL Adobe Workfront Planning] account.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Workfront Planning], see <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Create a connection to [!DNL Adobe Workfront Planning]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximum number of returned records]</p>
      </td>
      <td>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</td> 
      </tr>
  </tbody>
</table>

-->

### Obtener un registro

Este módulo de acción recupera un único registro de [!DNL Adobe Workfront Planning], especificado por su ID.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Workfront Planning], consulte <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Cree una conexión con [!DNL Adobe Workfront Planning]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de registro]</td>
      <td>Introduzca o asigne el ID del registro que desea recuperar.</td>
    </tr>
  </tbody>
</table>

### Obtener registros por tipo de registro

Este módulo de acción recupera todos los registros del tipo especificado.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Workfront Planning], consulte <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Cree una conexión con [!DNL Adobe Workfront Planning]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>Seleccione o asigne el espacio de trabajo que contiene los registros que desea recuperar.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo de registro]</td>
      <td>Seleccione el tipo de registro que desea recuperar.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Número máximo de registros devueltos]</p>
      </td>
      <td>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</td> 
  </tbody>
</table>

### Obtener tipos de registros

Este módulo de acción recupera una lista de tipos de registro en una [!DNL Adobe Workfront Planning] cuenta.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Workfront Planning], consulte <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Cree una conexión con [!DNL Adobe Workfront Planning]</a> en este artículo.</td>
    </tr>
  </tbody>
</table>

### Actualizar registro

Esta acción actualiza un único registro en Workfront Planning.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Workfront Planning], consulte <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Cree una conexión con [!DNL Adobe Workfront Planning]</a> en este artículo.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL ID de registro]</p>
      </td>
      <td>Introduzca o asigne el tipo de registro que desea actualizar Los tipos de registro disponibles se basan en su cuenta de Workfront Planning.</td> 
      </tr>
     <tr>
      <td role="rowheader">
        <p>Otros campos</p>
      </td>
      <td>Estos campos se basan en el tipo de registro seleccionado.</td> 
      </tr>
     <tr>
  </tbody>
</table>

### Buscar registros

Este módulo de acción recupera una lista de registros en función de los criterios especificados.

>[!NOTE]
>
>Este módulo está en construcción.
