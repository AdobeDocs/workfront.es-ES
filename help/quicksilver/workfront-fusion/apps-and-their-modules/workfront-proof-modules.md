---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: Módulos de prueba de Workfront
description: En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL Workfront Proof], así como conectarlo a varias aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion, Workfront Proof, Digital Content and Documents
exl-id: f5c6fb08-880d-4432-aef1-57db13b3ecdb
source-git-commit: a79c6b2fb2b651987f973bc0d74e0eeea312c5bc
workflow-type: tm+mt
source-wordcount: '2886'
ht-degree: 0%

---

# [!DNL Workfront Proof] módulos

En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL Workfront Proof], así como conectarlo a varias aplicaciones y servicios de terceros.

Esto resulta útil si necesita ejecutar tareas que actualmente no se admiten en pruebas en [!DNL Workfront] o [!DNL Workfront Proof], como actualizar pruebas en función de ciertos eventos y buscar los destinatarios de una prueba.

La variable [!DNL Workfront Proof] El conector no cuenta con el número de aplicaciones activas disponibles para su organización. Todos los escenarios, incluso si solo utilizan la variable [!DNL Workfront Proof] aplicación, haga un recuento con el recuento total de escenarios de su organización.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p>  <p>[!UICONTROL [!DNL Workfront Fusion] para la automatización del trabajo]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL Workfront Proof] módulos y sus campos

Al configurar [!DNL Workfront Proof] módulos, [!DNL Workfront Fusion] muestra los campos que se enumeran a continuación. Además de estos, se incluyen [!DNL Workfront Proof] pueden mostrarse los campos, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón de asignación encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Déclencheur](#triggers)
* [Acciones](#actions)
* [Búsquedas](#searches)

### Déclencheur

* [Pruebas de inspección](#watch-proofs)
* [Ver el resumen del PDF](#watch-for-pdf-summary)
* [[!UICONTROL Actividad de prueba de inspección]](#watch-proof-activity)

#### [!UICONTROL Pruebas de inspección]

Este módulo de déclencheur programado ejecuta un escenario cuando alguien crea o toma una decisión sobre una prueba.

El módulo devuelve una lista de todos los registros que encuentra durante el periodo especificado, junto con sus tipos. También devuelve los valores de los campos especificados. Si el módulo encuentra decisiones tomadas en la prueba, incluye tanto los valores anteriores como los actuales, en campos independientes. Puede asignar esta información en módulos posteriores en el escenario.

Esto ocurre en un intervalo programado regularmente que especifique.

Debe tener permisos suficientes para acceder a la prueba o pruebas en [!DNL Workfront Proof] para recuperar esta información.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Workfront Proof] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tipo de registro</td> 
   <td>Seleccione el tipo de [!DNL Workfront Proof] registre que desea que el módulo vea.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Salidas</td> 
   <td> <p>Seleccione la información que desee incluir en el paquete de salida para este módulo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Límite</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ver el resumen del PDF]

Este módulo de déclencheur instantáneo ejecuta un escenario cuando alguien crea un resumen de PDF para una prueba.

Se requiere un enlace web en este módulo.

El módulo devuelve todos los campos estándar asociados con la prueba, junto con los campos y valores personalizados a los que accede la conexión. También crea una nueva suscripción de evento para resúmenes de PDF y genera el contenido del atributo &quot;pdf_url&quot; enviado en la carga útil. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Workfront Proof] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Weblock]</td> 
   <td>Puede seleccionar un vínculo web existente o crear uno nuevo. Para obtener más información, consulte <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Déclencheur instantáneos (enlaces web) en [!DNL Adobe Workfront Fusion]</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Límite]</td> 
   <td>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actividad de prueba de inspección]

Este módulo de déclencheur ejecuta un escenario en el que se produce una actividad especificada en una prueba de prueba.

