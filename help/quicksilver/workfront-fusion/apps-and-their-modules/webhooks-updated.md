---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Enlaces web
description: Un enlace web es una llamada HTTP que se activa mediante un evento. Puede utilizar webhooks para activar módulos de déclencheur instantáneo. Cualquier aplicación conectada a Internet y que permita solicitudes HTTP puede enviar enlaces web a Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 987544a4-5840-40d4-9438-41a000aa22ee
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1391'
ht-degree: 0%

---

# Enlaces web

Un enlace web es una llamada HTTP que se activa mediante un evento. Puede utilizar webhooks para activar módulos de déclencheur instantáneo. Cualquier aplicación conectada a Internet y que permita solicitudes HTTP puede enviar enlaces web a Adobe Workfront Fusion.

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
   <td> <p>[!UICONTROL Workfront Fusion para automatización e integración del trabajo] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr>
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

&#42;&#42;Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Use un enlace web en [!DNL Workfront Fusion]

>[!NOTE]
>
>Para llamar a un enlace web de terceros (un enlace web saliente), utilice uno de los módulos HTTP. Para obtener más información, consulte [Módulos HTTP](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

Para utilizar un enlace web para conectar una aplicación a [!DNL Workfront Fusion]:

1. Agregue la variable **[!UICONTROL Enlaces web]** >**[!UICONTROL Vínculo web personalizado]** módulo de déclencheur instantáneo a su escenario.

1. Haga clic en **[!UICONTROL Agregar]** junto al campo Weblock e introduzca un nombre para el nuevo weblock.
1. (Opcional) Haga clic en **[!UICONTROL Configuración avanzada]**.
1. En el **[!UICONTROL Restricciones de IP]** , introduzca una lista separada por comas de las direcciones IP desde las que el módulo puede aceptar datos.
1. Haga clic en **[!UICONTROL Guardar]**

Después de crear un vínculo web, se muestra una dirección URL única. Esta es la dirección a la que el enlace web envía datos. Workfront Fusion valida los datos enviados a esta dirección y luego los pasa para su procesamiento en el escenario.

>[!NOTE]
>
>Una vez creado un vínculo web, puede utilizarlo en más de un escenario a la vez.

### Configuración de la estructura de datos del vínculo web {#configure-the-webhook-s-data-structure}

Para reconocer la estructura de datos de la carga útil entrante, [!DNL Workfront Fusion] analiza los datos de ejemplo que envía a la dirección mostrada. Puede proporcionar los datos de ejemplo realizando un cambio en el servicio o la aplicación que hará que ese servicio o la aplicación llamen al vínculo web. Por ejemplo, puede quitar un archivo.

O puede seguir los pasos que se indican a continuación para enviar los datos de ejemplo a través del [!UICONTROL HTTP] > [!UICONTROL Realizar una solicitud] módulo.

1. Cree un nuevo escenario con la variable **[!UICONTROL HTTP]** > **[!UICONTROL Realizar una solicitud]** módulo

1. Configure el módulo con los siguientes valores:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><p>[!UICONTROL URL] </p></td> 
      <td>Introduzca la URL del enlace web. Puede encontrar esta URL en el módulo [!UICONTROL Webhooks] que ha utilizado para configurar el enlace web.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Método] </td> 
      <td><p>[!UICONTROL POST]</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tipo de cuerpo]</td> 
      <td><p> [!UICONTROL Raw]</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Content type]</td> 
      <td><p> JSON (aplicación/json)</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Solicitar contenido]</td> 
      <td><p>Se espera JSON sin procesar en el enlace web</p></td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/new-scenario-set-up-like-this-350x446.png)

1. Abra el escenario con la [!UICONTROL Enlaces web] en una pestaña o ventana de navegador independiente.
1. En el módulo webhooks, haga clic en **[!UICONTROL Volver a determinar la estructura de datos]**.

   No es necesario desvincular otros módulos del módulo webhooks.

1. Cambie al escenario con la variable [!UICONTROL HTTP] y ejecútelo.
1. Vuelva al escenario con el módulo Webhooks.

   Un &quot;[!UICONTROL Determinado correctamente]&quot; mensaje significa que el módulo ha determinado correctamente la estructura de datos.

   ![](assets/successfully-determined-350x175.png)

1. Haga clic en **[!UICONTROL OK]** para guardar la estructura de datos.

   Los elementos del vínculo web ya están disponibles en el panel de asignación para su uso con módulos posteriores en el escenario.

## Cola

Si un vínculo web recibe datos y no hay un escenario activo que espere esos datos, los datos se almacenan en la cola. Una vez activado el escenario, procesa todos los paquetes que esperan en la cola secuencialmente.

>[!IMPORTANT]
>
>Las colas de Weblock se comparten entre escenarios que emplean el mismo weblock. Si se desactiva uno de los escenarios, todos los datos entrantes se mantienen en cola.

