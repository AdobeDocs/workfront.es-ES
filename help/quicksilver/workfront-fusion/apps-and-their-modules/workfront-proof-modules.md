---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de Workfront Proof
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion, Workfront Proof, Digital Content and Documents
exl-id: f5c6fb08-880d-4432-aef1-57db13b3ecdb
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '3230'
ht-degree: 91%

---

# Módulos de [!DNL Workfront Proof]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Módulos Workfront Proof](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-proof-modules.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

En un escenario de [!DNL Adobe Workfront Fusion], es posible automatizar los flujos de trabajo que utilizan [!DNL Workfront Proof], así como conectarlo a varias aplicaciones y servicios de terceros.

Esto es útil si necesita ejecutar tareas que actualmente no están soportadas en el sistema de pruebas dentro de [!DNL Workfront] o en [!DNL Workfront Proof], como actualizar pruebas basadas en ciertos eventos y buscar los destinatarios de una prueba.

El conector de [!DNL Workfront Proof] no cuenta para el número de aplicaciones activas disponibles para su organización. Todos los escenarios, incluso si solo usan la aplicación [!DNL Workfront Proof], no se contabilizan en el recuento total de escenarios de su organización.

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
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

## Información de Workfront Proof

El conector de Workfront Proof utiliza lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Versión de API</td> 
   <td> v21.3.0 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Etiqueta de API</td> 
   <td>Versión 1.8.92</td> 
  </tr>
 </tbody> 
 </table>

## Conectar [!DNL Workfront Proof] a [!DNL Workfront Fusion]

Puede crear una conexión con su cuenta de [!DNL Workfront Proof] directamente desde un módulo de [!DNL Workfront Fusion].

1. En cualquier módulo de [!DNL Workfront Fusion], haga clic en [!UICONTROL **Añadir**] junto al campo [!UICONTROL Conexión]

2. Rellene los campos siguientes:

   <table style="table-layout:auto"> 
        <col/>
        <col/>
        <tbody>
            <tr>
                <td role="rowheader">
                    <p role="rowheader">[!UICONTROL Connection name]</p>
                </td>
                <td>Introduzca un nombre para la conexión</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL connections.environmentType]</td>
                <td>Seleccione si este es un entorno de producción o un entorno no productivo, como Preview o Sandbox.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL connections.authenticationType]</td>
                <td>Seleccione si se trata de una cuenta de servicio o de una cuenta personal.</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Email / Username]</td>
                <td>Escriba el nombre de usuario de su cuenta de [!DNL Workfront Proof].</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Password]</td>
                <td>Escriba la contraseña de su cuenta de [!DNL Workfront Proof].</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Tenant ID]</td>
                <td><strong>Nota</strong>: Los clientes que no utilicen BYOK deben dejar este campo en blanco. <p>Introduzca el ID de entidad para esta cuenta. Si necesita ayuda para encontrar su ID de inquilino, póngase en contacto con Asistencia al cliente de Workfront.</p></td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Domain Extension]</td>
                <td>Introduzca la extensión de la URL que utiliza para acceder a su cuenta. <p>Ejemplo: <code>com</code> o <code>eu</code></p></td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Production, Preview, or Custom Environment]</td>
                <td>Seleccione una conexión a un entorno de producción, vista previa o personalizado.</td>
            </tr>
        </tbody>
    </table>


3. Haga clic en [!UICONTROL **Continuar**] para guardar la conexión y volver al módulo

## Módulos de [!DNL Workfront Proof] y sus campos