El módulo devuelve todos los campos estándar asociados con la prueba, junto con los campos y valores personalizados a los que accede la conexión. También crea una nueva suscripción de evento para los resúmenes de PDF y genera el contenido de la variable `pdf_url` enviado en la carga útil. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Workfront Proof] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de actividad]</td> 
   <td>Seleccione si desea ver cualquier nueva decisión (incluidos los cambios de estado de [!UICONTROL proof]) o solo los cambios de estado de prueba generales.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Límite]</td> 
   <td>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</td> 
  </tr> 
 </tbody> 
</table>

### Acciones

* [[!UICONTROL Crear revisión]](#create-proof)
* [[!UICONTROL Llamada de API personalizada]](#custom-api-call)
* [[!UICONTROL Descargar prueba]](#download-proof)
* [[!UICONTROL Leer un registro]](#read-a-record)
* [[!UICONTROL Resumen del PDF de solicitudes]](#request-pdf-summary)
* [[!UICONTROL Actualizar prueba]](#update-proof)
* [[!UICONTROL Cargar archivo]](#upload-file)

#### [!UICONTROL Crear revisión]

Este módulo de acción crea una nueva prueba o una nueva versión de una prueba en [!DNL Workfront Proof].

Especifique los parámetros para la nueva prueba y la prueba de origen si está creando una nueva versión.

El módulo devuelve el ID de la nueva versión de prueba o prueba. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Workfront Proof] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de prueba]</td> 
   <td> <p>Especifique si desea que la prueba que se ha creado tenga un flujo de trabajo básico o un [!UICONTROL Flujo de trabajo automatizado].</p> <p>A continuación, rellene los campos que se muestran para el tipo de prueba elegido. Por ejemplo, si elige [!UICONTROL Flujo de trabajo automatizado], rellene el <strong>[!UICONTROL Etapas del flujo de trabajo]</strong> para configurar las etapas.</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Permitir descargar el archivo original]</td> 
   <td>Seleccione si desea permitir que se descargue el archivo original desde el que se creó la prueba.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Classic Proof Viewer]</td> 
   <td>Seleccione si utiliza el visualizador de pruebas clásico.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Combinar todos los archivos en una sola prueba]</td> 
   <td>Active esta opción para combinar todos los archivos en una sola prueba de varias páginas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Crear una nueva versión de prueba]</td> 
   <td>Seleccione esta opción si desea que el módulo cree una nueva versión de una prueba existente. A continuación, en la variable <strong>[!UICONTROL ID de prueba existente]</strong> campo que muestra, asigna o introduce el ID exclusivo de la prueba.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Etiqueta de vínculo personalizado]</td> 
   <td>Introduzca o asigne una etiqueta para el vínculo de prueba personalizado.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL URL de vínculo personalizado]</td> 
   <td>Introduzca o asigne la dirección URL del vínculo personalizado.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Notificaciones de correo electrónico predeterminadas para suscriptores]</td> 
   <td>Escriba uno de los siguientes números para indicar cuál de las siguientes configuraciones de notificación de correo electrónico predeterminadas desea utilizar para la prueba que se crea.
    <ul>
     <li><strong>1</strong> - Todos los comentarios y respuestas nuevos</li>
     <li><strong>2</strong> - Respuestas a mis comentarios</li>
     <li><strong>3</strong> - Resumen diario</li>
     <li><strong>4</strong> - Resumen por hora</li>
     <li><strong>5</strong> - Solo decisiones</li>
     <li><strong>9</strong> - Desactivado</li>
    </ul></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Deshabilitar resumen de Excel]</td> 
   <td>Seleccione si desea deshabilitar la capacidad de descargar comentarios de prueba en un archivo de Excel.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Deshabilitar resumen de PDF]</td> 
   <td>Seleccione si desea deshabilitar la capacidad de descargar comentarios de prueba en un archivo PDF.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Deshabilitar correo electrónico de suscripción]</td> 
   <td>Seleccione si desea desactivar el correo electrónico de suscripción para esta prueba.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Habilitar el reproductor incrustado]</td> 
   <td>Seleccione si desea habilitar el reproductor incrustado para esta prueba.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Habilitar suscripciones]</td> 
   <td>Seleccione si las personas que no son participantes pueden suscribirse a la prueba.<br>Si selecciona esta opción, también puede seleccionar la Función predeterminada para suscriptores, tal como se describe en esta tabla.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Habilitar validación de suscripciones]</td> 
   <td>Seleccione si desea habilitar la validación del correo electrónico de suscripción. Si está habilitada, el suscriptor debe hacer clic en un vínculo de un correo electrónico para acceder a una prueba.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Habilitar URL de equipo]</td> 
   <td>Seleccione si desea que la prueba que se ha creado oculte o muestre la URL del equipo.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL File Hash] <span style="font-weight: normal;">o</span> [!UICONTROL File Hashes]</td> 
   <td>Añada el ID del archivo o archivos desde los que desea crear una o varias pruebas.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Nombres de archivo]</td> 
   <td>Añada el nombre o los nombres de archivo para la prueba que se crea Se trata de un campo obligatorio.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Bloquear prueba cuando se toman todas las decisiones necesarias]</td> 
   <td>Especifique si desea que la prueba que se crea se bloquee después de tomar todas las decisiones necesarias.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Notificar a los destinatarios sobre esta prueba]</td> 
   <td>Seleccione una opción para indicar si desea que se notifique a los destinatarios cuando se cree la prueba.&gt;</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof name]</td> 
   <td>Escriba un nombre para la prueba que se crea Este es un campo obligatorio. Utilice un símbolo de barra vertical (|) para separar nombres para varias pruebas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID del propietario de la prueba]</td> 
   <td>Introduzca o asigne el ID del propietario de la prueba. Si este campo se deja en blanco, el propietario de la prueba se establece en el usuario actual.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de referencia]</td> 
   <td>Introduzca el ID de referencia para la prueba.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Requiere firma electrónica]</td> 
   <td>Seleccione si desea exigir a una persona que tome una decisión sobre una prueba que envíe una firma electrónica.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Requiere inicio de sesión]</td> 
   <td> <p>Especifique si desea que la prueba que se crea requiera un inicio de sesión. </p> <p>Esto es igual al ajuste [!UICONTROL Login Required] que se explica en <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">[!UICONTROL Configurar la configuración de pruebas] en [!DNL Workfront Proof]</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID de resolución]</td> 
   <td>Introduzca el ID de la resolución que desea utilizar para la prueba. Para obtener una lista de ID de resolución, consulte la [!DNL Workfront Proof] <a href="http://api.proofhq.com/home/objects/soapworkflowproofobject">Documentación de API</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL SWF]</td> 
   <td>Introduzca el tipo de prueba del SWF.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Show] [item]</td> 
   <td>Para cada elemento, seleccione si desea mostrarlo en la prueba.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Workspace ID]</td> 
   <td>Introduzca el ID del espacio de trabajo en el que desea crear la prueba. </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Recipients]</td> 
   <td>Añada las direcciones de correo electrónico de los destinatarios que desee para la prueba que se crea .</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Plazo]</td> 
   <td> <p>Especifique la fecha límite que desee para la prueba que se crea. Utilice el siguiente formato de fecha:</p> <p><code>YYYY-MM-DD hh:mm</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Llamada de API personalizada]

