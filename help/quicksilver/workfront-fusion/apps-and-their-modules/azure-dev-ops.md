---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de Azure DevOps
description: En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL Azure DevOps], así como conectarlo a múltiples aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion
exl-id: ecaa93c9-47bb-4fe1-87b4-d2e117cc68ae
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1797'
ht-degree: 0%

---

# [!DNL Azure DevOps] módulos

En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL Azure DevOps], así como conectarlo a múltiples aplicaciones y servicios de terceros.

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

Para usar [!DNL Azure DevOps] módulos, debe tener un [!DNL Azure] Cuenta de DevOps.

## Connect [!DNL Azure DevOps] hasta [!DNL Workfront Fusion] {#connect-azure-devops-to-workfront-fusion}

1. Añadir un [!DNL Azure DevOps] a su escenario.
1. Clic **[!UICONTROL Añadir]** junto al [!UICONTROL Conexión] field.
1. En el [!UICONTROL Tipo de conexión] , seleccione **[!DNL Azure DevOps]**.

   >[!IMPORTANT]
   >
   >El [!UICONTROL [!DNL Azure DevOps] (Solicitar todos los ámbitos)] el tipo de conexión quedará obsoleta en un futuro próximo. Por lo tanto, no se recomienda su uso.

1. Rellene los campos siguientes:

   <table style="table-layout:auto">
        <tr>
            <td>[!UICONTROL Nombre de conexión]</td>
            <td>Escriba un nombre para la conexión que está creando.</td>
        </tr>
      <tr>
            <td>[!UICONTROL Organización]</td>
            <td>Introduzca el nombre de la organización en la que creó su [!DNL Azure DevOps] aplicación.</td>
        </tr>
    </table>

1. Clic **[!UICONTROL Continuar]** para finalizar la configuración de la conexión y continuar creando el escenario.

## [!UICONTROL Azure DevOps] módulos y sus campos

