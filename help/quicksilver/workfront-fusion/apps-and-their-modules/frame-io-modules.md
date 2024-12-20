---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos Frame.io
description: La cuenta  [!DNL Adobe Workfront Fusion Frame].io modules enable you to monitor, create, update, retrieve, or delete assets and comments in your [!DNL Frame.io] .
author: Becky
feature: Workfront Fusion
exl-id: 373a86f6-fbba-4914-b08d-a3a035ac0ae4
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '2356'
ht-degree: 0%

---

# [!DNL Frame.io] módulos

Los módulos [!DNL Adobe Workfront Fusion] [!DNL Frame.io] le permiten supervisar, crear, actualizar, recuperar o eliminar recursos y comentarios en su cuenta de [!DNL Frame.io].

Para ver un vídeo introductorio del conector Frame.io, consulte:

* [Frame.io](https://video.tv.adobe.com/v/3427032/){target=_blank}

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
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p>
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

Para usar módulos de [!DNL Frame.io], debe tener una cuenta de [!DNL Frame.io]

## Información de la API Frame.io

El conector Frame.io utiliza lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL básica</td> 
   <td> https://api.frame.io/v2</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Versión de API</td> 
   <td> Versión 2 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Etiqueta de API</td> 
   <td>Versión 1.0.76</td> 
  </tr>
 </tbody> 
 </table>

## Conectar [!DNL Frame.io] a [!UICONTROL Adobe Workfront Fusion]

Puede conectarse a [!DNL Frame.io] mediante un token de API o mediante OAuth 2.0.

[Conectarse a [!DNL Frame.io] usando un token de API](#connect-to-frameio-using-an-api-token)

[Conectarse a [!DNL Frame.io] usando OAuth 2.0 PKCE](#connect-to-frameio-using-oauth-20-pkce)

### Conectar con [!DNL Frame.io] mediante un token de API

Para conectar tu cuenta de [!DNL Frame.io] a [!DNL Workfront Fusion] mediante un token de API, debes crear el token de API en tu cuenta de [!DNL Frame.io] e insertarlo en el cuadro de diálogo [!DNL Workfront Fusion] [!DNL Frame.io] [!UICONTROL Crear una conexión].

1. Inicie sesión en su cuenta de [!DNL Frame.io].
1. Vaya a la página **[!UICONTROL Tokens]** en el [!DNL Frame.io] Developer.
1. Haga clic en **[!UICONTROL Nuevo]**.
1. Escriba el nombre del token, seleccione los ámbitos que desee usar y haga clic en **[!UICONTROL Crear]**.
1. Copie el token proporcionado.
1. Vaya a [!DNL Workfront Fusion] y abra el diálogo **[!UICONTROL Crear una conexión]** del módulo [!DNL Frame.io].
1. En el campo **[!UICONTROL Tipo de conexión]**, seleccione **[!DNL Frame.io]**.
1. Escriba el token que copió en el paso 5 en el campo **[!UICONTROL Su clave de API [!DNL Frame.io]]** y haga clic en **[!UICONTROL Continuar]** para establecer la conexión.

Se ha establecido la conexión. Puede continuar con la configuración del módulo.

### Conectar con [!DNL Frame.io] mediante OAuth 2.0 PKCE

Puede crear una conexión con [!DNL Frame.io] mediante OAuth 2.0 PKCE con un ID de cliente opcional. Si desea incluir un ID de cliente en la conexión, debe crear una aplicación OAuth 2.0 en la cuenta [!DNL Frame.io].

* [Conectarse a  [!DNL Frame.io] usando OAuth 2.0 PKCE (sin ID de cliente)](#connect-to-frameio-using-using-oauth-20-pkce-without-client-id)
* [Conectarse a  [!DNL Frame.io] usando OAuth 2.0 PKCE (con ID de cliente)](#connect-to-frameio-using-using-oauth-20-pkce-with-client-id)

#### Conectarse a [!DNL Frame.io] mediante OAuth 2.0 PKCE (sin ID de cliente)

1. Vaya a [!DNL Workfront Fusion] y abra el diálogo **[!UICONTROL Crear una conexión]** del módulo [!DNL Frame.io].
1. En el campo **[!UICONTROL Tipo de conexión]**, seleccione **[!UICONTROL [!DNL Frame.io]OAuth 2.0 PKCE]**.
1. Escriba un nombre para la nueva conexión en el campo **[!UICONTROL Nombre de conexión]**.
1. Haga clic en **[!UICONTROL Continuar]** para establecer la conexión.

Se ha establecido la conexión. Puede continuar con la configuración del módulo.

#### Conectarse a [!DNL Frame.io] mediante OAuth 2.0 PKCE (con ID de cliente)

1. Crear una aplicación OAuth 2.0 en [!DNL Frame.io]. Para obtener instrucciones, consulte la documentación de [!DNL Frame.io] en [!UICONTROL Flujo de autorización de código de OAuth 2.0].

   >[!IMPORTANT]
   >
   >Al crear la aplicación OAuth 2.0 en [!DNL Frame.io]:
   >
   >* Introduzca lo siguiente como URI de redireccionamiento:
   >   
   >  América/APAC `https://app.workfrontfusion.com/oauth/cb/frame-io5`
   >
   >  EMEA `https://app-eu.workfrontfusion.com/oauth/cb/frame-io5`
   >
   >* Active la opción PCKE.


1. Copie el `client_id` proporcionado.
1. Vaya a [!DNL Workfront Fusion] y abra el diálogo **[!UICONTROL Crear una conexión]** del módulo [!DNL Frame.io].
1. En el campo **[!UICONTROL Tipo de conexión]**, seleccione **[!UICONTROL [!DNL Frame.io]OAuth 2.0 PKCE]**.
1. Escriba un nombre para la nueva conexión en el campo **[!UICONTROL Nombre de conexión]**.
1. Haga clic en **[!UICONTROL Mostrar configuración avanzada]**.
1. Escriba el(la) `client_id` que copió en el paso 2 en el campo **[!UICONTROL ID de cliente]**.
1. Haga clic en **[!UICONTROL Continuar]** para establecer la conexión.

Se ha establecido la conexión. Puede continuar con la configuración del módulo.

## [!DNL Frame.io] módulos y sus campos

Al configurar [!DNL Frame.io] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL Frame.io] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, vea [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Recursos](#assets)
* [Comentarios](#comments)
* [Proyectos](#projects)
* [Otro](#other)

### Recursos

* [[!UICONTROL Crear un recurso]](#create-an-asset)
* [[!UICONTROL Eliminar un recurso]](#delete-an-asset)
* [[!UICONTROL Obtener un recurso]](#get-an-asset)
* [[!UICONTROL Lista de Assets]](#list-assets)
* [[!UICONTROL Actualizar un recurso]](#update-an-asset)
* [[!UICONTROL Recurso de observación eliminado]](#watch-asset-deleted)
* [[!UICONTROL Etiqueta de recurso de inspección actualizada]](#watch-asset-label-updated)
* [[!UICONTROL Ver nuevo recurso]](#watch-new-asset)

#### [!UICONTROL Crear un recurso]

Este módulo de acción crea un nuevo recurso.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Frame.io], vea <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de equipo] </td> 
   <td> <p>Seleccione o asigne el equipo propietario del proyecto para el que desea crear un recurso.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificador de proyecto] </td> 
   <td> <p>Seleccione el proyecto o asigne el ID del proyecto para el que desea crear un recurso.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificador de carpeta] </td> 
   <td> <p>Seleccione la carpeta o asigne el ID de la carpeta en la que desea crear un recurso.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo] </td> 
   <td> <p>Seleccione si desea crear una carpeta o un archivo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre] </td> 
   <td> <p>Introduzca el nombre del nuevo archivo o carpeta.</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">File Type </td> 
    <td> <p>Select the type of file you want to upload.</p> </td> 
   </tr>
  --> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">File Size </td> 
    <td> <p>The file size in bytes.</p> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL DE Source] </td> 
   <td> <p>Introduzca la dirección URL del archivo que desea cargar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descripción] </td> 
   <td> <p>Introduzca una breve descripción del recurso.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar un recurso]

Este módulo de acción elimina un recurso especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Frame.io], vea <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de equipo] </td> 
   <td> <p>Seleccione o asigne el equipo propietario del proyecto que contiene el recurso que desea eliminar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificador de proyecto]</td> 
   <td> <p> Seleccione el proyecto o proyecto que contiene el recurso que desea eliminar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificador de carpeta] </td> 
   <td> <p>Seleccione la carpeta que contiene el recurso que desea eliminar</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de recurso] </td> 
   <td> <p>Seleccione o asigne el recurso que desea eliminar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener un recurso]

Este módulo de acción recupera los detalles del recurso.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Frame.io], vea <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de equipo] </td> 
   <td> <p>Seleccione o asigne el equipo propietario del proyecto que contiene el recurso cuyos detalles desea recuperar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificador de proyecto]</td> 
   <td> <p> Seleccione el proyecto que contiene el recurso sobre el que desea recuperar detalles.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificador de carpeta] </td> 
   <td> <p>Seleccione la carpeta que contiene el recurso cuyos detalles desea recuperar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de recurso] </td> 
   <td> <p>Seleccione el recurso o asigne el ID del recurso sobre el que desea recuperar detalles.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Lista de Assets]

