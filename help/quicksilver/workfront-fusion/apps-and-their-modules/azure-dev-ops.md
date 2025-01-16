---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de Azure DevOps
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: ecaa93c9-47bb-4fe1-87b4-d2e117cc68ae
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1845'
ht-degree: 93%

---

# Módulos de [!DNL Azure DevOps]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Módulos DevOps de Azure](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/azure-dev-ops.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

En un escenario de [!DNL Adobe Workfront Fusion], puede automatizar los flujos de trabajo que utilizan [!DNL Azure DevOps], así como conectarlo a varias aplicaciones y servicios de terceros.

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

Para usar módulos de [!DNL Azure DevOps], debe tener una cuenta de DevOps de [!DNL Azure].

## Información de la API [!DNL Azure DevOps]

El conector de Azure DevOps utiliza lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Versión de API</td> 
   <td> Versión 5.1 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Etiqueta de API</td> 
   <td>Versión 1.29.33</td> 
  </tr>
 </tbody> 
</table>

## Conectar [!DNL Azure DevOps] a [!DNL Workfront Fusion] {#connect-azure-devops-to-workfront-fusion}

1. Añada un módulo de [!DNL Azure DevOps] a su escenario.
1. Haga clic en **[!UICONTROL Añadir]** junto al campo [!UICONTROL conexión].
1. En el campo [!UICONTROL Tipo de conexión], seleccione **[!DNL Azure DevOps]**.

   >[!IMPORTANT]
   >
   >El tipo de conexión [!UICONTROL [!DNL Azure DevOps] (Request All Scopes)] quedará obsoleto en un futuro próximo. Por lo tanto, no se recomienda su uso.

1. Rellene los campos siguientes:

   <table style="table-layout:auto">
        <tr>
            <td>[!UICONTROL Connection name]</td>
            <td>Introduzca un nombre para la conexión que está creando.</td>
        </tr>
      <tr>
            <td>[!UICONTROL Organization]</td>
            <td>Introduzca el nombre de la organización en la que ha creado la aplicación [!DNL Azure DevOps].</td>
        </tr>
    </table>

1. Haga clic en **[!UICONTROL Continuar]** para finalizar la configuración de la conexión y continuar creando el escenario.

## Módulos de [!UICONTROL Azure DevOps] y sus campos

