---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos ServiceNow
description: En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL ServiceNow], así como conectarlo a múltiples aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion
exl-id: b362cd8b-06b3-4f4c-b405-a2afc24abddb
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1613'
ht-degree: 1%

---

# [!DNL ServiceNow] módulos

En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL ServiceNow], así como conectarlo a múltiples aplicaciones y servicios de terceros.

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

Para usar [!DNL ServiceNow] módulos, debe tener un [!DNL ServiceNow] cuenta.

## Connect [!DNL ServiceNow] hasta [!DNL Workfront Fusion]

Para crear una conexión para su [!DNL ServiceNow] módulos:

1. Clic **[!UICONTROL Añadir]** junto al [!UICONTROL Conexión] cuando empiece a configurar la primera [!DNL ServiceNow] módulo.
1. Introduzca lo siguiente:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Nombre de conexión]</p> </td> 
      <td>Introduzca un nombre para el nuevo [!DNL ServiceNow] conexión</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Nombre de usuario]</p> </td> 
      <td>Introduzca su [!DNL ServiceNow] nombre de usuario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Contraseña]</p> </td> 
      <td>Introduzca su contraseña de ServiceNow.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Instancia]</p> </td> 
      <td> <p>Introduzca la dirección de su [!DNL ServiceNow] cuenta sin <code>https://</code> (normalmente <code>&lt;company>.service-now.com</code>).</p> </td> 
     </tr> 
    </tbody> 
   </table>

## [!UICONTROL ServiceNow] módulos y sus campos

Al configurar [!DNL ServiceNow] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, se añaden [!DNL ServiceNow] Los campos pueden mostrarse, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignación de información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>Si se selecciona un registro personalizado en una &quot;[!UICONTROL Tipo de registro]&quot;, puede llevar algún tiempo cargar los campos personalizados.
>
>Si no hay registros personalizados, la lista desplegable estará vacía.

* [[!UICONTROL Ver registros]](#watch-records)
* [[!UICONTROL Llamada de API personalizada]](#custom-api-call)
* [[!UICONTROL Leer un registro]](#read-a-record)
* [[!UICONTROL Desactivar un usuario]](#deactivate-a-user)
* [[!UICONTROL Descargar un archivo adjunto]](#download-an-attachment)
* [[!UICONTROL Cargar un archivo adjunto]](#upload-an-attachment)
* [[!UICONTROL Creación de un registro]](#create-a-record)
* [[!UICONTROL Actualización de un registro]](#update-a-record)
* [[!UICONTROL Eliminación de un registro]](#delete-a-record)
* [[!UICONTROL Búsqueda de registros]](#search-for-records)

### [!UICONTROL Ver registros]

Este módulo de déclencheur activa un escenario cuando se crea o actualiza un registro.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de ServiceNow a [!DNL Workfront Fusion], consulte <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de tabla]</td> 
   <td>Seleccione si la tabla que desea ver es una tabla personalizada o una tabla estándar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td>Seleccione el tipo de registro que desea ver.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pantalla]</td> 
   <td>Seleccione el tipo de valores que desea mostrar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salidas]</td> 
   <td>Seleccione los campos de los que desea que salga el módulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td>Seleccione si desea ver registros nuevos o actualizados.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Llamada de API personalizada]

Este módulo de acción le permite realizar una llamada autenticada personalizada a [!DNL ServiceNow] API. De este modo, se puede crear una automatización del flujo de datos que el otro no puede realizar [!DNL ServiceNow] módulos.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de ServiceNow a [!DNL Workfront Fusion], consulte <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL relativa]</td> 
   <td> <p>Escriba la dirección del servidor web con el que desea que interactúe el módulo.</p> <p>Puede escribir una dirección URL relativa, lo que significa que no tiene que incluir el protocolo (por ejemplo, <code>http://</code>) al principio. Esto sugiere al servidor web que la interacción se está produciendo en el servidor.</p> <p>Por ejemplo: <code>[!DNL /api/conversations].create</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   td&gt; <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada de API. Para obtener más información, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p> <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p> </td> 
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

### [!UICONTROL Leer un registro]

Este módulo de acción lee un [!DNL ServiceNow] mediante el ID del sistema.

El módulo devuelve cualquier campo estándar asociado con el registro, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de ServiceNow a [!DNL Workfront Fusion], consulte <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record System ID]</td> 
   <td>Introduzca o asigne el único [!DNL ServiceNow] ID del registro que desea que lea el módulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de tabla]</td> 
   <td>Seleccione si el registro que desea leer está en una tabla personalizada o en una tabla estándar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td>Seleccione el tipo de [!DNL ServiceNow] que desea que el módulo lea.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pantalla]</td> 
   <td>Seleccione el tipo de valores que desea mostrar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salidas]</td> 
   <td>Seleccione los campos de los que desea que salga el módulo.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Desactivar un usuario]

Este módulo de acción desactiva un usuario en [!DNL ServiceNow] mediante el ID del sistema.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de ServiceNow a [!DNL Workfront Fusion], consulte <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL User System ID]</td> 
   <td> Introduzca o asigne el único [!DNL ServiceNow] ID del usuario que desea que el módulo desactive.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Descargar un archivo adjunto]

