---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de Workfront Proof
description: En un  [!DNL Adobe Workfront Fusion] escenario, puede automatizar los flujos de trabajo que usan [!DNL Workfront Proof], así como conectarlo a varias aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion, Workfront Proof, Digital Content and Documents
exl-id: f5c6fb08-880d-4432-aef1-57db13b3ecdb
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '3176'
ht-degree: 0%

---

# [!DNL Workfront Proof] módulos

En un escenario de [!DNL Adobe Workfront Fusion], puede automatizar los flujos de trabajo que utilizan [!DNL Workfront Proof], así como conectarlo a varias aplicaciones y servicios de terceros.

Esto resulta útil si necesita ejecutar tareas que actualmente no se admiten en la revisión en [!DNL Workfront] o en [!DNL Workfront Proof], como actualizar revisiones basadas en ciertos eventos y buscar los destinatarios de una revisión.

El conector [!DNL Workfront Proof] no cuenta con respecto al número de aplicaciones activas disponibles para su organización. Todos los escenarios, incluso si solo usan la aplicación [!DNL Workfront Proof], no se contabilizan en el recuento total de escenarios de su organización.

Si necesita instrucciones para crear un escenario, consulte [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obtener información acerca de los módulos, vea [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <p>Requisito de licencia actual: no se requiere licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo], [!UICONTROL [!DNL Workfront Fusion] para automatización de trabajo]</p>
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

1. En cualquier módulo de [!DNL Workfront Fusion], haga clic en [!UICONTROL **Agregar**] junto al campo [!UICONTROL Conexión]

2. Rellene los campos siguientes:

   <table style="table-layout:auto"> 
        <col/>
        <col/>
        <tbody>
            <tr>
                <td role="rowheader">
                    <p role="rowheader">[!UICONTROL Nombre de conexión]</p>
                </td>
                <td>Escriba un nombre para la conexión</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL connections.environmentType]</td>
                <td>Seleccione si es un entorno de producción o un entorno que no sea de producción, como una vista previa o una zona protegida.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL connections.authenticationType]</td>
                <td>Seleccione si se trata de una cuenta de servicio o de una cuenta personal.</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Correo electrónico / Nombre de usuario]</td>
                <td>Escriba el nombre de usuario de su cuenta de [!DNL Workfront Proof].</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Contraseña]</td>
                <td>Escriba la contraseña de su cuenta de [!DNL Workfront Proof].</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL ID de inquilino]</td>
                <td><strong>Nota</strong>: Los clientes que no usen BYOK deben dejar este campo en blanco. <p>Introduzca el ID de inquilino de esta cuenta. Si necesita ayuda para encontrar su ID de inquilino, póngase en contacto con Asistencia al cliente de Workfront.</p></td>
            </tr>
            <tr>
                <td role="rowheader">Extensión de dominio de [!UICONTROL]</td>
                <td>Introduzca la extensión de la URL que utiliza para acceder a su cuenta. <p>Ejemplo: <code>com</code> o <code>eu</code></p></td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Producción, Vista previa o Entorno personalizado]</td>
                <td>Seleccione una conexión a un entorno de producción, vista previa o personalizado.</td>
            </tr>
        </tbody>
    </table>


3. Haga clic en [!UICONTROL **Continuar**] para guardar la conexión y volver al módulo

## [!DNL Workfront Proof] módulos y sus campos