Al configurar módulos de [!DNL Workfront Proof], [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL Workfront Proof] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. El título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Activadores](#triggers)
* [Acciones](#actions)
* [Búsquedas](#searches)

### Activadores

* [Ver pruebas](#watch-proofs)
* [Ver el resumen del PDF](#watch-for-pdf-summary)
* [[!UICONTROL Ver la actividad de revisión]](#watch-proof-activity)

#### [!UICONTROL Ver pruebas]

Este módulo de activación programada ejecuta un escenario cuando alguien crea o toma una decisión sobre una prueba.

El módulo devuelve una lista de todos los registros que encuentra durante el período especificado, junto con sus tipos. También devuelve los valores de los campos especificados. Si el módulo ha encontrado decisiones tomadas sobre la prueba, incluye los valores anterior y actual en campos independientes. Puede asignar esta información en módulos subsiguientes en el escenario.

Esto sucede en un intervalo programado de forma regular que usted especifica.

Debe tener permisos suficientes para tener acceso a la revisión o revisiones en [!DNL Workfront Proof] a fin de recuperar esta información.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Workfront Proof] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tipo de registro</td> 
   <td>Seleccione el tipo de registro de [!DNL Workfront Proof] que desea que vea el módulo.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Salidas</td> 
   <td> <p>Seleccione la información que desea incluir en el paquete de salida para este módulo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Límite</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ver el resumen del PDF]

Este módulo de activación instantánea ejecuta un escenario cuando alguien crea un resumen PDF para una prueba.

Se requiere un webhook en este módulo.

El módulo devuelve todos los campos estándar asociados con la prueba, junto con los campos y valores personalizados a los que accede la conexión. También crea una nueva suscripción de eventos para resúmenes en PDF y genera el contenido del atributo pdf_url enviado en la carga útil. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Workfront Proof] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Webhook]</td> 
   <td>Puede seleccionar un webhook existente o crear uno nuevo. Para obtener más información, consulte <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Activadores instantáneos (webhooks) en [!DNL Adobe Workfront Fusion]</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución de escenario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ver actividad de la prueba]

Este módulo de activación ejecuta un escenario cuando ocurre una actividad específica en una prueba.

El módulo devuelve todos los campos estándar asociados con la prueba, junto con los campos y valores personalizados a los que accede la conexión. También crea una nueva suscripción de eventos para resúmenes en PDF y genera el contenido del atributo `pdf_url` enviado en la carga útil. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Workfront Proof] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Activity type]</td> 
   <td>Seleccione si desea ver cualquier nueva decisión (incluidos los cambios de estado de [!UICONTROL proof]) o solo los cambios de estado de prueba generales.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución de escenario.</td> 
  </tr> 
 </tbody> 
</table>

### Acciones

