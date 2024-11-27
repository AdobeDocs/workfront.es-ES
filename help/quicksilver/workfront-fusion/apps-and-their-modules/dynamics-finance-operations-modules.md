---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de finanzas y operaciones de Microsoft Dynamics 365
description: En un escenario  [!DNL Adobe Workfront Fusion] puede automatizar los flujos de trabajo que utilizan Microsoft Dynamics 365 Finance and Operations, así como conectarlos a varias aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion
source-git-commit: 130437dd44db5db2a94914fb0e42fd35a7c14291
workflow-type: tm+mt
source-wordcount: '995'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics 365 Finance and Operations modules]

En un escenario de [!DNL Adobe Workfront Fusion], puede automatizar los flujos de trabajo que utilizan [!DNL Microsoft Dynamics 365], así como conectarlo a varias aplicaciones y servicios de terceros.

>[!NOTE]
>
>El conector [!DNL Microsoft Dynamics 365 Finance and Operations] no admite [!DNL Dynamics 365].
>
>Para módulos de Microsoft Dynamics 365, consulte [[!DNL Microsoft Dynamics 365 modules]](/help/quicksilver/workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md).

Si necesita instrucciones para crear un escenario, consulte [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obtener información acerca de los módulos, vea [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Crear una conexión

Para crear una conexión para los módulos de operaciones y finanzas de Microsoft Dynamics 365:

1. En cualquier módulo de Microsoft Dynamics 365 Finance and Operations, haga clic en **[!UICONTROL Agregar]** junto al cuadro Conexión.

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
          <p>Seleccione si va a crear una conexión estándar de Dynamics Finance and Operations o una conexión con un código de autorización.</p>
        </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Nombre de conexión]</td>
        <td>
          <p>Escriba un nombre para esta conexión.</p>
        </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL ID de cliente]</td>
        <td>Introduzca el [!UICONTROL Client ID] de Dynamics Finance and Operations.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Secreto de cliente]</td>
        <td>Introduzca el [!UICONTROL Secreto del cliente] de Dynamics Finance and Operations. </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL ID de inquilino]</td>
        <td>Introduzca su ID de inquilino de Dynamics Finance and Operations.</td>
        </tr>
        <tr>
        <td role="rowheader">Recurso</td>
        <td>Introduzca la URL de su cuenta de Dynamics Finance and Operations (sin https://)</td>
        </tr>
      </tbody>
    </table>

1. Haga clic en **[!UICONTROL Continuar]** para guardar la conexión y volver al módulo.



## Módulos de finanzas y operaciones de Microsoft Dynamics 365 y sus campos

>[!IMPORTANT]
>
>Las entidades de datos disponibles a través de la API de F&amp;O de Dynamics 365 pueden variar según la instancia. Si no está seguro de qué entidades están disponibles a través de la API, resulta útil ver las entidades de su instancia utilizando el punto final &quot;data&quot;. El punto final &quot;data&quot; en Dynamics 365 Finance and Operations es la URL raíz para acceder a los servicios OData. Este extremo le permite interactuar con varias entidades de datos expuestas por el sistema mediante protocolos OData estándar.
>
>Puede recuperar estas entidades mediante el módulo de llamada de API personalizado.
>
><!--For more information -->



### Crear elemento de entidad

Este módulo de acción crea un nuevo elemento de entidad en Microsoft Dynamics 365 Finance and Operations.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Conexión]</td>
    <td> <p>Para obtener instrucciones sobre cómo conectar Microsoft Dynamics 365 Finance and Operations a [!DNL Workfront Fusion], consulte <a href="#create-a-connection" class="MCXref xref">Crear una conexión</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Entidad]</td>
     <td>Introduzca o asigne el tipo de entidad de Dynamics Finance and Operations que desea crear.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Cuerpo]</td>
     <td> <p>Introduzca o asigne un cuerpo JSON que contenga los datos que desea incluir en el nuevo elemento de entidad.</p> </td> 
  </tr> 
 </tbody> 
</table>



### Eliminar elemento de entidad

Este módulo de acción elimina un elemento de entidad de Dynamics Finance and Operations. El elemento se identifica con sus campos Primary key.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Conexión]</td>
    <td> <p>Para obtener instrucciones sobre cómo conectar Microsoft Dynamics 365 Finance and Operations a [!DNL Workfront Fusion], consulte <a href="#create-a-connection" class="MCXref xref">Crear una conexión</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Entidad]</td>
     <td>Introduzca o asigne el tipo de entidad de Dynamics Finance and Operations que desea eliminar.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Campos de clave principal]</td>
     <td> Los campos Primary key identifican el elemento. Para cada campo de clave principal que desee proporcionar, haga clic en <b>Agregar elemento</b> y escriba o asigne la clave y el valor únicos que identifican ese elemento. </td> 
  </tr> 
 </tbody> 
</table>

### Realizar una llamada de API personalizada