Este módulo de acción le permite realizar una llamada autenticada personalizada al [!DNL Workfront Proof] API. De este modo, puede crear una automatización del flujo de datos que no se pueda lograr con la otra [!DNL Workfront Proof] módulos.

El módulo devuelve el código de estado, los encabezados y el cuerpo. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Workfront Proof] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Método]</td> 
   <td>Establezca la acción para la llamada de API. Para ver las acciones disponibles, consulte la <a href="http://api.proofhq.com/">Documentación de la API de prueba</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Body (XML)]</td> 
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Al utilizar afirmaciones condicionales como <code>if</code> en su JSON, ponga las comillas fuera de la afirmación condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Ejemplo:**
>
>![](assets/wfp-api-module-example-350x586.png)

#### [!UICONTROL Descargar prueba]

Este módulo de acción descarga el archivo de origen de una prueba concreta que se identifica con su ID.

Usted especifica el ID de la prueba.

El módulo devuelve el contenido del archivo de origen utilizado para crear la prueba. Puede asignar esta información en módulos posteriores en el escenario.

Debe tener permisos suficientes para acceder al registro en [!DNL Workfront Proof] para recuperar esta información.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Workfront Proof] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de prueba]</td> 
   <td> <p>Escriba el ID exclusivo de la prueba, que se encuentra en la página [!UICONTROL Proof Details]. Para obtener más información, consulte <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md" class="MCXref xref" data-mc-variable-override="">Administrar detalles de prueba en [!DNL Workfront Proof]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Leer un registro]

