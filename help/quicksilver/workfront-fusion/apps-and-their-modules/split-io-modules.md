---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Módulos Split.io
description: En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL Split.io], así como conectarlo a varias aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion
exl-id: 4576a2e4-b495-430e-a9de-4e1ec7379ab8
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1773'
ht-degree: 0%

---

# [!DNL Split.io] módulos

En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL Split.io], así como conectarlo a varias aplicaciones y servicios de terceros.

Si necesita instrucciones para crear un escenario, consulte [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

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

Para usar [!DNL Split.io] módulos, debe tener un [!DNL Split.io] cuenta.

## Connect [!DNL Split.io] a [!DNL Workfront Fusion] {#connect-split-io-to-workfront-fusion}

Puede crear una conexión con su [!DNL Split.io] cuenta directamente desde dentro de un [!DNL Split.io] módulo.

1. En cualquier [!DNL Split.io] módulo, haga clic en **[!UICONTROL Agregar]** junto a la variable [!UICONTROL Conexión] campo .
1. Introduzca un nombre para la conexión.
1. Escriba la [!DNL Split.io] Clave de API.

   Para obtener más información, consulte [!DNL Split.io] claves de API, consulte [Claves de API](https://help.split.io/hc/en-us/articles/360019916211-API-keys) en el [!DNL Split.io] documentación.

1. Haga clic en **[!UICONTROL Continuar]** para crear la conexión y volver al módulo .

## [!DNL Split.io] módulos y sus campos

Al configurar [!DNL split.io] módulos, [!DNL Workfront Fusion] muestra los campos que se enumeran a continuación. Además de estos, se incluyen [!DNL split.io] pueden mostrarse los campos, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón de asignación encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Acciones](#actions)
* [Búsquedas](#searches)

### Acciones

* [[!UICONTROL Llamada de API personalizada]](#custom-api-call)
* [[!UICONTROL Dividir]](#get-split)
* [[!UICONTROL Obtener definición de división en entorno]](#get-split-definition-in-environment)
* [[!UICONTROL Crear división]](#create-split)
* [[!UICONTROL Eliminar división]](#delete-split)
* [[!UICONTROL Crear definición de división en entorno]](#create-split-definition-in-environment)
* [[!UICONTROL Eliminar definición dividida del entorno]](#remove-split-definition-from-environment)
* [[!UICONTROL Definición de división de actualización parcial en el entorno]](#partial-update-split-definition-in-environment)
* [[!UICONTROL Asociación de etiquetas]](#associate-tags)

#### [!UICONTROL Llamada de API personalizada]

Este módulo de acción le permite realizar una llamada autenticada personalizada al [!DNL split.io] API. De este modo, puede crear una automatización del flujo de datos que no se pueda lograr con la otra [!DNL split.io] módulos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Split.io] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Especifique una ruta relativa a <code>https://api.split.io/internal/api/v2/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada a la API. Para obtener más información, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p> <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion añade los encabezados de autorización por usted.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadena de consulta]</td> 
   <td> <p>Añada la consulta para la llamada de API en forma de objeto JSON estándar.</p> <p>Por ejemplo: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Al utilizar afirmaciones condicionales como <code>if</code> en su JSON, ponga las comillas fuera de la afirmación condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td>Introduzca o asigne el número máximo de registros con los que desea que funcione el módulo durante cada ciclo de ejecución del escenario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Dividir]

Este módulo de acción recupera la división.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Split.io] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Seleccione o asigne el espacio de trabajo que contiene la división que desea recuperar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Introduzca o asigne el nombre de la división que desea recuperar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener definición de división en entorno]

Este módulo de acción recupera una definición de división específica del entorno designado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Split.io] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Seleccione o asigne el espacio de trabajo que contiene la definición de división que desea recuperar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre o ID del entorno]</td> 
   <td>Seleccione o asigne el entorno que contiene la definición de división que desea recuperar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Introduzca o asigne el nombre de la división para la que desea recuperar la definición de división.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear división]

Este módulo de acción crea una nueva división en su organización, dado un tipo de tráfico.

>[!NOTE]
>
>La API no configura la división en ningún entorno.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Split.io] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Seleccione o asigne el espacio de trabajo donde desea crear la división.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de tráfico ID o nombre]</td> 
   <td>Seleccione o asigne el tipo de tráfico que desee utilizar para crear la división.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Introduzca o asigne un nombre para la división que desea crear.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descripción dividida]</td> 
   <td>Introduzca o asigne una descripción de [!UICONTROL split] para la división que desea crear.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar división]

Este módulo de acción elimina una división de su organización. Esto desconfigura automáticamente la definición de división de todos los entornos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Split.io] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Seleccione o asigne el espacio de trabajo donde desea eliminar la división.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Introduzca o asigne el nombre de la división que desea eliminar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear definición de división en entorno]