* [[!UICONTROL Crear prueba]](#create-proof)
* [[!UICONTROL Llamada de API personalizada]](#custom-api-call)
* [[!UICONTROL Descargar prueba]](#download-proof)
* [[!UICONTROL Leer un registro]](#read-a-record)
* [[!UICONTROL Solicitar resumen de PDF]](#request-pdf-summary)
* [[!UICONTROL Actualizar prueba]](#update-proof)
* [[!UICONTROL Cargar archivo]](#upload-file)

#### [!UICONTROL Crear prueba]

Este módulo de acción crea una nueva revisión o versión de una revisión en [!DNL Workfront Proof].

Especifique los parámetros para la nueva prueba y la prueba de origen si va a crear una nueva versión.

El módulo devuelve el ID de la nueva versión de prueba o revisión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Workfront Proof] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Type]</td> 
   <td> <p>Especifique si desea que la prueba creada tenga un flujo de trabajo básico o un [!UICONTROL Automated Workflow].</p> <p>A continuación, rellene los campos que se muestran para el tipo de prueba elegido. Por ejemplo, si elige [!UICONTROL Automated Workflow], rellene el campo <strong>[!UICONTROL Workflow Stages]</strong> para configurar las fases.</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Allow original file to be downloaded]</td> 
   <td>Seleccione si desea permitir la descarga del archivo original desde el que se creó la prueba.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Classic Proof Viewer]</td> 
   <td>Seleccione si está utilizando el visor de pruebas clásico.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Combine all files into single proof]</td> 
   <td>Habilite esta opción para combinar todos los archivos en una sola prueba de varias páginas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Create a new proof version]</td> 
   <td>Seleccione esta opción si desea que el módulo cree una nueva versión de una revisión existente. A continuación, en el campo <strong>[!UICONTROL Existing Proof ID]</strong> que se muestra, asigne o escriba el ID único de la prueba.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Link Label]</td> 
   <td>Introduzca o asigne una etiqueta para el vínculo de prueba personalizado.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Link URL]</td> 
   <td>Introduzca o asigne la URL para el enlace personalizado.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Default email notifications for subscribers]</td> 
   <td>Escriba uno de los siguientes números para indicar cuál de las siguientes configuraciones predeterminadas de notificación por correo electrónico desea usar para la prueba que se crea.
    <ul>
     <li><strong>1</strong> - Todos los comentarios y respuestas nuevos</li>
     <li><strong>2</strong> - Respuestas a mis comentarios</li>
     <li><strong>3</strong> - Resumen diario</li>
     <li><strong>4</strong> - Resumen por hora</li>
     <li><strong>5</strong> - Solo decisiones</li>
     <li><strong>9</strong> - Deshabilitado</li>
    </ul></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Disable Excel Summary]</td> 
   <td>Seleccione si desea deshabilitar la capacidad de descargar comentarios de revisión en un archivo de Excel.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Disable PDF Summary]</td> 
   <td>Seleccione si desea deshabilitar la capacidad de descargar comentarios de revisión en un archivo de PDF.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Disable Subscription Email]</td> 
   <td>Seleccione si desea desactivar el correo electrónico de suscripción para esta prueba.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Enable Embed Player]</td> 
   <td>Seleccione si desea habilitar el reproductor incrustado para esta prueba.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Enable Subscriptions]</td> 
   <td>Seleccione si se permite que las personas que no son participantes se suscriban a la prueba.<br>Si selecciona esta opción, también puede seleccionar el Rol predeterminado para los suscriptores, tal como se describe en esta tabla.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Enable Subscriptions Validation]</td> 
   <td>Seleccione si desea activar la validación del correo electrónico de suscripción. Si está activada, el suscriptor debe hacer clic en un vínculo de un correo electrónico para acceder a una prueba.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Enable Team URL]</td> 
   <td>Seleccione si desea que la prueba creada oculte o muestre la dirección URL del equipo.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL File Hash] <span style="font-weight: normal;">o</span> [!UICONTROL File Hashes]</td> 
   <td>Añada el ID del archivo o archivos de los que desea crear una prueba o pruebas.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL File Names]</td> 
   <td>Añada el nombre o los nombres de archivo para la prueba que se crea. Este campo es obligatorio.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Lock proof when all required decisions are made]</td> 
   <td>Especifique si desea que la prueba creada se bloquee después de que se tomen todas las decisiones requeridas.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Notify recipients about this proof]</td> 
   <td>Seleccione una opción para indicar si desea que los destinatarios sean notificados cuando se cree la prueba.&gt;</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof name]</td> 
   <td>Escriba un nombre para la prueba que se crea. Este campo es obligatorio. Utilice un símbolo de barra vertical (|) para separar los nombres de varias pruebas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof owner ID]</td> 
   <td>Introduzca o asigne el ID del propietario de la prueba. Si este campo se deja en blanco, el propietario de la prueba se establece en el usuario actual.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reference ID]</td> 
   <td>Introduzca el ID de referencia de la prueba.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Require electronic signature]</td> 
   <td>Seleccione si desea exigir que cualquiera que tome una decisión sobre una prueba envíe una firma electrónica.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Require login]</td> 
   <td> <p>Especifique si desea que la prueba creada requiera un inicio de sesión. </p> <p>Esto es lo mismo que la configuración de [!UICONTROL Login Required] explicada en <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">[!UICONTROL Configure Proof Settings] en [!DNL Workfront Proof]</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Resolution ID]</td> 
   <td>Introduzca el ID de la resolución que desea utilizar para la prueba. Para obtener una lista de los identificadores de resolución, consulte la [!DNL Workfront Proof] <a href="https://api.proofhq.com/home/objects/soapworkflowproofobject.html">documentación de API</a>.</td> 
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
   <td>Añada las direcciones de correo electrónico de los destinatarios que desee para la prueba creada .</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Deadline]</td> 
   <td> <p>Especifique la fecha límite que desea para la prueba que se ha creado. Utilice el siguiente formato de fecha:</p> <p><code>YYYY-MM-DD hh:mm</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Llamada de API personalizada]

Este módulo de acción le permite realizar una llamada autenticada personalizada a la API [!DNL Workfront Proof]. De este modo, puede crear una automatización del flujo de datos que no puedan realizar los otros [!DNL Workfront Proof] módulos.

El módulo devuelve el código de estado, los encabezados y el cuerpo. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Workfront Proof] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Method]</td> 
   <td>Establezca la acción para la llamada de API. Para ver las acciones disponibles, consulte la <a href="https://api.proofhq.com/">Documentación de la API de prueba</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Body (XML)]</td> 
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Cuando utilice afirmaciones condicionales como <code>if</code> en su JSON, coloque las comillas fuera de la afirmación condicional.</p> 
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