Este módulo de búsqueda recupera todos los recursos de la carpeta del proyecto especificado.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Frame.io], vea <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de equipo] </td> 
   <td> <p>Seleccione o asigne el equipo propietario del proyecto que contiene la carpeta de la que desea recuperar los recursos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificador de proyecto]</td> 
   <td> <p> Seleccione el proyecto que contiene la carpeta de la que desea recuperar los recursos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificador de carpeta] </td> 
   <td> <p>Seleccione la carpeta desde la que desee enumerar los recursos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite] </td> 
   <td> <p>Establezca el número máximo de recursos que [!DNL Workfront Fusion] devolverá durante un ciclo de ejecución.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### `[!UICONTROL Update an Asset]`

Este módulo de acción le permite actualizar el nombre, la descripción o los campos personalizados de un recurso existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Frame.io], vea <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de equipo] </td> 
   <td> <p>Seleccione o asigne el equipo propietario del proyecto para el que desea actualizar un recurso.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificador de proyecto] </td> 
   <td> <p>Seleccione el proyecto o asigne el ID del proyecto para el que desea actualizar un recurso.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificador de carpeta] </td> 
   <td> <p>Seleccione la carpeta o asigne el ID de la carpeta en la que desea actualizar un recurso.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre] </td> 
   <td> <p>Introduzca el nombre del archivo actualizado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descripción] </td> 
   <td> <p>Introduzca una breve descripción del recurso actualizado.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Recurso de observación eliminado]