Este módulo de acción configura una definición dividida para un entorno específico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Split.io] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Seleccione o asigne el espacio de trabajo en el que desea crear una definición dividida.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre o ID del entorno]</td> 
   <td>Seleccione o asigne el entorno en el que desea crear una definición dividida.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Introduzca o asigne el nombre de la división para la que desea crear una definición.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comentarios]</td> 
   <td>Introduzca o asigne cualquier comentario que desee agregar a la definición de división.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Rules]</td> 
   <td> <p>Para cada regla de segmentación que desee agregar a la definición, haga clic en <b>[!UICONTROL Agregar elemento]</b>y, a continuación, introduzca o asigne la regla.</p> <p>Para obtener más información sobre las reglas de segmentación, consulte <a href="https://docs.split.io/reference#create-split-definition-in-environment">Crear una definición dividida en un entorno</a> en el [!DNL Split.io] documentación.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Regla predeterminada]</td> 
   <td> <p>Introduzca o asigne la regla que desea que utilice la división para el tráfico que no cumple las especificaciones del resto de reglas.</p> <p>Para obtener más información sobre las reglas de segmentación, consulte <a href="https://docs.split.io/reference#create-split-definition-in-environment">Crear una definición dividida en un entorno</a> en el [!DNL Split.io] documentación.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tratamiento predeterminado]</td> 
   <td> <p>Introduzca o asigne el tratamiento que desea que utilice la división si se elimina la división o si el cliente no está incluido en la asignación de tráfico.</p> <p>Para obtener más información sobre los tratamientos, consulte <a href="https://docs.split.io/reference#create-split-definition-in-environment">Crear una definición dividida en un entorno</a> en el [!DNL Split.io] documentación.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tratamientos]</td> 
   <td> <p>Para cada tratamiento que desee agregar a la definición, haga clic en <b>[!UICONTROL Agregar elemento]</b>y, a continuación, introduzca o asigne el tratamiento.</p> <p>Para obtener más información sobre los tratamientos, consulte <a href="https://docs.split.io/reference#create-split-definition-in-environment">Crear una definición dividida en un entorno</a> en el [!DNL Split.io] documentación.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar definición dividida del entorno]

Este módulo de acción desconfigura una definición dividida para un entorno específico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Split.io] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Seleccione o asigne el espacio de trabajo donde desea quitar una definición dividida.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre o ID del entorno]</td> 
   <td>Seleccione o asigne el entorno en el que desea eliminar una definición dividida.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Introduzca o asigne el nombre de la división para la que desea quitar una definición.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comentarios]</td> 
   <td>Introduzca o asigne cualquier comentario que desee agregar a la definición de división.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Definición de división de actualización parcial en el entorno]

Este módulo de acción actualiza una definición dividida para un entorno específico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Split.io] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Seleccione o asigne el espacio de trabajo donde desea actualizar una definición dividida.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre o ID del entorno]</td> 
   <td>Seleccione o asigne el entorno en el que desea actualizar una definición dividida.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Introduzca o asigne el nombre de la división para la que desea actualizar una definición.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Actualizar contenido]</td> 
   <td> <p>Para cada atributo de la división que desea actualizar, haga clic en <b>[!UICONTROL Agregar elemento]</b> e introduzca o asigne los cambios deseados.</p> <p>Para obtener más información, consulte <a href="https://docs.split.io/reference#partial-update-split-definition-in-environment">Definición de división de actualización parcial en el entorno</a> en el [!DNL Split.io] documentación.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comentarios]</td> 
   <td>Introduzca o asigne cualquier comentario que desee agregar a la definición de división.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Asociación de etiquetas]

Este módulo de acción agrega etiquetas al objeto especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Split.io] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Seleccione o asigne el espacio de trabajo donde desee añadir una etiqueta.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre de objeto]</td> 
   <td>Introduzca o asigne el nombre del objeto al que desea añadir etiquetas.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de objeto]</td> 
   <td> <p>Introduzca o asigne el tipo de objeto al que desea agregar etiquetas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Etiquetas]</td> 
   <td> <p>Para cada etiqueta que desee agregar, haga clic en <b>[!UICONTROL Agregar elemento]</b> y escriba o asigne la etiqueta .</p> </td> 
  </tr> 
 </tbody> 
</table>

### Búsquedas

* [[!UICONTROL Obtener espacios de trabajo]](#get-workspaces)
* [[!UICONTROL Obtener entornos]](#get-environments)
* [[!UICONTROL Obtener divisiones]](#get-splits)
* [[!UICONTROL Enumerar definiciones de división en un entorno]](#list-split-definitions-in-an-environment)
* [[!UICONTROL Obtener tipos de tráfico]](#get-traffic-types)

#### [!UICONTROL Obtener espacios de trabajo]

Este módulo de búsqueda recupera los espacios de trabajo de una organización.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Split.io] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td>Introduzca o asigne el número máximo de espacios de trabajo que desea que recupere el módulo durante cada ciclo de ejecución del escenario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener entornos]

Este módulo de búsqueda recupera una lista de entornos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Split.io] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Seleccione o asigne el espacio de trabajo que contiene los entornos que desea enumerar.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener divisiones]

Este módulo de búsqueda recupera una lista de divisiones.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Split.io] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Seleccione o asigne el espacio de trabajo que contiene las divisiones que desea enumerar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td>Introduzca o asigne el número máximo de divisiones que desea que recupere el módulo durante cada ciclo de ejecución del escenario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Enumerar definiciones de división en un entorno]

Este módulo de búsqueda recupera una lista de definiciones divididas en un entorno determinado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Split.io] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Seleccione o asigne el espacio de trabajo que contiene las definiciones de división que desea enumerar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre o ID del entorno]</td> 
   <td>Seleccione o asigne el entorno que contiene las definiciones de división que desea enumerar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td>Introduzca o asigne el número máximo de definiciones de división que desea que recupere el módulo durante cada ciclo de ejecución del escenario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener tipos de tráfico]

Este módulo de búsqueda recupera una lista de tipos de tráfico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Split.io] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Seleccione o asigne el espacio de trabajo que contiene los tipos de tráfico que desea enumerar.</td> 
  </tr> 
 </tbody> 
</table>