Este módulo de acción descarga el archivo de origen de una prueba concreta que identifica con su ID.

Especifique el ID de la prueba.

El módulo devuelve el contenido del archivo fuente utilizado para crear la prueba. Puede asignar esta información en módulos subsiguientes en el escenario.

Debe tener permisos suficientes para obtener acceso al registro de [!DNL Workfront Proof] a fin de recuperar esta información.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Workfront Proof] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof ID]</td> 
   <td> <p>Escriba el identificador único de la prueba, que se encuentra en la página [!UICONTROL Proof Details]. Para obtener más información, consulte <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md" class="MCXref xref" data-mc-variable-override="">Administrar detalles de revisión en [!DNL Workfront Proof]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Leer un registro]

Este módulo de acción lee datos de una sola revisión en [!DNL Workfront Proof].

Especifique el ID de la prueba y la información que desee de ella.

El módulo devuelve los valores de los campos que elija para la prueba, junto con sus tipos. Puede asignar esta información en módulos subsiguientes en el escenario.

Debe tener permisos suficientes para obtener acceso al registro de [!DNL Workfront Proof] a fin de recuperar esta información.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Workfront Proof] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td>Seleccione si desea leer una prueba, comentarios de prueba o revisores de prueba.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Outputs]</td> 
   <td> <p>Seleccione la información que desea incluir en el paquete de salida para este módulo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>Escriba o asigne el identificador único [!DNL Workfront Proof] del registro que desea que lea el módulo.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Solicitar resumen de PDF]

Este módulo de acción solicita el resumen del PDF para una revisión en particular en [!DNL Workfront Proof].

Especifique el ID de la prueba.

El módulo devuelve información resumida del PDF. Puede asignar esta información en módulos subsiguientes en el escenario.

Debe tener permisos suficientes para obtener acceso al registro de [!DNL Workfront Proof] a fin de recuperar esta información.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Workfront Proof] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof ID]</td> 
   <td> <p>Introduzca el identificador único [!DNL Workfront Proof] de la revisión para la cual desea solicitar un resumen de PDF.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Callback URL]</td> 
   <td>Introduzca o asigne la dirección URL a la que desea enviar el resumen del PDF.</td> 
  </tr> 
 </tbody> 
</table>

##### Posible error

* **Error**: “[!UICONTROL No cuenta con privilegios para realizar esta solicitud. La fase debe contener al menos un destinatario]”.
* **Solución**: asegúrese de que no es el único que está asignado a las fases del flujo de trabajo. Debe haber otro usuario asignado a las fases del flujo de trabajo.

#### [!UICONTROL Actualizar revisión]

Este módulo de acción actualiza una revisión existente en [!DNL Workfront Proof].

Especifique el ID de la prueba y el tipo de registro, así como los campos que desea incluir en la salida.