Este módulo de acción descarga un archivo adjunto en una [!DNL ServiceNow] registro.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de ServiceNow a [!DNL Workfront Fusion], consulte <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de sistema de datos adjuntos]</td> 
   <td> Introduzca o asigne el único [!DNL ServiceNow] ID del archivo adjunto que desea que descargue el módulo.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Cargar un archivo adjunto]

Este módulo de acción carga un archivo adjunto en una [!DNL ServiceNow] registro.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de ServiceNow a [!DNL Workfront Fusion], consulte <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre de tabla]</td> 
   <td>Introduzca o asigne el nombre de la tabla en la que desea cargar el archivo adjunto.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de sistema]</td> 
   <td>Introduzca o asigne el único [!DNL ServiceNow] ID del sistema en el que desea cargar el archivo adjunto.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre de archivo]</td> 
   <td>Escriba o asigne un nombre para el archivo adjunto</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contenido de archivo]</td> 
   <td>Introduzca o asigne el archivo que desea cargar [!DNL ServiceNow].</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Creación de un registro]

Este módulo de acción crea un nuevo [!DNL ServiceNow] registro.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de ServiceNow a [!DNL Workfront Fusion], consulte <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de tabla]</td> 
   <td>Seleccione si desea crear un registro en una tabla personalizada o en una tabla estándar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td>Seleccione el tipo de [!DNL ServiceNow] que desea que el módulo cree. A continuación, puede rellenar los campos disponibles para este tipo de registro.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Actualización de un registro]

Este módulo de acción crea un nuevo [!DNL ServiceNow] registro.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de ServiceNow a [!DNL Workfront Fusion], consulte <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record System ID]</td> 
   <td>Introduzca o asigne el único [!DNL ServiceNow] ID del registro que desea que actualice el módulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de tabla]</td> 
   <td>Seleccione si el registro que desea actualizar se encuentra en una tabla personalizada o estándar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td>Seleccione el tipo de [!DNL ServiceNow] que desea que el módulo actualice. A continuación, puede rellenar los campos disponibles para este tipo de registro.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Eliminación de un registro]

Este módulo de acción elimina un incidente o un usuario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de ServiceNow a [!DNL Workfront Fusion], consulte <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td>Seleccione si desea eliminar un incidente o un usuario.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de sistema]</td> 
   <td>Introduzca o asigne el único [!DNL ServiceNow] ID del registro que desea que elimine el módulo.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Búsqueda de registros]

Este módulo busca registros utilizando los criterios seleccionados.

El módulo devuelve cualquier campo estándar asociado con el registro, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de ServiceNow a [!DNL Workfront Fusion], consulte <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de tabla]</td> 
   <td>Seleccione si la tabla que desea buscar es una tabla personalizada o una tabla estándar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td>Seleccione el tipo de registro que desea buscar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conjunto de resultados]</td> 
   <td>Seleccione si desea que el módulo devuelva todos los registros que coincidan con los criterios o sólo el primer registro que lo coincida. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recuento máximo de registros]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de búsqueda]</td> 
   <td> <p>Seleccione el tipo de búsqueda que desea que ejecute el módulo</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Consulta avanzada]</strong> </p> 
      <ul> 
       <li> <p>[!UICONTROL Consulta de búsqueda]</p> <p>Introduzca la consulta de búsqueda personalizada. Para obtener información sobre [!DNL ServiceNow] consultas de búsqueda personalizadas, consulte la <a href="https://docs.servicenow.com/bundle/orlando-platform-user-interface/page/use/common-ui-elements/reference/r_OpAvailableFiltersQueries.html">Documentación de consulta de ServiceNow</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Simple]</strong> </p> 
      <ul> 
       <li> <p>[!UICONTROL Criterios de búsqueda]</p> <p>Introduzca los criterios según los cuales desea que busque el módulo. Para obtener más información sobre la configuración de filtros de búsqueda, consulte <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Añadir un filtro a un escenario en Adobe Workfront Fusion</a>.</p> </li> 
       <li> <p>[!UICONTROL Ordenar por]</p> <p>Indique por qué campo desea que el módulo ordene los resultados y si deben ordenarse de forma ascendente o descendente.</p> </li> 
      </ul> </li> 
    </ul> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pantalla]</td> 
   <td>Seleccione el tipo de valores que desea mostrar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salidas]</td> 
   <td>Seleccione los campos de los que desea que salga el módulo.</td> 
  </tr> 
 </tbody> 
</table>