Al configurar [!DNL Workfront Proof] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL Workfront Proof] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, vea [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Déclencheur](#triggers)
* [Acciones](#actions)
* [Búsquedas](#searches)

### Déclencheur

* [Ver revisiones](#watch-proofs)
* [Observe el resumen del PDF](#watch-for-pdf-summary)
* [[!UICONTROL Actividad de revisión]](#watch-proof-activity)

#### [!UICONTROL Observar revisiones]

Este módulo de déclencheur programado ejecuta un escenario en el que alguien crea o toma una decisión sobre una revisión.

El módulo devuelve una lista de todos los registros que encuentra durante el período especificado, junto con sus tipos. También devuelve los valores de los campos especificados. Si el módulo ha encontrado decisiones tomadas sobre la prueba, incluye los valores anterior y actual en campos independientes. Puede asignar esta información en módulos subsiguientes en el escenario.

Esto sucede en un intervalo programado de forma regular que usted especifica.

Debe tener permisos suficientes para tener acceso a la revisión o revisiones en [!DNL Workfront Proof] a fin de recuperar esta información.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Workfront Proof] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tipo de registro</td> 
   <td>Seleccione el tipo de registro [!DNL Workfront Proof] que desea que el módulo vea.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Salidas</td> 
   <td> <p>Seleccione la información que desee incluir en el paquete de salida para este módulo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Límite</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Observe el resumen del PDF]

Este módulo de déclencheur instantáneo ejecuta un escenario en el que alguien crea un resumen de PDF para una prueba.

Se requiere un webhook en este módulo.

El módulo devuelve todos los campos estándar asociados con la prueba, junto con los campos y valores personalizados a los que accede la conexión. También crea una nueva suscripción de evento para resúmenes de PDF y genera el contenido del atributo &quot;pdf_url&quot; enviado en la carga. Puede asignar esta información en módulos subsiguientes en el escenario.

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
   <td>Puede seleccionar un webhook existente o crear uno nuevo. Para obtener más información, vea <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">déclencheur instantáneos (webhooks) en [!DNL Adobe Workfront Fusion]</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Límite]</td> 
   <td>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actividad de revisión]

Este módulo de déclencheur ejecuta un escenario en el que se produce una actividad especificada en una prueba de revisión.

El módulo devuelve todos los campos estándar asociados con la prueba, junto con los campos y valores personalizados a los que accede la conexión. También crea una nueva suscripción de evento para resúmenes de PDF y genera el contenido del atributo `pdf_url` enviado en la carga. Puede asignar esta información en módulos subsiguientes en el escenario.

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
   <td>[!UICONTROL Tipo de actividad]</td> 
   <td>Seleccione si desea ver cualquier nueva decisión (incluidos los cambios de estado de [!UICONTROL prueba]) o solo los cambios de estado de prueba generales.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Límite]</td> 
   <td>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</td> 
  </tr> 
 </tbody> 
</table>

### Acciones

* [[!UICONTROL Crear revisión]](#create-proof)
* [[!UICONTROL Llamada de API personalizada]](#custom-api-call)
* [[!UICONTROL Descargar revisión]](#download-proof)
* [[!UICONTROL Leer un registro]](#read-a-record)
* [[!UICONTROL Solicitar resumen de PDF]](#request-pdf-summary)
* [[!UICONTROL Actualizar revisión]](#update-proof)
* [[!UICONTROL Cargar archivo]](#upload-file)

#### [!UICONTROL Crear revisión]

Este módulo de acción crea una nueva revisión o versión de una revisión en [!DNL Workfront Proof].

Especifique los parámetros para la nueva prueba y la prueba de origen si va a crear una nueva versión.

El módulo devuelve el ID de la nueva versión de prueba o revisión. Puede asignar esta información en módulos posteriores en el escenario.

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
   <td>[!UICONTROL Tipo de prueba]</td> 
   <td> <p>Especifique si desea que la prueba creada tenga un flujo de trabajo básico o un flujo de trabajo automatizado de [!UICONTROL].</p> <p>A continuación, rellene los campos que se muestran para el tipo de prueba elegido. Por ejemplo, si elige [!UICONTROL Flujo de trabajo automatizado], rellene el campo <strong>[!UICONTROL Fases del flujo de trabajo]</strong> para configurar las fases.</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Permitir la descarga del archivo original]</td> 
   <td>Seleccione si desea permitir la descarga del archivo original desde el que se creó la prueba.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Classic Proof Viewer]</td> 
   <td>Seleccione si está utilizando el Visor de pruebas clásico.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Combinar todos los archivos en una sola prueba]</td> 
   <td>Active esta opción para combinar todos los archivos en una sola prueba de varias páginas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Crear nueva versión de revisión]</td> 
   <td>Seleccione esta opción si desea que el módulo cree una nueva versión de una revisión existente. A continuación, en el campo <strong>[!UICONTROL Existing Proof ID]</strong> que se muestra, asigne o escriba el ID único de la prueba.</td> 
  </tr> 
  <tr> 
   <td>Etiqueta de vínculo personalizado de [!UICONTROL]</td> 
   <td>Introduzca o asigne una etiqueta para el vínculo de prueba personalizado.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL URL de vínculo personalizado]</td> 
   <td>Introduzca o asigne la dirección URL del vínculo personalizado.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Notificaciones por correo electrónico predeterminadas para suscriptores]</td> 
   <td>Escriba uno de los números siguientes para indicar cuál de los siguientes valores predeterminados de notificación por correo electrónico desea utilizar para la prueba que se crea.
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
   <td>[!UICONTROL Deshabilitar resumen de Excel]</td> 
   <td>Seleccione si desea deshabilitar la capacidad de descargar comentarios de revisión en un archivo de Excel.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Deshabilitar resumen de PDF]</td> 
   <td>Seleccione si desea deshabilitar la capacidad de descargar comentarios de revisión en un archivo de PDF.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Deshabilitar correo electrónico de suscripción]</td> 
   <td>Seleccione si desea deshabilitar el correo electrónico de suscripción para esta prueba.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Habilitar reproductor incrustado]</td> 
   <td>Seleccione si desea habilitar el reproductor incrustado para esta prueba.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Habilitar suscripciones]</td> 
   <td>Seleccione si las personas que no son participantes pueden suscribirse a la prueba.<br>Si selecciona esta opción, también puede seleccionar el Rol predeterminado para los suscriptores, tal como se describe en esta tabla.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Habilitar validación de suscripciones]</td> 
   <td>Seleccione si desea activar la validación del correo electrónico de suscripción. Si está activada, el suscriptor debe hacer clic en un vínculo de un correo electrónico para acceder a una prueba.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Habilitar URL del equipo]</td> 
   <td>Seleccione si desea que la prueba creada oculte o muestre la dirección URL del equipo.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Hash de archivo] <span style="font-weight: normal;">o</span> [!UICONTROL Hashes de archivo]</td> 
   <td>Añada el ID del archivo o archivos desde los que desea crear una o varias pruebas.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Nombres de archivo]</td> 
   <td>Añada el nombre o los nombres del archivo para la prueba que se ha creado. Este campo es obligatorio.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Bloquear prueba cuando se toman todas las decisiones necesarias]</td> 
   <td>Especifique si desea que la prueba creada se bloquee después de tomar todas las decisiones necesarias.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Notificar a los destinatarios sobre esta revisión]</td> 
   <td>Seleccione una opción para indicar si desea que se notifique a los destinatarios cuando se cree la prueba.&gt;</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre de prueba]</td> 
   <td>Escriba un nombre para la prueba que se crea. Este campo es obligatorio. Utilice un símbolo de barra vertical (|) para separar los nombres de varias pruebas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Identificador de propietario de revisión]</td> 
   <td>Introduzca o asigne el ID del propietario de la prueba. Si este campo se deja en blanco, el propietario de la prueba se establece en el usuario actual.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de referencia]</td> 
   <td>Introduzca el ID de referencia de la prueba.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Requerir firma electrónica]</td> 
   <td>Seleccione si desea exigir a cualquier persona que tome una decisión sobre una prueba que envíe una firma electrónica.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Requerir inicio de sesión]</td> 
   <td> <p>Especifique si desea que la prueba creada requiera un inicio de sesión. </p> <p>Esto es lo mismo que la configuración de [!UICONTROL Se requiere inicio de sesión] explicada en <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">[!UICONTROL Configurar opciones de revisión] en [!DNL Workfront Proof]</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID de resolución]</td> 
   <td>Introduzca el ID de la resolución que desea utilizar para la prueba. Para obtener una lista de los identificadores de resolución, consulte la [!DNL Workfront Proof] <a href="https://api.proofhq.com/home/objects/soapworkflowproofobject.html">documentación de API</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL SWF]</td> 
   <td>Introduzca el tipo de prueba del SWF.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Mostrar] [elemento]</td> 
   <td>Para cada elemento, seleccione si desea mostrarlo en la prueba.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Workspace ID]</td> 
   <td>Introduzca el ID del espacio de trabajo en el que desea crear la prueba. </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Destinatarios]</td> 
   <td>Añada las direcciones de correo electrónico de los destinatarios que desee para la prueba creada</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Plazo]</td> 
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
   <td>[!UICONTROL Método]</td> 
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