Este módulo de déclencheur inicia un escenario cuando se elimina un recurso.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Nombre de webhook de [!UICONTROL]</td> 
   <td> <p> Introduzca el nombre del webhook (por ejemplo: Recurso eliminado).</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Frame.io], vea <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de equipo] </td> 
   <td> <p>Seleccione el equipo para el que se crea este webhook.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Etiqueta de recurso de inspección actualizada]

Este módulo de déclencheur inicia un escenario cuando se establece, cambia o elimina el estado de un recurso.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Nombre de webhook de [!UICONTROL]</td> 
   <td> <p> Introduzca el nombre del webhook (por ejemplo: Estado del recurso actualizado).</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Frame.io], vea <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de equipo] </td> 
   <td> <p>Seleccione el equipo para el que se crea este webhook.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ver nuevo recurso]

Este módulo de déclencheur inicia un escenario cuando se crea un nuevo recurso.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Nombre de webhook de [!UICONTROL]</td> 
   <td> <p> Introduzca el nombre del webhook (por ejemplo: Recurso creado).</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Frame.io], vea <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de equipo] </td> 
   <td> <p>Seleccione el equipo para el que se crea este webhook.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Comentarios

* [[!UICONTROL Crear un comentario]](#create-a-comment)
* [[!UICONTROL Eliminar un comentario]](#delete-a-comment)
* [[!UICONTROL Obtener un comentario]](#get-a-comment)
* [[!UICONTROL Enumerar comentarios]](#list-comments)
* [[!UICONTROL Actualizar un comentario]](#update-a-comment)
* [[!UICONTROL Ver comentario actualizado]](#watch-comment-updated)
* [[!UICONTROL Ver nuevo comentario]](#watch-new-comment)

#### [!UICONTROL Crear un comentario]

Este módulo de acción agrega un nuevo comentario o respuesta al recurso.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Frame.io], vea <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo] </td> 
   <td> <p>Seleccione si desea crear un comentario o responder a un comentario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de equipo] </td> 
   <td> <p>Seleccione o asigne el equipo propietario del proyecto que contiene el recurso al que desea agregar un comentario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificador de proyecto] </td> 
   <td> <p>Seleccione el proyecto o asigne el ID del proyecto que contiene el recurso al que desea agregar un comentario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificador de carpeta] </td> 
   <td> <p>Seleccione la carpeta o asigne el ID de la carpeta que contiene el recurso al que desea agregar un comentario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de recurso] </td> 
   <td> <p>Seleccione o asigne el recurso al que desee agregar un comentario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de comentario] </td> 
   <td> <p>Seleccione o asigne el comentario al que desee agregar una respuesta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Texto]</td> 
   <td> <p> Introduzca el contenido de texto del comentario o la respuesta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Marca de tiempo] </td> 
   <td> <p>Introduzca el número de fotograma en el vídeo al que debe estar vinculado el comentario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar un comentario]