Al configurar [!DNL Azure DevOps] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, se añaden [!DNL Azure DevOps] Los campos pueden mostrarse, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignación de información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Déclencheur](#triggers)
* [Acciones](#actions)
* [Búsquedas](#searches)

### Déclencheur

#### [!UICONTROL Buscar elementos de trabajo]

Este módulo de déclencheur instantáneo ejecuta un escenario cuando se agrega, actualiza o elimina un registro en [!UICONTROL Azure DevOps].

El módulo devuelve cualquier campo estándar asociado con el registro, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Seleccione o agregue un webhook para el módulo.</p> <p>Para obtener más información sobre los webhooks en los módulos de déclencheur, consulte <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Déclencheur instantáneos (webhooks) en [!DNL Adobe Workfront Fusion]</a>.</p> <p>Para obtener información sobre cómo crear un webhook, consulte <a href="../../workfront-fusion/apps-and-their-modules/webhooks-updated.md" class="MCXref xref">Webhooks</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Acciones

* [Llamada de API personalizada](#custom-api-call)
* [Leer registro](#read-record)
* [Creación de un registro](#create-a-record)
* [Actualizar un elemento de trabajo](#update-a-work-item)
* [[!UICONTROL Cargar un archivo adjunto]](#upload-an-attachment)
* [Descargar un archivo adjunto](#download-an-attachment)
* [Vincular elementos de trabajo]([!UICONTROL #link-work-items])

#### [!UICONTROL Llamada de API personalizada]

Este módulo de acción le permite realizar una llamada autenticada personalizada a [!DNL Azure DevOps] API. De este modo, se puede crear una automatización del flujo de datos que el otro no puede realizar [!DNL Azure DevOps] módulos.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Azure DevOps] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL base]</td> 
   <td> <p>Seleccione o asigne la dirección URL base que utiliza para conectarse a su [!DNL Azure DevOps] account</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL relativa]</td> 
   <td> <p>Introduzca la dirección URL relativa a la que desea conectarse para esta llamada de API.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>{organization}/_apis[/{area}]/{resource}</code> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL API Version]</td> 
   <td>Seleccione o asigne la versión de [!DNL Azure DevOps] API a la que desea conectarse para esta llamada de API. Si no se selecciona ninguna versión, [!DNL Workfront Fusion] se conecta a [!DNL Azure DevOps] Versión de API 5.1.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada de API. Para obtener más información, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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

#### [!UICONTROL Leer registro]

Este módulo de acción lee datos de un único registro en [!DNL Azure DevOps].

Especifique el ID del registro.

El módulo devuelve el ID del registro y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Azure DevOps] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione si desea leer un proyecto o un elemento de trabajo</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Proyecto]</strong>: seleccione el proyecto que desea leer.</p> </li> 
     <li> <p><strong>[!UICONTROL Elemento de trabajo]</strong>: seleccione el proyecto que contiene el elemento de trabajo que desea leer y, a continuación, seleccione el tipo de elemento de trabajo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salidas]</td> 
   <td>Seleccione la información que desee incluir en el paquete de salida para este módulo. Los campos disponibles dependen del tipo de elemento de trabajo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Introduzca o asigne el ID del registro que desea leer.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Creación de un registro]

Este módulo de acción crea un nuevo proyecto o elemento de trabajo.

El módulo genera el ID de objeto para el elemento de trabajo recién creado o la URL y el código de estado de un proyecto recién creado.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Azure DevOps] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione si desea crear un elemento de trabajo o un proyecto.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Proyecto]</strong> </p> <p>Rellene los campos siguientes:</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Nombre]</strong>: introduzca o asigne un nombre para el nuevo proyecto.</p> </li> 
       <li> <p><strong>[!UICONTROL Descripción]</strong>: introduzca o asigne una descripción para el nuevo proyecto. </p> </li> 
       <li> <p><strong>[!UICONTROL Visibilidad]</strong>: seleccione si desea que el proyecto sea público o privado. Los usuarios deben haber iniciado sesión en su organización y se les debe haber concedido acceso al proyecto para interactuar con un proyecto privado. Los proyectos públicos son visibles para los usuarios que no han iniciado sesión en su organización.</p> </li> 
       <li> <p><strong>[!UICONTROL Control de versiones]</strong>: seleccione si desea que el proyecto utilice [!DNL Git] o [!UICONTROL Control de versiones de Team Foundation (TFCV)] para el control de versiones.</p> </li> 
       <li> <p><strong>[!UICONTROL Proceso de elemento de trabajo]</strong>: seleccione el proceso de trabajo que desea utilizar para el proyecto. Las opciones son [!UICONTROL Basic], [!UICONTROL Scrum], [!UICONTROL Capability Maturity Model Integration (CMMI)] y [!UICONTROL Agile].</p> <p>Para obtener más información sobre [!DNL Azure DevOps] procesos, consulte <a href="https://docs.microsoft.com/en-us/azure/devops/boards/work-items/guidance/choose-process?view=azure-devops&amp;tabs=basic-process">Elegir un proceso</a> en el [!DNL Azure DevOps] Documentación.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Elemento de trabajo]</strong> </p> <p>Rellene los campos siguientes:</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Proyecto]</strong>: seleccione el proyecto donde desea crear el elemento de trabajo.</p> </li> 
       <li> <p><strong>[!UICONTROL Tipo de elemento de trabajo]</strong>: seleccione el tipo de elemento de trabajo que desea crear.</p> </li> 
       <li> <p><strong>[!UICONTROL Otros campos]</strong>: en estos campos, introduzca el valor que desea que tenga el elemento de trabajo para una propiedad determinada. Los campos disponibles dependen del tipo de elemento de trabajo.</p> </li> 
      </ul> </li> 
    </ul> </td> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Azure DevOps] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Proyecto]</td> 
   <td>Seleccione el proyecto que contiene el elemento de trabajo que desea actualizar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de elemento de trabajo]</td> 
   <td> <p>Seleccione el tipo de elemento de trabajo que desea actualizar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Otros campos]</td> 
   <td>En cada uno de estos campos, introduzca el valor que desea que tenga el elemento de trabajo para una propiedad determinada. Los campos disponibles dependen del tipo de elemento de trabajo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. elemento de trabajo]</td> 
   <td>Escriba o asigne el identificador del elemento de trabajo que desea actualizar.</td> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Azure DevOps] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Proyecto] </td> 
   <td> <p>Seleccione el proyecto en el que desea cargar un archivo adjunto.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. elemento de trabajo]</td> 
   <td> <p>Introduzca o asigne el ID del elemento de trabajo en el que desea cargar un archivo adjunto.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comentario]</td> 
   <td>Escriba el texto del comentario que desee agregar al archivo adjunto cargado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen] </td> 
   <td>Seleccione un archivo de origen de un módulo anterior o introduzca o asigne el nombre y el contenido del archivo de origen.</td> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Azure DevOps] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL de datos adjuntos]</td> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Azure DevOps] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. elemento de trabajo]</td> 
   <td>Escriba o asigne el identificador del elemento de trabajo principal al que desea vincular otro elemento de trabajo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de elemento de trabajo vinculado]</td> 
   <td>Introduzca o asigne el ID del elemento de trabajo que desea vincular al elemento de trabajo principal.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de vínculo]</td> 
   <td> <p>Defina la relación entre los elementos de trabajo que desea vincular.</p> <p>Para obtener más información, consulte <a href="https://docs.microsoft.com/en-us/azure/devops/boards/queries/link-type-reference?view=azure-devops">Referencia de tipo de vínculo</a> en la documentación de [!UICONTROL Azure DevOps].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comentario]</td> 
   <td>Escriba o asigne el texto de un comentario. Esto resulta útil para explicar el razonamiento o la intención del vínculo.</td> 
  </tr> 
 </tbody> 
</table>

### Búsquedas

#### [!UICONTROL Lista de elementos de trabajo]

Este módulo de acción recupera todos los elementos de trabajo de un tipo específico en una [!DNL Azure DevOps] proyecto.

El módulo devuelve el ID del elemento de trabajo principal y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Azure DevOps] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Proyecto]</td> 
   <td>Seleccione el proyecto del que desea recuperar elementos de trabajo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de elemento de trabajo]</td> 
   <td> <p>Seleccione el tipo de elemento de trabajo que desea recuperar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salidas]</td> 
   <td>Seleccione las propiedades que desea que aparezcan en la salida del módulo. Los campos disponibles dependen del tipo de elemento de trabajo que desee recuperar. Debe seleccionar al menos una propiedad.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td>Especifique o asigne el número máximo de elementos de trabajo que [!DNL Workfront Fusion] devuelve durante un ciclo de ejecución.</td> 
  </tr> 
 </tbody> 
</table>