Este módulo de acción lee datos de una sola prueba en [!DNL Workfront Proof].

Especifique el ID de la prueba y la información que desea de ella.

El módulo devuelve los valores de los campos que elija para la prueba, junto con sus tipos. Puede asignar esta información en módulos posteriores en el escenario.

Debe tener permisos suficientes para acceder al registro en [!DNL Workfront Proof] para recuperar esta información.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Workfront Proof] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de registro]</td> 
   <td>Seleccione si desea leer una prueba, comentarios de prueba o revisores de prueba.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Salidas]</td> 
   <td> <p>Seleccione la información que desee incluir en el paquete de salida para este módulo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>Introduzca o asigne la variable única [!DNL Workfront Proof] ID del registro que desea que lea el módulo.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Resumen del PDF de solicitudes]

Este módulo de acción solicita el resumen del PDF para una prueba concreta en [!DNL Workfront Proof].

Usted especifica el ID de la prueba.

El módulo devuelve la información de resumen del PDF. Puede asignar esta información en módulos posteriores en el escenario.

Debe tener permisos suficientes para acceder al registro en [!DNL Workfront Proof] para recuperar esta información.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Workfront Proof] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de prueba]</td> 
   <td> <p>Escriba la variable única [!DNL Workfront Proof] ID de la prueba para la que desea solicitar un resumen del PDF.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Callback URL]</td> 
   <td>Introduzca o asigne la dirección URL a la que desea enviar el resumen del PDF.</td> 
  </tr> 
 </tbody> 
</table>

##### Posible error

* **Error**: &quot;[!UICONTROL No tiene privilegios para realizar esta solicitud. La fase debe contener al menos un destinatario.]&quot;
* **Solución**: Asegúrese de que no es el único asignado a las fases del flujo de trabajo. Debe haber otro usuario asignado a las fases del flujo de trabajo.

#### [!UICONTROL Actualizar prueba]

Este módulo de acción actualiza una prueba existente en [!DNL Workfront Proof].

Especifique el ID y el tipo de registro de la prueba y los campos que desea incluir en la salida.