## Formatos de datos entrantes compatibles

[!DNL Workfront Fusion] admite 3 formatos de datos entrantes: [!UICONTROL Cadena de consulta], [!UICONTROL Datos de formulario] y [!UICONTROL JSON].

[!DNL Workfront Fusion] valida todos los datos entrantes con la estructura de datos seleccionada. A continuación, según la configuración del escenario, los datos se almacenan en la cola para su procesamiento o se procesan inmediatamente.

Si alguna parte de los datos no pasa la validación, [!DNL Workfront Fusion] devuelve un código de estado HTTP 400 y especifica, en el cuerpo de la respuesta HTTP, el motivo por el que los datos entrantes fallaron en las comprobaciones de validación. Si la validación de los datos entrantes se realiza correctamente, Workfront Fusion devuelve un error[!UICONTROL 200 aceptados]&quot;.

* [[!UICONTROL Cadena de consulta]](#query-string)
* [[!UICONTROL Datos de formulario]](#form-data)
* [[!UICONTROL JSON]](#json)

### [!UICONTROL Cadena de consulta]

```
GET https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>?name=<yourname>&job=automate
```

### [!UICONTROL Datos de formulario]

```
POST https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>

Content-Type: application/x-www-form-urlencoded

name=<yourname>&job=automate
```

#### Datos de formulario de varias partes

```
POST https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>


Content-Type: multipart/form-data; boundary=---generatedboundary

---generatedboundary

Content-Disposition: form-data; name="file"; filename="file.txt"


Content-Type: text/plain


Content of file.txt


---generatedboundary

Content-Disposition: form-data; name="name"

Workfront Fusion

---generatedboundary
```

Para recibir archivos codificados con `multipart/form-data`, debe configurar una estructura de datos con un `collection` campo de tipo que contiene los campos anidados `name`, `mime`y `data`. El campo `name` es `text` y contiene el nombre del archivo cargado. La variable `mime` es `text` y contiene un archivo en formato MIME. El campo `data` es `buffer` y contiene datos binarios para el archivo que se va a transferir.

Para obtener más información sobre el formato MIME, consulte [Módulos MIME](../../workfront-fusion/apps-and-their-modules/mime.md).

### [!UICONTROL JSON]

```
POST https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>

Content-Type: application/json

{"name": "Workfront Fusion", "job": "automate"}
```

>[!TIP]
>
>Si desea acceder al JSON original, habilite el paso a través de JSON al configurar el vínculo web.
>
>1. Haga clic en **[!UICONTROL Agregar]** para agregar un nuevo weblock.
>1. Haga clic en **[!UICONTROL Mostrar configuración avanzada]**.
>1. Haga clic en **[!UICONTROL Transmisión de JSON]**.

>


## Encabezados de enlace web

Para acceder a los encabezados de weblock, habilite Get request headers al configurar el weblink.

1. Haga clic en **[!UICONTROL Agregar]** para agregar un nuevo weblock.
1. Haga clic en **[!UICONTROL Mostrar configuración avanzada]**.
1. Haga clic en **[!UICONTROL Obtener encabezados de solicitud]**.

Puede extraer un valor de encabezado determinado mediante la combinación de `map()` y `get()` funciones.

>[!INFO]
>
>**Ejemplo:**
>
>El ejemplo siguiente muestra una fórmula que extrae el valor de la variable `authorization` del `Headers[]` matriz. La fórmula se utiliza en un filtro que compara el valor extraído con el texto dado para pasar solo los enlaces web si hay una coincidencia.
>
>![](assets/set-up-a-filter-350x169.png)
>
>Para obtener más información sobre la obtención del elemento de una matriz con una clave determinada, consulte [Asignación del elemento de una matriz con una clave determinada](../../workfront-fusion/mapping/map-information-between-modules.md#mapping) en el artículo [Asignación de información de un módulo a otro en Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

## Respuesta a los enlaces web

La respuesta predeterminada a una llamada de enlace web es el texto &quot;Aceptado&quot;. La respuesta se devuelve a la aplicación que llamó al enlace web durante la ejecución del módulo Weblock personalizado.

* [Probar la respuesta a un enlace web](#test-the-response-to-a-webhook)
* [Ejemplo de respuesta del HTML](#html-response-example)
* [Ejemplo de redirección](#redirect-example)

### Probar la respuesta a un enlace web

1. Incluya la variable **[!UICONTROL Vínculo web personalizado]** en su escenario.
1. Añada un nuevo enlace web al módulo.
1. Copie la URL del vínculo web en el portapapeles.
1. Ejecute el escenario.

   El icono de relámpago en el [!UICONTROL Vínculo web personalizado] cambia a puntos giratorios. Esto muestra que el módulo está esperando a la llamada de enlace web.

1. Abra una nueva ventana del explorador, pegue la dirección URL copiada en la barra de direcciones y pulse **[!UICONTROL Entrar]**.

   La variable [!UICONTROL Vínculo web personalizado] se activa y el explorador mostrará una página nueva.

Si desea personalizar la respuesta del weblock, utilice el módulo Weblock Response.

La configuración del módulo contiene dos campos: [!UICONTROL Estado] y [!UICONTROL Cuerpo].

* La variable [!UICONTROL Estado] El campo contiene códigos de estado de respuesta HTTP como 2xx para Success (por ejemplo, `200` para OK), 3xx para Redirección (por ejemplo, `307` para la redirección temporal), 4xx para errores de cliente (por ejemplo, `400` para solicitud incorrecta), etc.

* La variable [!UICONTROL Cuerpo] contiene todo lo que será aceptado por la llamada de weblock. Puede ser texto simple, HTML, XML, JSON, etc.

   >[!TIP]
   >
   >Se recomienda configurar la variable `Content-Type` encabezado al tipo MIME correspondiente: `text/plain` para texto sin formato, `text/html` para HTML, `application/json` para JSON, `application/xml` para XML, etc. Para obtener más información sobre los tipos MIME, consulte [Módulos MIME](../../workfront-fusion/apps-and-their-modules/mime.md).

El tiempo de espera para enviar una respuesta es de 40 segundos. Si la respuesta no está disponible dentro de ese periodo, Workfront Fusion devuelve el estado &quot;200 Accepted&quot;.

### Ejemplo de respuesta del HTML

>[!INFO]
>
>**Ejemplo:**
>
>Configure las variables [!UICONTROL Respuesta de Weblock] como se indica a continuación:
>
><table style="table-layout:auto"> 
&gt; <col> 
&gt; <col> 
&gt; <tbody> 
&gt;  <tr> 
&gt;   <td role="rowheader">[!UICONTROL Status] </td> 
&gt;   <td> <p>Código de estado HTTP de éxito 2xx, por ejemplo 200</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader">[!UICONTROL Body] </td> 
&gt;   <td> <p>código del HTML</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader"> <p>[!UICONTROL encabezados personalizados]</p> </td> 
&gt;   <td> 
&gt;    <ul> 
&gt;     <li><strong>Clave</strong>: Content-type</li> 
&gt;     <li><strong>Valor</strong>: text/html</li> 
&gt;    </ul> </td> 
&gt;  </tr> 
&gt; </tbody> 
&gt;</table>
>
>![](assets/custom-headers-350x235.png)
>
>Esto generará una respuesta de HTML que se muestra en un explorador web:
>
>![](assets/html-response-350x70.png)

### Ejemplo de redirección

>[!INFO]
>
>**Ejemplo:** Configure las variables [!UICONTROL Respuesta de Weblock] como se indica a continuación:
>
><table style="table-layout:auto"> 
&gt; <col> 
&gt; <col> 
&gt; <tbody> 
&gt;  <tr> 
&gt;   <td role="rowheader">[!UICONTROL Status] </td> 
&gt;   <td> <p>Código de estado HTTP de redirección 3xx, por ejemplo 303</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader"> <p>[!UICONTROL encabezados personalizados]</p> </td> 
&gt;   <td> 
&gt;    <ul> 
&gt;     <li><strong>[!UICONTROL Key]</strong>: Ubicación</li> 
&gt;     <li><strong>[!UICONTROL Valor]</strong>: La dirección URL a la que desea redirigir.</li> 
&gt;    </ul> </td> 
&gt;  </tr> 
&gt; </tbody> 
&gt;</table>
>
>![](assets/webhook-response-350x279.png)

## Desactivación de Weblock

Los Webhooks se desactivan automáticamente si se aplica cualquiera de las siguientes opciones:

* El enlace web no ha estado conectado a ningún escenario durante más de 5 días
* El enlace web solo se utiliza en escenarios inactivos, que han estado inactivos durante más de 30 días.

Los enlaces web desactivados se eliminan y no se registran automáticamente si no están conectados a ningún escenario y han estado en estado desactivado durante más de 30 días.


## Resolución de problemas

### Elementos que faltan en el panel de asignación

Si faltan algunos elementos en el panel de asignación en la configuración de los módulos después de [!UICONTROL Enlaces web] > [!UICONTROL Vínculo web personalizado] , haga clic en el **[!UICONTROL Enlaces web] > [!UICONTROL Vínculo web personalizado]** para abrir su configuración y haga clic en **[!UICONTROL Volver a determinar la estructura de datos]**:

![](assets/redetermine-data-structure-btn-350x195.png)

A continuación, siga los pasos descritos en la sección [Configuración de la estructura de datos del vínculo web](#configure-the-webhook-s-data-structure) en este artículo.