Al configurar los módulos de [!DNL Azure DevOps], [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL Azure DevOps] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. El título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Activadores](#triggers)
* [Acciones](#actions)
* [Búsquedas](#searches)

### Activadores

#### [!UICONTROL Ver elementos de trabajo]

Este módulo de activador instantáneo ejecuta un escenario cuando se añade, actualiza o elimina un registro en [!UICONTROL Azure DevOps].

El módulo devuelve cualquier campo estándar asociado con el registro, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Seleccione o añada un webhook para el módulo.</p> <p>Para obtener más información sobre los webhooks en los módulos de activador, consulte <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Activadores instantáneos (webhooks) en [!DNL Adobe Workfront Fusion]</a>.</p> <p>Para obtener información sobre cómo crear un webhook, consulte <a href="../../workfront-fusion/apps-and-their-modules/webhooks-updated.md" class="MCXref xref">Webhooks</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Acciones

* [Crear un registro](#create-a-record)
* [Llamada de API personalizada](#custom-api-call)
* [Descargar un archivo adjunto](#download-an-attachment)
* [Vincular elementos de trabajo](#link-work-items)
* [Leer registro](#read-record)
* [Actualizar un elemento de trabajo](#update-a-work-item)
* [[!UICONTROL Cargar un archivo adjunto]](#upload-an-attachment)

#### [!UICONTROL Llamada de API personalizada]

Este módulo de acción le permite realizar una llamada autenticada personalizada a la API [!DNL Azure DevOps]. De este modo, puede crear una automatización del flujo de datos imposibles de realizar por los otros [!DNL Azure DevOps] módulos.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL Azure DevOps] a [!DNL Workfront Fusion], consulte <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Azure DevOps] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Base URL]</td> 
   <td> <p>Seleccione o asigne la dirección URL base que utiliza para conectarse a su cuenta de [!DNL Azure DevOps]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Relative URL]</td> 
   <td> <p>Introduzca la dirección URL relativa a la que desea conectarse para esta llamada de API.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>{organization}/_apis[/{area}]/{resource}</code> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL API Version]</td> 
   <td>Seleccione o asigne la versión de la API de [!DNL Azure DevOps] a la que desee conectarse para esta llamada de API. Si no se ha seleccionado ninguna versión, [!DNL Workfront Fusion] se conecta a la versión 5.1 de la API de [!DNL Azure DevOps].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Seleccione el método de petición HTTP que necesita para configurar la llamada de la API. Para obtener más información, vea <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de petición HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p> <p>Por ejemplo: <code>{"Content-type":"application/json"}</code></p> </td> 
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

#### [!UICONTROL Crear un registro]

Este módulo de acción crea un nuevo proyecto o elemento de trabajo.

El módulo genera el ID de objeto para el elemento de trabajo recién creado o la URL y el código de estado de un proyecto recién creado.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL Azure DevOps] a [!DNL Workfront Fusion], consulte <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Azure DevOps] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td> <p>Seleccione si desea crear un elemento de trabajo o un proyecto.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Project]</strong> </p> <p>Rellene los campos siguientes:</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Name]</strong>: escriba o asigne un nombre para el nuevo proyecto.</p> </li> 
       <li> <p><strong>[!UICONTROL Description]</strong>: escriba o asigne una descripción para el nuevo proyecto. </p> </li> 
       <li> <p><strong>[!UICONTROL Visibility]</strong>: seleccione si desea que el proyecto sea público o privado. Para poder interactuar con un proyecto privado, los usuarios deben haber iniciado sesión en su organización y se les debe haber concedido acceso al proyecto. Los proyectos públicos son visibles para los usuarios que no han iniciado sesión en su organización.</p> </li> 
       <li> <p><strong>[!UICONTROL Version control]</strong>: seleccione si desea que el proyecto use [!DNL Git] o [!UICONTROL Team Foundation Version Control (TFCV)] para el control de versiones.</p> </li> 
       <li> <p><strong>[!UICONTROL Work item process]</strong>: seleccione el proceso de trabajo que desee utilizar para el proyecto. Las opciones son [!UICONTROL Basic], [!UICONTROL Scrum], [!UICONTROL Capability Maturity Model Integration (CMMI)] y [!UICONTROL Agile].</p> <p>Para obtener más información sobre los procesos de [!DNL Azure DevOps], consulte <a href="https://docs.microsoft.com/en-us/azure/devops/boards/work-items/guidance/choose-process?view=azure-devops&amp;tabs=basic-process">Elegir un proceso</a> en la documentación de [!DNL Azure DevOps].</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Work item]</strong> </p> <p>Rellene los campos siguientes:</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Project]</strong>: seleccione el proyecto donde desea crear el elemento de trabajo.</p> </li> 
       <li> <p><strong>[!UICONTROL Work item type]</strong>: seleccione el tipo de elemento de trabajo que desea crear.</p> </li> 
       <li> <p><strong>[!UICONTROL Other fields]</strong>: en estos campos, escriba el valor que desea que tenga el elemento de trabajo para una propiedad determinada. Los campos disponibles dependen del tipo de elemento de trabajo.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Descargar un archivo adjunto]

Este módulo de acción descarga un archivo adjunto.

El módulo devuelve el contenido del archivo adjunto.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre la conexión de su cuenta de [!DNL Azure DevOps] a [!DNL Workfront Fusion], consulte <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Azure DevOps] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Attachment URL]</td> 
   <td> <p>Introduzca o asigne la dirección URL del archivo adjunto que desea descargar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Vincular elementos de trabajo]

Este módulo de acción vincula dos elementos de trabajo y define la relación entre ellos.