El módulo devuelve todos los campos estándar asociados con el registro, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Debe tener permisos suficientes para acceder al registro en [!DNL Workfront Proof] para recuperar esta información.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Workfront Proof] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de prueba]</td> 
   <td> <p>Escriba el ID exclusivo de la prueba, que se encuentra en la página [!UICONTROL Proof Details]. Para obtener más información, consulte <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md" class="MCXref xref" data-mc-variable-override="">Administrar detalles de prueba en [!DNL Workfront Proof]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plazo]</td> 
   <td> <p>Especifique la fecha límite que desee para la prueba que se crea. Utilice el siguiente formato de fecha:</p> <p><code>YYYY-MM-DD hh:mm</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Notificaciones de correo electrónico predeterminadas para suscriptores]</td> 
   <td>Seleccione cuál de las siguientes opciones predeterminadas de notificación de correo electrónico desea utilizar para la prueba que se crea.
    <ul>
     <li> [!UICONTROL Todos los comentarios y respuestas nuevos]</li>
     <li>[!UICONTROL Respuestas a mis comentarios]</li>
     <li>[!UICONTROL Daily summary]</li>
     <li> [!UICONTROL Resumen por hora]</li>
     <li> [!UICONTROL Decisiones solamente]</li>
     <li> [!UICONTROL deshabilitado]</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Función predeterminada]</td> 
   <td>Seleccione la función predeterminada para la prueba.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Deshabilitar correo electrónico de suscripción]</td> 
   <td>Seleccione si desea desactivar el correo electrónico de suscripción para esta prueba.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Habilitar suscripciones]</td> 
   <td>Seleccione si las personas que no son participantes pueden suscribirse a la prueba.<br>Si selecciona esta opción, también puede seleccionar la [!UICONTROL Función predeterminada] para suscriptores, tal como se describe en esta tabla.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Habilitar validación de suscripciones]</td> 
   <td>Seleccione si desea habilitar la validación del correo electrónico de suscripción. Si está habilitada, el suscriptor debe hacer clic en un vínculo de un correo electrónico para acceder a una prueba.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Habilitar URL de equipo]</td> 
   <td>Seleccione si desea que la prueba que se ha creado oculte o muestre la URL del equipo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Bloquear prueba cuando se toman todas las decisiones necesarias]</td> 
   <td>Especifique si desea que la prueba que se crea se bloquee después de tomar todas las decisiones necesarias.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mensaje]</td> 
   <td>Introduzca o asigne un mensaje que desee adjuntar a la prueba.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de prueba] </td> 
   <td>Introduzca o asigne el ID de la prueba que desea actualizar.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre de prueba]</td> 
   <td>Introduzca o asigne el nombre de la prueba que desea actualizar.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Requiere inicio de sesión]</td> 
   <td> <p>Especifique si desea que la prueba que se crea requiera un inicio de sesión. </p> <p>Esto es igual al ajuste [!UICONTROL Login Required] que se explica en <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">[!UICONTROL Configurar la configuración de pruebas] en [!DNL Workfront Proof]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mostrar versiones como]</td> 
   <td>Seleccione si desea mostrar un vínculo a otras versiones de esta prueba.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Asunto]</td> 
   <td>Introduzca o asigne el asunto de la prueba</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Cargar archivo]

Este módulo de acción carga un archivo para utilizarlo con la variable [!UICONTROL Crear prueba] módulo en [!DNL Workfront Proof].

El módulo devuelve un ID de hash para el archivo cargado. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Workfront Proof] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Búsquedas

* [[!UICONTROL Buscar]](#search)
* [[!UICONTROL Enumerar plantillas de flujo de trabajo]](#list-workflow-templates)

#### [!UICONTROL Buscar]

Este módulo de búsqueda busca registros en un objeto de [!DNL Workfront Proof] que coinciden con la consulta de búsqueda especificada.

El módulo devuelve el ID de la prueba si está buscando una prueba. O bien, devuelve los ID de usuario, correos electrónicos, nombres, posiciones y alias de correo electrónico de los destinatarios, si está buscando destinatarios. Puede asignar esta información en módulos posteriores en el escenario.

Debe tener permisos suficientes para acceder al registro en [!DNL Workfront Proof] para recuperar esta información.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Workfront Proof] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Buscar</td> 
   <td> <p>Consulte[!UICONTROL ] Seleccione el tipo de registro que desea que busque el módulo.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Proof]</strong> </p> <p>Introduzca el Nombre de prueba de la prueba que desea buscar.</p> </li> 
     <li> <p><strong>[!UICONTROL Recipient]</strong> </p> <p>Introduzca la dirección de correo electrónico del destinatario que desea buscar.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Conjunto de resultados]</td> 
   <td>Indique si el módulo buscará <strong>[!UICONTROL Todos los registros coincidentes]</strong> o solo el <strong>[!UICONTROL Registro de primera coincidencia]</strong>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Ordenar por]</td> 
   <td>Seleccione el campo por el que desea ordenar los resultados.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Dirección de clasificación]</td> 
   <td> <p>Seleccione si desea ordenar los resultados de forma ascendente o descendente.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Enumerar plantillas de flujo de trabajo]

Este módulo de búsqueda enumera todas las plantillas de flujo de trabajo disponibles.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Workfront Proof] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Salidas]</td> 
   <td> <p>Seleccione la información que desee incluir en el paquete de salida para este módulo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de plantillas que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>