Este módulo de acción elimina un comentario existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Frame.io], vea <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de equipo]</td> 
   <td> <p> Seleccione o asigne el equipo propietario del proyecto que contiene el recurso desde el que desea eliminar un comentario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificador de proyecto]</td> 
   <td> <p> Seleccione el proyecto o asigne el ID del proyecto que contiene el recurso desde el que desea eliminar un comentario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificador de carpeta]</td> 
   <td> <p> Seleccione la carpeta que contiene el recurso desde el que desea eliminar un comentario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de recurso] </td> 
   <td> <p>Seleccione el recurso que contiene el comentario que desea eliminar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de comentario] </td> 
   <td> <p>Seleccione el comentario que desea eliminar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener un comentario]

Este módulo de acción recupera los detalles del comentario especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Frame.io], vea <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de equipo] </td> 
   <td> <p>Seleccione o asigne el equipo propietario del proyecto que contiene la carpeta de la que desea recuperar los recursos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificador de proyecto] </td> 
   <td> <p>Seleccione el proyecto que contiene la carpeta de la que desea recuperar los recursos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificador de carpeta] </td> 
   <td> <p>Seleccione la carpeta desde la que desee enumerar los recursos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de recurso] </td> 
   <td> <p>Seleccione el recurso que contiene el comentario que desea recuperar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de comentario] </td> 
   <td> <p>Seleccione el comentario cuyos detalles desee recuperar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Enumerar comentarios]