Este módulo de acción realiza una llamada personalizada a la API de Dynamics Finance and Operations.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
    <td> <p>Para obtener instrucciones sobre cómo conectar Microsoft Dynamics 365 Finance and Operations a [!DNL Workfront Fusion], consulte <a href="#create-a-connection" class="MCXref xref">Crear una conexión</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>Introduzca una ruta relativa a la URL de Dynamics Finance and Operations.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada de API. Para obtener más información, vea <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar. Determina el tipo de contenido de la solicitud.</p> <p>Por ejemplo,<code> {"Content-type":"application/json"}</code></p> <p>Nota: Si se producen errores y es difícil determinar su origen, considere la posibilidad de modificar los encabezados basados en la documentación de [!DNL Workfront]. Si su llamada de API personalizada devuelve un error de solicitud HTTP 422, intente utilizar un encabezado <code>"Content-Type":"text/plain"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadena de consulta]</td> 
   <td> <p>Añada la consulta para la llamada de API en forma de objeto JSON estándar.</p> <p>Por ejemplo: <code>{"name":"something-urgent"}</code></p> <p>Sugerencia: Le recomendamos que envíe información a través del cuerpo de JSON en lugar de como parámetros de consulta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cuerpo]</td> 
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Cuando utilice afirmaciones condicionales como <code>if</code> en su JSON, coloque las comillas fuera de la afirmación condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>



### Leer elemento de entidad

Este módulo de acción devuelve datos de un elemento de entidad. El elemento se identifica con sus campos Primary key.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Conexión]</td>
    <td> <p>Para obtener instrucciones sobre cómo conectar Microsoft Dynamics 365 Finance and Operations a [!DNL Workfront Fusion], consulte <a href="#create-a-connection" class="MCXref xref">Crear una conexión</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Entidad]</td>
     <td>Introduzca o asigne el tipo de entidad de Dynamics Finance and Operations que desea leer.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Campos de clave principal]</td>
     <td> Los campos Primary key identifican el elemento. Para cada campo de clave principal que desee proporcionar, haga clic en <b>Agregar elemento</b> y escriba o asigne la clave y el valor únicos que identifican ese elemento. </td> 
  </tr> 
 </tbody> 
</table>

### Actualizar elemento de entidad

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Conexión]</td>
    <td> <p>Para obtener instrucciones sobre cómo conectar Microsoft Dynamics 365 Finance and Operations a [!DNL Workfront Fusion], consulte <a href="#create-a-connection" class="MCXref xref">Crear una conexión</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Entidad]</td>
     <td>Introduzca o asigne el tipo de entidad de Dynamics Finance and Operations que desea actualizar.</td> 
  </tr>  
  <tr> 
    <td>[!UICONTROL Campos de clave principal]</td>
     <td> Los campos Primary key identifican el elemento. Para cada campo de clave principal que desee proporcionar, haga clic en <b>Agregar elemento</b> y escriba o asigne la clave y el valor únicos que identifican ese elemento. </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Cuerpo]</td>
     <td> <p>Introduzca o asigne un cuerpo JSON que contenga los datos que desea incluir en el nuevo elemento de entidad.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Buscar

Este módulo de búsqueda devuelve los resultados en función de los criterios especificados.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su aplicación [!DNL Workfront] a [!DNL Workfront Fusion], vea <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Workfront] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Entidad]</td> 
   <td>Introduzca o asigne el tipo de entidad de Dynamics Finance and Operations que desea buscar.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Criterios de búsqueda]</td> 
   <td> <p>Introduzca el campo por el que desea buscar, el operador que desea utilizar en la consulta y el valor que está buscando en el campo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Ordenar por]</td> 
   <td> <p>Introduzca o asigne el campo por el que desea ordenar los resultados.</p> </td> 
  </tr> 
 </tbody> 
</table>


<!--

### List All

This module lists all records for a given entity.  The item is identified by its Primary key fields.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection]</td>
    <td> <p>For instructions about connecting Microsoft Dynamics 365 Finance and Operations to [!DNL Workfront Fusion], see <a href="#create-a-connection" class="MCXref xref">Create a connection</a> in this article.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Record Type]</td>
     <td>Choose the Dynamics Finance and Operations entity type that you want the module to list.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Outputs]</td>
     <td> <p>Select the information you want included in the output bundle for this module.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Watch Record

This trigger module starts a scenario when a record of the given type is created or updated.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
    <td> <p>For instructions about connecting Microsoft Dynamics 365 Finance and Operations to [!DNL Workfront Fusion], see <a href="#create-a-connection" class="MCXref xref">Create a connection</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Select the type of [!DNL Workfront] record that you want the module to watch.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Enter the field that you want to search by, the operator you want to use in your query, and the value that you are searching for in the field.</p> <p>Note: Do not use <code>username </code>in your search criteria. Including <code>username </code>in an API query to [!DNL Workfront] logs the user into Workfront, and the search will not be successful.</p> <p>Note: <code>In</code> and <code>NotIn</code>work with arrays. The inputs should be in array format.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Select the information you want included in the output bundle for this module.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->