#### [!UICONTROL Descargar revisión]

Este módulo de acción descarga el archivo de origen de una prueba concreta que identifica con su ID.

Especifique el ID de la prueba.

El módulo devuelve el contenido del archivo de origen utilizado para crear la prueba. Puede asignar esta información en módulos posteriores en el escenario.

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
   <td>[!UICONTROL Identificador de revisión]</td> 
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
   <td>[!UICONTROL Tipo de registro]</td> 
   <td>Seleccione si desea leer una prueba, comentarios de prueba o revisores de prueba.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Salidas]</td> 
   <td> <p>Seleccione la información que desee incluir en el paquete de salida para este módulo.</p> </td> 
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
   <td>[!UICONTROL Identificador de revisión]</td> 
   <td> <p>Introduzca el identificador único [!DNL Workfront Proof] de la revisión para la cual desea solicitar un resumen de PDF.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Callback URL]</td> 
   <td>Introduzca o asigne la dirección URL a la que desea enviar el resumen del PDF.</td> 
  </tr> 
 </tbody> 
</table>

##### Posible error

* **Error**: &quot;[!UICONTROL No cuenta con privilegios para realizar esta solicitud. La fase debe contener al menos un destinatario.]&quot;
* **Solución**: asegúrese de que no es el único que está asignado a las fases del flujo de trabajo. Debe haber otro usuario asignado a las fases del flujo de trabajo.

#### [!UICONTROL Actualizar revisión]

Este módulo de acción actualiza una revisión existente en [!DNL Workfront Proof].

Especifique el ID de la prueba y el tipo de registro, así como los campos que desea incluir en la salida.