Este módulo de búsqueda recupera todos los comentarios del recurso especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Frame.io], vea <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de equipo] </td> 
   <td> <p>Seleccione o asigne el equipo propietario del proyecto que contiene la carpeta de la que desea recuperar los comentarios.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificador de proyecto] </td> 
   <td> <p>Seleccione el proyecto que contiene la carpeta de la que desea recuperar los comentarios.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificador de carpeta] </td> 
   <td> <p>Seleccione la carpeta que contiene el recurso cuyos comentarios desea enumerar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de recurso] </td> 
   <td> <p>Seleccione el recurso cuyos comentarios desee enumerar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite] </td> 
   <td> <p>Establezca el número máximo de comentarios que devolverá [!DNL Workfront Fusion] durante un ciclo de ejecución.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actualizar un comentario]

Este módulo de acción edita un comentario existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Frame.io], vea <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de equipo] </td> 
   <td> <p>Seleccione o asigne el equipo propietario del proyecto que contiene el recurso en el que desea actualizar un comentario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificador de proyecto] </td> 
   <td> <p>Seleccione el proyecto \ que contiene el recurso en el que desea actualizar un comentario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificador de carpeta] </td> 
   <td> <p>Seleccione la carpeta que contiene el recurso en el que desea actualizar un comentario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de recurso] </td> 
   <td> <p>Seleccione el recurso en el que desea actualizar un comentario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de comentario] </td> 
   <td> <p>Seleccione el comentario que desea actualizar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Texto]</td> 
   <td> <p> Introduzca el contenido de texto del comentario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Marca de tiempo] </td> 
   <td> <p>Introduzca el número de fotograma en el vídeo al que está vinculado el comentario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ver comentario actualizado]

Este módulo de déclencheur inicia un escenario cuando se edita un comentario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Nombre de webhook de [!UICONTROL] </td> 
   <td> <p>Introduzca el nombre del webhook, por ejemplo: Comentario editado.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Frame.io], vea <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de equipo] </td> 
   <td> <p>Seleccione el equipo para el que se crea este webhook.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ver nuevo comentario]

Este módulo de déclencheur inicia un escenario cuando se crea un nuevo comentario o respuesta.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Nombre de webhook de [!UICONTROL] </td> 
   <td> <p>Introduzca el nombre del webhook, p. ej. Nuevo comentario.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Frame.io], vea <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de equipo] </td> 
   <td> <p>Seleccione el equipo para el que se crea este webhook.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Proyectos

#### [!UICONTROL Lista de proyectos]

Este módulo de búsqueda recupera todos los proyectos del equipo especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Frame.io], vea <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de equipo] </td> 
   <td> <p>Seleccione o asigne el equipo para el que desea recuperar proyectos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite] </td> 
   <td> <p>Establezca el número máximo de proyectos que devolverá [!DNL Workfront Fusion] durante un ciclo de ejecución.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Otro

#### [!UICONTROL Realizar una llamada API]

Este módulo le permite realizar una llamada de API personalizada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Frame.io], vea <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Conectar [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Escriba una ruta relativa a <code>https://api.frame.io</code>. Ejemplo: <code> /v2/teams</code></p> <p>Nota: Para obtener la lista de extremos disponibles, consulte la Referencia de la API [!DNL Frame.io].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Método]</p> </td> 
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada de API. Para obtener más información, vea <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p> <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] agrega encabezados de autorización automáticamente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadena de consulta] </td> 
   <td> <p>Introduzca la cadena de consulta de solicitud. Para cada parámetro que desee incluir en la cadena de consulta, haga clic en <b>[!UICONTROL Agregar elemento]</b> e introduzca el nombre del campo y el valor deseado.</p> </td> 
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

**Ejemplo:** La siguiente llamada de API devuelve todos los equipos y sus detalles en su cuenta de [!DNL Frame.io]:

URL: `/v2/teams`

Método: `GET`

![](assets/api-call-example.png)

El resultado se puede encontrar en Salida del módulo, en Paquete > Cuerpo.

En nuestro ejemplo, se han devuelto los detalles de 1 equipo:

![](assets/api-call-output.png)