El módulo devuelve el ID del elemento de trabajo principal y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre la conexión de su cuenta de [!DNL Azure DevOps] a [!DNL Workfront Fusion], consulte <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Azure DevOps] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Work item ID]</td> 
   <td>Escriba o asigne el identificador del elemento de trabajo principal al que desee vincular otro elemento de trabajo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Linked work item ID]</td> 
   <td>Introduzca o asigne el ID del elemento de trabajo que desee vincular al elemento de trabajo principal.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Link Type]</td> 
   <td> <p>Defina la relación entre los elementos de trabajo que desea vincular.</p> <p>Para obtener más información, consulte <a href="https://docs.microsoft.com/es-es/azure/devops/boards/queries/link-type-reference?view=azure-devops">Referencia de tipo de vínculo</a> en la documentación de [!UICONTROL Azure DevOps].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comment]</td> 
   <td>Escriba o asigne el texto de un comentario. Esto resulta útil para explicar el razonamiento o la intención del vínculo.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Leer registro]

Este módulo de acción lee datos de un único registro en [!DNL Azure DevOps].

Especifique el identificador del registro.

El módulo devuelve el ID del registro y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL Azure DevOps] a [!DNL Workfront Fusion], consulte <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Azure DevOps] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td> <p>Seleccione si desea leer un proyecto o un elemento de trabajo</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Project]</strong>: seleccione el proyecto que desea leer.</p> </li> 
     <li> <p><strong>[!UICONTROL Work item]</strong>: seleccione el proyecto que contiene el elemento de trabajo que desea leer y, a continuación, seleccione el tipo de elemento de trabajo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Seleccione la información que desea incluir en el paquete de salida para este módulo. Los campos disponibles dependen del tipo de elemento de trabajo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Introduzca o asigne el ID del registro que desea leer.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actualizar un elemento de trabajo]

Este módulo de acción actualiza un elemento de trabajo existente mediante su ID.

El módulo devuelve el ID del elemento de trabajo actualizado.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL Azure DevOps] a [!DNL Workfront Fusion], consulte <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Azure DevOps] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project]</td> 
   <td>Seleccione el proyecto que contiene el elemento de trabajo que desea actualizar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Work Item Type]</td> 
   <td> <p>Seleccione el tipo de elemento de trabajo que desea actualizar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Other Fields]</td> 
   <td>En cada uno de estos campos, introduzca el valor que desea que tenga el elemento de trabajo para una propiedad determinada. Los campos disponibles dependen del tipo de elemento de trabajo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Work item ID]</td> 
   <td>Escriba o asigne el ID del elemento de trabajo que desea actualizar.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Cargar un archivo adjunto]

Este módulo de acción carga un archivo y lo adjunta a un elemento de trabajo.

El módulo devuelve el ID de archivo adjunto y una URL de descarga para el archivo adjunto.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL Azure DevOps] a [!DNL Workfront Fusion], consulte <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Azure DevOps] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project] </td> 
   <td> <p>Seleccione el proyecto en el que desea cargar un archivo adjunto.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Work item ID]</td> 
   <td> <p>Introduzca o asigne el ID del elemento de trabajo en el que desea cargar un archivo adjunto.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comment]</td> 
   <td>Escriba el texto del comentario que desee añadir al archivo adjunto cargado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file] </td> 
   <td>Seleccione un archivo de origen de un módulo anterior o introduzca o asigne el nombre y el contenido del archivo de origen.</td> 
  </tr> 
 </tbody> 
</table>

### Búsquedas

#### [!UICONTROL Lista de elementos de trabajo]

Este módulo de acción recupera todos los elementos de trabajo de un tipo específico en un proyecto de [!DNL Azure DevOps].

El módulo devuelve el ID del elemento de trabajo principal y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL Azure DevOps] a [!DNL Workfront Fusion], consulte <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Azure DevOps] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project]</td> 
   <td>Seleccione el proyecto cuyos elementos de trabajo desea recuperar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Work item type]</td> 
   <td> <p>Seleccione el tipo de elemento de trabajo que desea recuperar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Seleccione las propiedades que desea que aparezcan en la salida del módulo. Los campos disponibles dependen del tipo de elemento de trabajo que desee recuperar. Debe seleccionar al menos una propiedad.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Escriba o asigne el número máximo de elementos de trabajo que [!DNL Workfront Fusion] devuelve durante un ciclo de ejecución.</td> 
  </tr> 
 </tbody> 
</table>