El módulo devuelve cualquier campo estándar asociado con el registro, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

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
   <td>[!UICONTROL Identificador de revisión]</td> 
   <td> <p>Escriba el identificador único de la prueba, que se encuentra en la página [!UICONTROL Proof Details]. Para obtener más información, consulte <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md" class="MCXref xref" data-mc-variable-override="">Administrar detalles de revisión en [!DNL Workfront Proof]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plazo]</td> 
   <td> <p>Especifique la fecha límite que desea para la prueba que se ha creado. Utilice el siguiente formato de fecha:</p> <p><code>YYYY-MM-DD hh:mm</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Notificaciones por correo electrónico predeterminadas para suscriptores]</td> 
   <td>Seleccione cuál de las siguientes opciones predeterminadas de notificación por correo electrónico desea utilizar para la prueba que se crea.
    <ul>
     <li> [!UICONTROL Todos los comentarios y respuestas nuevos]</li>
     <li>[!UICONTROL Respuestas a mis comentarios]</li>
     <li>[!UICONTROL Resumen diario]</li>
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
   <td>Seleccione si desea deshabilitar el correo electrónico de suscripción para esta prueba.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Habilitar suscripciones]</td> 
   <td>Seleccione si las personas que no son participantes pueden suscribirse a la prueba.<br>Si selecciona esta opción, también puede seleccionar el [!UICONTROL Rol predeterminado] para los suscriptores, tal como se describe en esta tabla.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Habilitar validación de suscripciones]</td> 
   <td>Seleccione si desea activar la validación del correo electrónico de suscripción. Si está activada, el suscriptor debe hacer clic en un vínculo de un correo electrónico para acceder a una prueba.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Habilitar URL del equipo]</td> 
   <td>Seleccione si desea que la prueba creada oculte o muestre la dirección URL del equipo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Bloquear prueba cuando se toman todas las decisiones necesarias]</td> 
   <td>Especifique si desea que la prueba creada se bloquee después de tomar todas las decisiones necesarias.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mensaje]</td> 
   <td>Introduzca o asigne un mensaje que desee que acompañe a la prueba.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Identificador de revisión] </td> 
   <td>Introduzca o asigne el ID de la prueba que desea actualizar.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre de revisión]</td> 
   <td>Introduzca o asigne el nombre de la prueba que desea actualizar.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Requerir inicio de sesión]</td> 
   <td> <p>Especifique si desea que la prueba creada requiera un inicio de sesión. </p> <p>Esto es lo mismo que la configuración de [!UICONTROL Se requiere inicio de sesión] explicada en <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">[!UICONTROL Configurar opciones de revisión] en [!DNL Workfront Proof]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mostrar versiones como]</td> 
   <td>Seleccione si desea mostrar un vínculo a otras versiones de esta revisión.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Asunto]</td> 
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
   <td>[!UICONTROL archivo Source]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Búsquedas

* [[!UICONTROL Plantillas de flujo de trabajo de lista]](#list-workflow-templates)
* [[!UICONTROL Búsqueda]](#search)

#### [!UICONTROL Plantillas de flujo de trabajo de lista]

Este módulo de búsqueda enumera todas las plantillas de flujo de trabajo disponibles.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Workfront Proof] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Salidas]</td> 
   <td> <p>Seleccione la información que desee incluir en el paquete de salida para este módulo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de plantillas que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Búsqueda]

Este módulo de búsqueda busca registros en un objeto de [!DNL Workfront Proof] que coincidan con la consulta de búsqueda especificada.

El módulo devuelve el ID de la prueba si está buscando una prueba. También devuelve los ID de usuario, los correos electrónicos, los nombres, las posiciones y los alias de correo electrónico de los destinatarios, si está buscando destinatarios. Puede asignar esta información en módulos posteriores en el escenario.

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
   <td> <p>Se[!UICONTROL ]Seleccione el tipo de registro que desea que busque el módulo.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Proof]</strong> </p> <p>Introduzca el Nombre de la revisión que desea buscar.</p> </li> 
     <li> <p><strong>[!UICONTROL Destinatario]</strong> </p> <p>Introduzca la dirección de correo electrónico del destinatario que desea buscar.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Conjunto de resultados]</td> 
   <td>Indique si el módulo buscará <strong>[!UICONTROL Todos los registros coincidentes]</strong> o solo el <strong>[!UICONTROL Primer registro coincidente]</strong>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Ordenar por]</td> 
   <td>Seleccione el campo por el que desea ordenar los resultados.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Dirección de ordenación]</td> 
   <td> <p>Seleccione si desea ordenar los resultados de forma ascendente o descendente.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Plantillas de flujo de trabajo de lista]

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
   <td>[!UICONTROL Salidas]</td> 
   <td> <p>Seleccione la información que desee incluir en el paquete de salida para este módulo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de plantillas que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>