El módulo devuelve cualquier campo estándar asociado con el registro, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Debe tener permisos suficientes para obtener acceso al registro de [!DNL Workfront Proof] a fin de recuperar esta información.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Workfront Proof] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof ID]</td> 
   <td> <p>Escriba el identificador único de la prueba, que se encuentra en la página [!UICONTROL Proof Details]. Para obtener más información, consulte <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md" class="MCXref xref" data-mc-variable-override="">Administrar detalles de revisión en [!DNL Workfront Proof]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Deadline]</td> 
   <td> <p>Especifique la fecha límite que desea para la prueba que se ha creado. Utilice el siguiente formato de fecha:</p> <p><code>YYYY-MM-DD hh:mm</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Default email notifications for subscribers]</td> 
   <td>Seleccione cuál de las siguientes opciones predeterminadas de notificación por correo electrónico desea utilizar para la prueba que se crea.
    <ul>
     <li> [!UICONTROL All new comments and replies]</li>
     <li>[!UICONTROL Replies to my comments]</li>
     <li>[!UICONTROL Daily summary]</li>
     <li> [!UICONTROL Hourly summary]</li>
     <li> [!UICONTROL Decisions only]</li>
     <li> [!UICONTROL Disabled]</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Default Role]</td> 
   <td>Seleccione el rol predeterminado para la prueba.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Disable Subscription Email]</td> 
   <td>Seleccione si desea desactivar el correo electrónico de suscripción para esta prueba.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enable Subscriptions]</td> 
   <td>Seleccione si se permite que las personas que no son participantes se suscriban a la prueba.<br>Si selecciona esta opción, también puede seleccionar el [!UICONTROL Default Role] para los suscriptores, tal como se describe en esta tabla.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enable Subscriptions Validation]</td> 
   <td>Seleccione si desea activar la validación del correo electrónico de suscripción. Si está activada, el suscriptor debe hacer clic en un vínculo de un correo electrónico para acceder a una prueba.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enable Team URL]</td> 
   <td>Seleccione si desea que la prueba creada oculte o muestre la dirección URL del equipo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lock proof when all required decisions are made]</td> 
   <td>Especifique si desea que la prueba creada se bloquee después de que se tomen todas las decisiones requeridas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Message]</td> 
   <td>Introduzca o asigne un mensaje que desee que acompañe a la prueba.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof ID] </td> 
   <td>Introduzca o asigne el ID de la prueba que desea actualizar.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Name]</td> 
   <td>Introduzca o asigne el nombre de la prueba que desea actualizar.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Require login]</td> 
   <td> <p>Especifique si desea que la prueba creada requiera un inicio de sesión. </p> <p>Esto es lo mismo que la configuración [!UICONTROL Login Required] explicada en <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">[!UICONTROL Configure Proof Settings] en [!DNL Workfront Proof]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Show Versions Like]</td> 
   <td>Seleccione si desea mostrar un vínculo a otras versiones de esta revisión.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subject]</td> 
   <td>Introduzca o asigne el asunto de la prueba</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Cargar archivo]

Este módulo de acción carga un archivo para utilizarlo con el módulo [!UICONTROL Crear revisión] en [!DNL Workfront Proof].

El módulo devuelve un ID de hash para el archivo cargado. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Workfront Proof] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source file]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Búsquedas

* [[!UICONTROL Plantillas de flujo de trabajo de pruebas]](#list-workflow-templates)
* [[!UICONTROL Búsqueda]](#search)

#### [!UICONTROL Plantillas de flujo de trabajo de pruebas]

Este módulo de búsqueda enumera todas las plantillas de flujo de trabajo disponibles.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL Workfront Proof] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Outputs]</td> 
   <td> <p>Seleccione la información que desea incluir en el paquete de salida para este módulo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p>Introduzca o asigne el número máximo de plantillas que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Búsqueda]

Este módulo de búsqueda busca registros en un objeto de [!DNL Workfront Proof] que coincidan con la consulta de búsqueda especificada.

El módulo devuelve el ID de la prueba si está buscando una prueba. También devuelve los ID de usuario, los correos electrónicos, los nombres, las posiciones y los alias de correo electrónico de los destinatarios, si está buscando destinatarios. Puede asignar esta información en módulos subsiguientes en el escenario.

Debe tener permisos suficientes para obtener acceso al registro de [!DNL Workfront Proof] a fin de recuperar esta información.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Workfront Proof] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Buscar</td> 
   <td> <p>[!UICONTROL ]Seleccione el tipo de registro que desea que busque el módulo.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Proof]</strong> </p> <p>Introduzca el Nombre de la revisión que desea buscar.</p> </li> 
     <li> <p><strong>[!UICONTROL Recipient]</strong> </p> <p>Introduzca la dirección de correo electrónico del destinatario que desea buscar.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Result Set]</td> 
   <td>Indique si el módulo buscará <strong>[!UICONTROL All Matching Records]</strong> o solo el <strong>[!UICONTROL First Matching Record]</strong>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Sort By]</td> 
   <td>Seleccione el campo por el que desea ordenar los resultados.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Sorting Direction]</td> 
   <td> <p>Seleccione si desea ordenar los resultados de forma ascendente o descendente.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listar plantillas de flujo de trabajo]

Este módulo de búsqueda enumera todas las plantillas de flujo de trabajo disponibles.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Workfront Proof] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Outputs]</td> 
   <td> <p>Seleccione la información que desea incluir en el paquete de salida para este módulo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p>Introduzca o asigne el número máximo de plantillas que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>
