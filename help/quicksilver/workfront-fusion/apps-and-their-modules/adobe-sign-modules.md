---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de Adobe Acrobat Sign
description: Con los módulos  [!DNL Adobe Acrobat Sign] , puedes iniciar un escenario  [!DNL Adobe Workfront Fusion] basado en eventos de tu cuenta de Acrobat Sign [!DNL Adobe] y crear, leer o actualizar acuerdos y otros registros, buscar registros usando los criterios que hayas establecido y cargar documentos.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 01158218-31a6-4c68-a9b7-6a678a8f40c9
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '6652'
ht-degree: 0%

---

# [!DNL Adobe Acrobat Sign] módulos

Con los módulos [!DNL Adobe Acrobat Sign], puede iniciar un escenario [!DNL Adobe Workfront Fusion] basado en los eventos de su cuenta de [!DNL Adobe Acrobat Sign], crear, leer o actualizar acuerdos y otros registros, buscar registros con los criterios que haya establecido y cargar documentos.

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

## Información de la API [!DNL Adobe Acrobat Sign]

El conector de Adobe Acrobat Sign utiliza lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Versión de API</td> 
   <td> v6 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Etiqueta de API</td> 
   <td>Versión 1.35.1</td> 
  </tr>
 </tbody> 
</table>


## [!DNL Adobe Acrobat Sign] recomendaciones de uso del conector

La aplicación [!DNL Adobe Sign] hace que la automatización de los procesos empresariales de firma electrónica en [!DNL Fusion] sea mucho más fácil y eficaz.

Los nuevos usuarios de [!DNL Adobe Sign] deben prestar mucha atención a algunas de las restricciones relacionadas con la actualización de acuerdos. Los acuerdos no suelen cambiarse una vez iniciados. Recomendamos que los nuevos usuarios de [!DNL Adobe Sign] se centren en la creación de nuevos acuerdos mediante el módulo de creación de acuerdos. Esto hará que [!DNL Fusion] automatizaciones sean más sencillas y funcionen mejor con [!DNL Adobe Sign].

[!DNL Adobe Sign] acuerdos necesitan un campo con el que trabajar. Hay algunas opciones para hacerlo, pero la más fácil y común es cargar un documento transitorio y luego asignar ese documento a su acuerdo.

![](assets/adobe-sign-recommendations-350x168.png)

## [!DNL Adobe Acrobat Sign] módulos y sus campos

Al configurar [!DNL Adobe Acrobat Sign] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL Adobe Acrobat Sign] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, vea [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Déclencheur](#triggers)
* [Acciones](#actions)
* [Búsquedas](#searches)

### Déclencheur

<!--
* [Watch for agreements](#watch-for-agreements) 
* [Watch for events](#watch-for-events)
-->

+++ **[!UICONTROL Esté atento a los acuerdos]**

Este módulo de déclencheur inicia un escenario cuando se crea o actualiza un acuerdo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
<td>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Adobe Acrobat Sign] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a></td>  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td>Seleccione si desea inspeccionar registros nuevos, registros actualizados o ambos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro] </td> 
   <td>Seleccione el tipo de registro que desea que vea el registro.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Buscar texto]</td> 
   <td> <p>Introduzca los términos que desea buscar. El módulo devuelve registros que incluyen estos términos como valores de campo.</p> <p>Para obtener más información sobre la búsqueda de campos en [!DNL Adobe Acrobat Sign], consulte "Cómo funciona la búsqueda de texto" en <a href="https://helpx.adobe.com/sign/using/adobesign-search-users-agreements.html#HowSearchWorks">Búsqueda de Adobe Sign: cómo funciona</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de acuerdos devueltos]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Esté atento a los eventos]**

Este módulo de déclencheur inicia un escenario cuando se produce un evento de selección.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td>Seleccione el webhook que desee usar o haga clic en <b>[!UICONTROL Agregar]</b> y rellene los campos siguientes.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nombre de webhook de [!UICONTROL]</td> 
   <td> <p>Escriba un nombre para el webhook</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Adobe Acrobat Sign] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ámbitos]</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Cuenta]</p> </li> 
     <li> <p>[!UICONTROL Grupo]</p> </li> 
     <li> <p>[!UICONTROL Usuario]</p> </li> 
     <li> <p>[!UICONTROL Recurso]</p> <p>Si selecciona [!UICONTROL Resource], introduzca el identificador de recurso y el tipo de recurso.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nivel de recurso]</td> 
   <td> <p>Seleccione el tipo de recurso que desea ver.</p> 
    <ul> 
     <li> <p>[!UICONTROL Acuerdos]</p> </li> 
     <li> <p>[!UICONTROL Widgets]</p> </li> 
     <li> <p>[!UICONTROL MegaAsignaciones]</p> </li> 
     <li> <p>Documentos de la biblioteca [!UICONTROL]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Eventos de suscripción de webhook de [!UICONTROL]</td> 
   <td>Seleccione los [!DNL Adobe Sign] eventos que desea que el módulo vea.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre para mostrar de la aplicación]</td> 
   <td>El nombre para mostrar de la aplicación a través de la cual se crea el webhook.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre de aplicación]</td> 
   <td>El nombre para mostrar de la aplicación a través de la cual se crea el webhook.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Correos electrónicos de notificación de problemas]</td> 
   <td> <p>Esta configuración solo funciona para cuentas de administrador</p> <p>Para cada dirección de correo electrónico a la que desee enviar correos electrónicos de notificación de problemas, haga clic en <b>[!UICONTROL Agregar]</b> e introduzca la dirección de correo electrónico.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Acuerdo parámetros condicionales]</td> 
   <td>Si desea agregar parámetros condicionales, seleccione <b>[!UICONTROL Yes]</b> en el tipo de registro al que desea agregar parámetros y, a continuación, seleccione <b>[!UICONTROL Yes]</b> en cualquier parámetro que desee habilitar.</td> 
  </tr> 
 </tbody> 
</table>

+++

### Acciones

<!--
* [Create a record](#create-a-record) 
* [Create an agreement](#create-an-agreement) 
* [Create related records](#create-related-records) 
* [Custom API Call](#custom-api-call) 
* [List records](#list-records) 
* [Read a record](#read-a-record) 
* [Read related records](#read-related-records) 
* [Update a record](#update-a-record) 
* [Update related record](#update-related-record) 
* [Upload document](#upload-document)
-->

+++ **[!UICONTROL Crear un registro]**

Este módulo de acción crea un nuevo registro del tipo seleccionado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Adobe Acrobat Sign] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td>Añada los encabezados de la solicitud en forma de objeto JSON estándar. Por ejemplo, <code>{"Content-type":"application/json"}</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione el tipo de registro que desea crear.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Group]</b> </p> </li> 
     <li> <p><b>[!UICONTROL Documento de biblioteca]</b> </p> </li> 
     <li> <p><b>[!UICONTROL Usuario]</b> </p> </li> 
     <li> <p><b>[!UICONTROL Formulario web] ([!UICONTROL Widget])</b> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Información de grupo]</td> 
   <td> <p>Introduzca o asigne el [!UICONTROL Name] y el [!UICONTROL ID] del grupo e indique si este grupo es el predeterminado para la cuenta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Información de documento de la biblioteca [!UICONTROL]</td> 
   <td> <p>Rellene los campos siguientes:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Archivos para enviar]</b> </p> <p>Para cada archivo que desee agregar, haga clic en <b>[!UICONTROL Agregar elemento]</b> y rellene los campos.</p> 
      <ul> 
       <li><b>[!UICONTROL ID de documento transitorio]</b> <p>Introduzca el ID del documento transitorio</p> </li> 
       <li> <p><b>[!UICONTROL transferencia de archivo de URL]</b> </p> <p>Rellene los campos siguientes:</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Mime-Type]</b> </p> <p>Introduzca el tipo MIME del archivo original. Los tipos MIME (Extensión multipropósito de correo de Internet) son etiquetas que permiten al software identificar diferentes tipos de datos compartidos en Internet. Los servidores y exploradores web utilizan el tipo MIME para determinar qué se debe hacer con un archivo. Por ejemplo, un archivo con el tipo MIME <code>text/html</code> se procesará en un explorador de forma distinta que un archivo con el tipo MIME <code>image/jpeg</code>.</p> </li> 
         <li> <p><b>[!UICONTROL Nombre]</b> </p> <p>Introduzca un nombre para el archivo.</p> </li> 
         <li> <p><b>[!UICONTROL URL]</b> </p> <p>Escriba la dirección URL del archivo que desea enviar.</p> </li> 
        </ul> </li> 
       <li> <p><b>[!UICONTROL Notarize]</b> </p> <p>Seleccione si este documento debe estar registrado por un notario.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Nombre de plantilla de biblioteca]</b> </p> <p>Introduzca o asigne el nombre de la plantilla de biblioteca</p> </li> 
     <li> <p><b>[!UICONTROL Modo compartido]</b> </p> <p>Especifique quién debe tener acceso al documento de biblioteca.</p> </li> 
     <li> <p><b>[!UICONTROL Estado del documento de la biblioteca]</b> </p> <p>Seleccione si el documento está en estado de creación o activo.</p> </li> 
     <li> <p><b>[!UICONTROL Tipo de plantilla de biblioteca]</b> </p> <p>Para cada tipo de plantilla de biblioteca que desee utilizar, haga clic en <b>[!UICONTROL Agregar elemento]</b> y seleccione el tipo de plantilla.</p> </li> 
     <li> <p><b>[!UICONTROL Última fecha de evento]</b> </p> <p>Introduzca la última fecha en la que se produjo un evento en el documento de biblioteca.</p> <p>Para obtener una lista de los formatos de fecha y hora admitidos, vea <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipos en [!DNL Adobe Workfront Fusion]</a>.</p> </li> 
     <li> <p><b>[!UICONTROL Estado del documento de la biblioteca]</b> </p> <p>Seleccione el estado del documento de biblioteca.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Información de usuario]</td> 
   <td> <p>Rellene los campos siguientes:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Correo electrónico]</b> </p> <p>Introduzca la dirección de correo electrónico del usuario.</p> </li> 
     <li> <p><b>[!UICONTROL Es el administrador de cuentas]</b> </p> <p>Marque esta opción si el usuario creado es administrador de cuentas.</p> </li> 
     <li> <p><b>[!UICONTROL ID de usuario]</b> </p> <p>Introduzca el ID único del usuario</p> </li> 
     <li> <p><b>[!UICONTROL ID de cuenta]</b> </p> <p>Escriba el identificador único de la cuenta de [!DNL Adobe Acrobat Sign] asociada a este usuario.</p> </li> 
     <li> <p><b>[!UICONTROL Nombre]</b> </p> <p>Introduzca el nombre del usuario.</p> </li> 
     <li> <p><b>[!UICONTROL Apellido]</b> </p> <p>Introduzca los apellidos del usuario</p> </li> 
     <li> <p><b>[!UICONTROL Company]</b> </p> <p>Introduzca el nombre de la empresa del usuario.</p> </li> 
     <li> <p><b>[!UICONTROL Iniciales]</b> </p> <p>Introduzca las iniciales del usuario.</p> </li> 
     <li> <p><b>[!UICONTROL Configuración regional]</b> </p> <p>Introduzca la configuración regional del usuario. Determina el idioma de la interfaz de usuario. </p> </li> 
     <li> <p><b>[!UICONTROL Teléfono]</b> </p> <p>Introduzca el número de teléfono del usuario</p> </li> 
     <li> <p><b>Id. de grupo principal</b> </p> <p>Introduzca el grupo al que se agrega el nuevo usuario. Si no se escribe nada, el usuario se agregará al grupo predeterminado de la cuenta.</p> </li> 
     <li> <p><b>[!UICONTROL Puesto]</b> </p> <p>Introduzca el cargo del usuario.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Información de formulario web de [!UICONTROL]</td> 
   <td> <p>Rellene los campos siguientes</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Información de archivo]</b> </p> <p>Para cada archivo que desee agregar al formulario web, haga clic en Add y rellene los campos siguientes:</p> 
      <ul> 
       <li> <p>[!UICONTROL Tipo de archivo]</p> <p>[!UICONTROL Documento]</p> </li> 
       <li> <p>[!UICONTROL Documento transitorio]</p> </li> 
       <li> <p>[!UICONTROL Información de archivo de URL]</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Nombre de formulario web]</b> </p> <p>Introduzca un nombre para el formulario web. Este nombre se utiliza para identificar el formulario web en lugares como correos electrónicos y sitios web.</p> </li> 
     <li> <p><b>[!UICONTROL estado del formulario web]</b> </p> <p>Seleccione el estado en el que se debe crear el nuevo formulario web.</p> </li> 
     <li> <p><b>[!UICONTROL Información del conjunto de participantes del formulario web]</b> </p> 
      <ul> 
       <li> <p><b>[!UICONTROL Información de miembro]</b> </p> <p>Para cada miembro que desee agregar al conjunto de participantes, haga clic en <b>[!UICONTROL Agregar elemento]</b>. </p> 
        <ul> 
         <li> <p><b>[!UICONTROL Correo electrónico]</b> </p> <p>Deje esta opción en blanco.</p> </li> 
         <li> <p><b>[!UICONTROL Opción de seguridad]</b> </p> <p>Si desea agregar una opción de seguridad para autenticar a este usuario, seleccione <b>[!UICONTROL Yes]</b>, luego seleccione la opción de seguridad y rellene los campos que requiera.</p> </li> 
        </ul> </li> 
       <li> <p><b>[!UICONTROL Rol]</b> </p> <p>Seleccione la función. Todos los miembros de este conjunto de participantes comparten la función.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL formulario web información de conjuntos de participantes adicionales]</b> </p> 
      <ul> 
       <li> <p><b>[!UICONTROL Información de miembro]</b> </p> <p>Para cada miembro que desee agregar al conjunto de participantes, haga clic en <b>[!UICONTROL Agregar elemento]</b>.</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Correo electrónico]</b> </p> <p>Deje esta opción en blanco.</p> </li> 
         <li> <p><b>[!UICONTROL Opción de seguridad]</b> </p> <p>Si desea agregar una opción de seguridad para autenticar a este usuario, seleccione <b>[!UICONTROL Yes]</b>, luego seleccione la opción de seguridad y rellene los campos que requiera.</p> </li> 
        </ul> </li> 
       <li> <p><b>[!UICONTROL Rol]</b> </p> </li> 
       <li> <p><b>[!UICONTROL ID de participante de formulario web] </b> </p> <p>Introduzca el ID del participante del formulario web.</p> </li> 
       <li> <p><b>[!UICONTROL Pedido]</b> </p> <p>Especifique el orden en que este conjunto de participantes debe interactuar con el formulario web. Por ejemplo, el grupo de participantes que tiene un valor de pedido de 1 debe ir primero, 2 debe ir después, y así sucesivamente. Los números de pedido deben comenzar por uno y no deben haber espacios en la serie. </p> </li> 
       <li> <p><b>[!UICONTROL Información del conjunto de participantes del proveedor]</b> </p> <p>Si se desconoce el participante, introduzca si el proveedor debe proporcionar los detalles del participante e introduzca un mensaje con los detalles necesarios para el participante desconocido.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Información de error de autenticación]</b> </p> <p>Si desea proporcionar una página de error o error para los usuarios, seleccione <b>[!UICONTROL Yes]</b> y rellene los campos siguientes:</p> 
      <ul> 
       <li> <p><b>[!UICONTROL URL]</b> </p> <p>Introduzca la dirección URL de la página de error</p> </li> 
       <li> <p><b>[!UICONTROL Deframe]</b> </p> <p>Active esta opción si desea que la página de error aparezca dentro del formulario web</p> </li> 
       <li> <p><b>[!UICONTROL Retardo]</b> </p> <p>Introduzca el retraso, en segundos, antes de redirigir al usuario a la página de error.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL CC info]</b> </p> <p>Para cada dirección de correo electrónico que desee recibir un correo electrónico cuando se firme el acuerdo final en el formulario web, haga clic en <b>[!UICONTROL Agregar elemento]</b> e introduzca la dirección de correo electrónico.</p> </li> 
     <li> <p><b>[!UICONTROL Información de finalización]</b> </p> <p style="font-style: normal;">Si desea proporcionar una página de éxito para los usuarios, seleccione <b>[!UICONTROL Yes]</b> y rellene los campos siguientes:</p> 
      <ul> 
       <li> <p><b>[!UICONTROL URL]</b> </p> <p>Introduzca la URL de la página de éxito</p> </li> 
       <li> <p><b>[!UICONTROL Deframe]</b> </p> <p>Active esta opción si desea que la página de éxito aparezca dentro del formulario web</p> </li> 
       <li> <p><b>[!UICONTROL Retardo]</b> </p> <p>Introduzca el retraso, en segundos, antes de que el usuario sea redirigido a la página de éxito.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Id. de grupo]</b> </p> <p>Introduzca el ID del grupo al que pertenece el formulario web. Si no se introduce nada, el formulario web pertenece al grupo principal del usuario de la cuenta.</p> </li> 
     <li> <p><b>[!UICONTROL Última fecha de evento]</b> </p> <p>Introduzca la fecha en la que se produjo el último evento en el formulario web. Usar el formato <code>yyyy-MM-dd'T'HH:mm:ssZ</code>.</p> </li> 
     <li> <p><b>[!UICONTROL Configuración regional]</b> </p> <p>Introduzca la configuración regional del usuario. Determina el idioma de la interfaz de usuario. </p> </li> 
     <li> <p><b>[!UICONTROL opción de seguridad]n</b> </p> <p>Introduzca la contraseña utilizada para proteger el documento. Debe comunicar esta contraseña por separado a las partes relevantes.</p> </li> 
     <li> <p><b>[!UICONTROL Información de almacenamiento en depósito]</b> </p> <p>Si la cuenta está configurada para el almacenamiento de documentos y la opción para habilitar por acuerdo, puede activar esta opción para almacenar este acuerdo en el almacén.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Crear un acuerdo]**

Este módulo de acción crea un acuerdo, lo envía para su firma y devuelve el ID del acuerdo.

>[!NOTE]
>
>Se recomienda cargar el documento para firmar como documento transitorio y, a continuación, asignarlo al campo [!UICONTROL Archivo para enviar] en el módulo [!UICONTROL Crear un acuerdo]. Por ejemplo, consulte &quot;Cargar documento&quot; en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
<td>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Adobe Acrobat Sign] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a></td>  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td>Añada los encabezados de la solicitud en forma de objeto JSON estándar. Por ejemplo, <code>{"Content-type":"application/json"}</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivos para enviar]</td> 
   <td> <p>Para cada elemento que desee incluir en el acuerdo, haga clic en <b>[!UICONTROL Agregar elemento]</b> y rellene los campos siguientes:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Tipo de archivo]</b> </p> 
      <ul> 
       <li> <p><b>[!UICONTROL Documento]</b> </p> <p>Rellene los campos siguientes:</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Fecha de creación]</b> </p> <p>Escriba o asigne la fecha de creación del documento con el formato <code>yyyy-MM-dd'T'HH:mm:ssZ</code>. Por ejemplo, <code>2016-02-25T18:46:19Z</code> representa la hora UTC.</p> </li> 
         <li> <p><b>[!UICONTROL ID]</b> </p> <p>Introduzca o asigne el ID del documento.</p> </li> 
         <li> <p><b>[!UICONTROL Etiqueta]</b> </p> <p>Introduzca o asigne una etiqueta única para el archivo. En el caso del flujo de trabajo personalizado, esto asigna un archivo al elemento de archivo correspondiente en la definición del flujo de trabajo. Esto debe especificarse en caso de solicitud de creación de acuerdo de flujo de trabajo personalizado.</p> </li> 
         <li> <p><b>[!UICONTROL Número de páginas]</b> </p> <p>Introduzca o asigne el número de páginas del documento.</p> </li> 
         <li> <p><b>[!UICONTROL Mime-Type]</b> </p> <p>Introduzca o asigne el tipo MIME del archivo original. Los tipos MIME (Extensión multipropósito de correo de Internet) son etiquetas que permiten al software identificar diferentes tipos de datos compartidos en Internet. Los servidores y exploradores web utilizan el tipo MIME para determinar qué se debe hacer con un archivo. Por ejemplo, un archivo con el tipo MIME <code>text/html</code> se procesará en un explorador de forma distinta que un archivo con el tipo MIME <code>image/jpeg</code>.</p> </li> 
         <li> <p><b>[!UICONTROL Nombre]</b> </p> <p>Escriba o asigne un nombre para el documento.<br></p> </li> 
        </ul> </li> 
       <li> <p><b>[!UICONTROL Id. de documento de biblioteca]</b> </p> <p>Introduzca el ID del documento de biblioteca</p> </li> 
       <li> <p><b>[!UICONTROL ID de documento transitorio]</b> </p> <p>Introduzca el ID del documento transitorio</p> </li> 
       <li> <p><b>[!UICONTROL transferencia de archivo de URL]</b> </p> <p>Rellene los campos siguientes:</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Mime-Type]</b> </p> <p>Introduzca el tipo MIME del archivo original. Los tipos MIME (Extensión multipropósito de correo de Internet) son etiquetas que permiten al software identificar diferentes tipos de datos compartidos en Internet. Los servidores y exploradores web utilizan el tipo MIME para determinar qué se debe hacer con un archivo. Por ejemplo, un archivo con el tipo MIME <code>text/html</code> se procesará en un explorador de forma distinta que un archivo con el tipo MIME <code>image/jpeg</code>.</p> </li> 
         <li> <p><b>[!UICONTROL Nombre]</b> </p> <p>Introduzca un nombre para el archivo.</p> </li> 
         <li> <p><b>[!UICONTROL URL]</b> </p> <p>Escriba la dirección URL del archivo que desea enviar.</p> </li> 
        </ul> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Etiqueta]</b> </p> <p>Introduzca una etiqueta para el archivo.</p> </li> 
     <li> <p><b>[!UICONTROL Notarize]</b> </p> <p>Active esta opción para indicar que el archivo debe estar certificado por un notario.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL nombre del contrato]</td> 
   <td>Introduzca un nombre para el nuevo acuerdo. Este nombre se utiliza para identificar el acuerdo en lugares como correos electrónicos y sitios web.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Participante establece información]</td> 
   <td> <p>Para cada conjunto de participantes que desee agregar, haga clic en <b>[!UICONTROL Agregar elemento]</b> y rellene los campos siguientes.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Miembros]</b> </p> <p>Para cada persona que desee agregar al conjunto de participantes, haga clic en <b>[!UICONTROL Agregar elemento]</b> e introduzca la dirección de correo electrónico de la persona.</p> </li> 
     <li> <p><b>[!UICONTROL Pedido]</b> </p> <p>Especifique el orden en que este conjunto de participantes debe firmar el acuerdo. Por ejemplo, el grupo de participantes que tiene el valor de un pedido de 1 debe firmar primero, 2 debe firmar después, y así sucesivamente. Los números de pedido deben comenzar por uno y no deben haber espacios en la serie. </p> </li> 
     <li> <p><b>[!UICONTROL Rol]</b> </p> <p>Seleccione un rol para este conjunto de participantes. Todos los participantes en el conjunto reciben esta función.</p> </li> 
     <li> <p><b>[!UICONTROL ID]</b> </p> <p>Introduzca o asigne el ID de este conjunto de participantes.</p> </li> 
     <li> <p><b>[!UICONTROL Etiqueta]</b> </p> <p>Introduzca o asigne una etiqueta única para el juego de participantes. Para los flujos de trabajo personalizados, la etiqueta especificada en el conjunto de participación debe asignarla al paso de participación en el flujo de trabajo personalizado.</p> </li> 
     <li> <p><b>[!UICONTROL Nombre]</b> </p> <p>Introduzca un nombre para el juego de participantes. Este nombre debe ser único dentro del acuerdo.</p> </li> 
     <li> <p><b>[!UICONTROL Mensaje privado]</b> </p> <p>Introduzca o asigne un mensaje para este juego de participantes. Todos los participantes en el conjunto reciben este mensaje.</p> </li> 
     <li> <p><b>[!UICONTROL Páginas visibles]</b> </p> <p>Si la visibilidad limitada del documento está habilitada para este contrato, especifique qué archivos son visibles para este conjunto de participantes. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de firma]</td> 
   <td> <p>Seleccione el tipo de firma que requiere el acuerdo.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Firma electrónica]</b> </p> <p>El acuerdo debe firmarse electrónicamente.</p> </li> 
     <li> <p><b>[!UICONTROL Escrito]</b> </p> <p>El acuerdo debe firmarse a mano y el acuerdo firmado debe analizarse y cargarse.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Estado]</td> 
   <td> <p>Seleccione un estado para este acuerdo.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Creación]</b> </p> <p>Aún puede editar o agregar campos a este acuerdo.</p> </li> 
     <li> <p><b>[!UICONTROL Borrador]</b> </p> <p>Puede generar gradualmente este acuerdo antes de enviarlo.</p> </li> 
     <li> <p><b>[!UICONTROL En Proceso]</b> </p> <p>Este acuerdo se enviará inmediatamente.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL CC]</td> 
   <td> <p>Puede enviar este acuerdo a las partes interesadas que no necesiten firmarlo, como las partes interesadas. Reciben un correo electrónico al principio del proceso de firma y otro cuando se recibe la firma final. También reciben una copia del acuerdo para el PDF. </p> <p>Para cada persona que desee incluir en la copia de seguridad de este contrato, haga clic en <b>[!UICONTROL Agregar elemento]</b> y rellene los campos siguientes:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Correo electrónico]</b> </p> <p>Introduzca o asigne la dirección de correo electrónico que desea que aparezca en el contrato.</p> </li> 
     <li> <p><b>[!UICONTROL Etiqueta]</b> </p> <p>Introduzca o asigne una etiqueta para esta dirección de correo electrónico, tal como se ve en la descripción del flujo de trabajo</p> </li> 
     <li> <p><b>[!UICONTROL Páginas visibles]</b> </p> </li> 
     <li> <p>Si la visibilidad limitada del documento está habilitada para este contrato, especifique qué archivos son visibles para este conjunto de participantes. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email option]</td> 
   <td> <p>Para cada tipo de correo electrónico, seleccione si ese tipo de correo se envía a todos los participantes o ninguno.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Correos electrónicos de finalización]</b> </p> <p>Enviar un correo electrónico cuando se complete, cancele, caduque o rechace este acuerdo.</p> </li> 
     <li> <p><b>[!UICONTROL Correos electrónicos en vuelo]</b> </p> <p>Se envía un correo electrónico cuando se delega o reemplaza este acuerdo.</p> </li> 
     <li> <p><b>[!UICONTROL Correos electrónicos de inicio del acuerdo]</b> </p> <p>Enviar un correo electrónico cuando se cree este acuerdo o cuando se solicite una acción.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID externo]</td> 
   <td> <p>Introduzca o asigne un ID para este acuerdo. Puede especificarlo cuando se cree el acuerdo y utilizarlo para ubicarlo en módulos o consultas posteriores.</p> <p>Nota: El valor ID externo es visible para todos los participantes a través de la API, por lo que no debe utilizarse para contener un token confidencial.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Combinar información de campo]</td> 
   <td> <p>Para cada campo del acuerdo para el que desee colocar un valor predeterminado, haga clic en <b>[!UICONTROL Agregar elemento]</b> e introduzca el valor predeterminado y el nombre del campo.</p> <p>Los valores se presentarán a los firmantes para los campos editables. Para los campos de solo lectura, los valores proporcionados no se podrán editar durante el proceso de firma.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Información de notario]</td> 
   <td> <p>Rellene los campos siguientes:</p> 
    <ul> 
     <li> <p><b>[!Cita UICONTROL]</b> </p> <p>Introduzca o asigne una fecha y hora propuestas para la cita con el notariado de este acuerdo.</p> </li> 
     <li> <p><b>[!UICONTROL Nota]</b> </p> <p>Introduzca o asigne las notas que desee incluir sobre la sesión del notario.</p> </li> 
     <li> <p><b>[!UICONTROL Pago]</b> </p> <p>Seleccione si el firmante o el remitente del acuerdo pagan al notario.</p> </li> 
     <li> <p><b>[!UICONTROL Notary Type]</b> </p> <p>Seleccione el tipo de notario</p> 
      <ul> 
       <li> <p>[!UICONTROL Proveedor notario]</p> <p>El notario es proporcionado por el notario.</p> </li> 
       <li> <p>[!UICONTROL BYON notario]</p> <p>El notario es proporcionado por el cliente.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Opción [!UICONTROL Post sign]</td> 
   <td> <p>Seleccione si desea que los firmantes se dirijan a una página de éxito después de firmar el acuerdo. Si selecciona <b>[!UICONTROL Sí]</b>, rellene los campos siguientes:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Retraso de redirección]</b> </p> <p>Introduzca o asigne un número que represente el número de segundos antes de que el firmante se redirija a la página de éxito. Si este valor es mayor que 0, el usuario verá primero el mensaje de éxito estándar de [!DNL Adobe Sign] y, después de un retraso, se le redirigirá a la página de éxito.</p> </li> 
     <li> <p><b>[!UICONTROL URL de redireccionamiento]</b> </p> <p>Introduzca o asigne una URL de acceso público a la que se enviará al usuario después de completar correctamente el proceso de firma.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Opción de seguridad]</td> 
   <td> <p>Introduzca o asigne la contraseña secundaria que se utilizará para proteger el documento de PDF. </p> <p>Importante: [!DNL Adobe Sign] nunca compartirá esta contraseña, por lo que debe comunicarla por separado a las partes relevantes.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Información de salto]</td> 
   <td>Si la cuenta está configurada para el almacenamiento de documentos y la opción para habilitar por acuerdo, puede activar esta opción para almacenar este acuerdo en el almacén.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Crear registros relacionados]**

Este módulo de acción crea registros vinculados a un módulo seleccionado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Adobe Acrobat Sign] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p> <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] agrega encabezados de autorización automáticamente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td>Seleccione el tipo de registro del registro original con el que desea asociar los registros creados.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Agreement]/[!UICONTROL Library document]/[!UICONTROL User]/[!UICONTROL Widget ID]</td> 
   <td>Introduzca o asigne el ID del objeto con el que desea asociar el registro creado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campo relacionado con el acuerdo]</td> 
   <td> <p>Seleccione el tipo de campo relacionado que desea crear</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Campos de formulario]</b> </p> <p>Introduzca el ID de plantilla de la plantilla que contiene los campos que desea crear</p> </li> 
     <li> <p><b>[!UICONTROL Recordatorios]</b> </p> <p>Rellene los campos siguientes:</p> 
      <ul> 
       <li> <p><b>[!UICONTROL ID de participante de destinatario]</b> </p> <p>Para cada participante al que desee enviar un recordatorio, haga clic en [!UICONTROL Agregar elemento] e introduzca el ID del participante.</p> </li> 
       <li> <p><b>[!UICONTROL Estado]</b> </p> <p>Para los registros nuevos, el estado debe ser [!UICONTROL Active].</p> </li> 
       <li> <p><b>[!UICONTROL Primera demora de recordatorio]</b> </p> <p>Introduzca el retraso en horas antes de enviar el primer recordatorio. El valor mínimo permitido es 1 hora y el valor máximo no puede ser mayor que la diferencia entre la creación del acuerdo y la hora de caducidad del acuerdo en horas. Si no se establece este retraso, el primer recordatorio se basará en la frecuencia.</p> </li> 
       <li> <p><b>[!UICONTROL Frecuencia de recordatorio]</b> </p> <p>Defina la frecuencia con la que desea que se envíe el recordatorio. Si no se proporciona la frecuencia, el recordatorio se enviará una vez.</p> </li> 
       <li> <p><b>[!UICONTROL Última fecha de envío]</b> </p> <p>El sistema establece este campo.</p> </li> 
       <li> <p><b>[!UICONTROL Siguiente fecha de envío]</b> </p> <p>Este campo debe estar en blanco o establecido en [!UICONTROL ONCE].</p> </li> 
       <li> <p><b>[!UICONTROL Nota]</b> </p> <p>Introduzca una nota para incluirla en el recordatorio. Esto resulta útil para indicar al participante por qué se requiere su participación.</p> </li> 
       <li> <p><b>[!UICONTROL Iniciar contador de recordatorio desde]</b> </p> <p>Seleccione si el recordatorio se enviará en función del momento en el que se crea el acuerdo cuando esté disponible.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Informe de identidad del signatario]</b> </p> <p>Introduzca la contraseña utilizada para proteger el documento de PDF.</p> </li> 
     <li> <p><b>[!UICONTROL Vistas]</b> </p> <p>Introduzca los campos siguientes</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Nombre]</b> </p> <p>Seleccione el nombre de la vista que desee crear.</p> </li> 
       <li> <p><b>[!UICONTROL Usuario de inicio de sesión automático]</b> </p> <p>Seleccione <b>[!UICONTROL Yes]</b> para iniciar sesión automáticamente en la dirección URL devuelta.</p> </li> 
       <li> <p><b>[!UICONTROL Frame Parent]</b> </p> <p>Introduzca o asigne una lista separada por comas de direcciones URL de dominio principal en la que se pueden ienmarcar las direcciones URL devueltas. Si se deja vacío, las páginas de [!DNL Adobe Acrobat Sign] no se podrán ver en el iframe.</p> </li> 
       <li> <p><b>[!UICONTROL Configuración regional]</b> </p> <p>Introduzca el idioma en el que desea crear la vista. </p> </li> 
       <li> <p><b>[!UICONTROL Sin indicador de Chrome]</b> </p> <p>Seleccione <b>[!UICONTROL Yes]</b> para mostrar la página incrustada sin un encabezado o pie de página de exploración.</p> </li> 
       <li> <p><b>[!UICONTROL Puede editar archivos]</b> </p> <p>Seleccione <b>[!UICONTROL Yes]</b> si desea que la sección de carga de archivos se edite agregando o quitando archivos. Este no es un mecanismo de control de acceso. El valor predeterminado es [!UICONTROL Sí].</p> </li> 
       <li> <p><b>[!UICONTROL Documento de biblioteca]</b> </p> <p>Seleccione <b>[!UICONTROL Yes]</b> si desea que los vínculos de documentos de biblioteca estén visibles. El valor predeterminado es [!UICONTROL Sí].</p> </li> 
       <li> <p><b>[!UICONTROL Archivo local]</b> </p> <p>Seleccione <b>[!UICONTROL Yes]</b> si desea que aparezca el botón de carga del archivo local. El valor predeterminado es [!UICONTROL Sí].</p> </li> 
       <li> <p><b>[!UICONTROL Conectores web]</b> </p> <p>Seleccione <b>[!UICONTROL Yes]</b> si desea que aparezcan los vínculos para adjuntar documentos de orígenes web. El valor predeterminado es Sí.</p> </li> 
       <li> <p><b>[!UICONTROL está seleccionada como vista previa]</b> </p> <p>Seleccione <b>[!UICONTROL Yes]</b> para establecer la página de composición en modo de creación.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Member share]</b> </p> <p>Para cada miembro con el que desee compartir el acuerdo, haga clic en <b>[!UICONTROL Agregar elemento]</b> e introduzca la dirección de correo electrónico del miembro y un mensaje para ese miembro.</p> </li> 
     <li> <p>[!UICONTROL Delegar conjunto de participantes]</p> 
      <ul> 
       <li> <p><b>[!UICONTROL ID del conjunto de participantes]</b> </p> <p>Introduzca el ID del juego de participantes</p> </li> 
       <li> <p><b>[!UICONTROL Información de miembro]</b> </p> <p>Para cada miembro que desee agregar, haga clic en [!UICONTROL Agregar elemento] e introduzca la dirección de correo electrónico y la información de teléfono del miembro.</p> </li> 
       <li> <p><b>[!UICONTROL Mensaje privado]</b> </p> <p>Introduzca un mensaje. Todos los miembros del conjunto de participantes reciben este mensaje.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Información de vista de biblioteca]</td> 
   <td> <p>Rellene los campos siguientes:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Nombre]</b> </p> <p>Introduzca un nombre para la plantilla de biblioteca. Este nombre se utiliza en correos electrónicos y sitios web.</p> </li> 
     <li> <p><b>[!UICONTROL Usuario de inicio de sesión automático]</b> </p> <p>Seleccione <b>[!UICONTROL Yes]</b> para iniciar sesión automáticamente en la dirección URL devuelta.</p> </li> 
     <li> <p><b>[!UICONTROL Frame parent]</b> </p> <p>Introduzca o asigne una lista separada por comas de direcciones URL de dominio principal en la que se pueden ienmarcar las direcciones URL devueltas. Si se deja vacío, las páginas de [!DNL Adobe Acrobat Sign] no se podrán ver en el iframe.</p> </li> 
     <li> <p><b>[!UICONTROL Configuración regional]</b> </p> <p>Introduzca el idioma en el que desea crear la vista. </p> </li> 
     <li> <p><b>[!UICONTROL Sin indicador de Chrome]</b> </p> <p>Seleccione <b>[!UICONTROL Yes]</b> para mostrar la página incrustada sin un encabezado o pie de página de exploración.</p> </li> 
     <li> <p><b>[!UICONTROL Enviar configuración de vista]</b> </p> <p>Seleccione <b>[!UICONTROL Yes]</b> si desea configurar la vista de [!UICONTROL Send] y, a continuación, rellene los campos siguientes.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL nombre del contrato]</b> </p> <p>Introduzca o asigne el nombre del acuerdo para el documento de biblioteca en la página de redacción.</p> </li> 
       <li> <p><b>[!UICONTROL Puede editar archivos]</b> </p> <p>Seleccione <b>[!UICONTROL Yes]</b> si desea que la sección de carga de archivos se edite agregando o quitando archivos. Este no es un mecanismo de control de acceso. El valor predeterminado es [!UICONTROL Sí].</p> </li> 
       <li> <p><b>[!UICONTROL Archivo local]</b> </p> <p>Seleccione <b>[!UICONTROL Yes]</b> si desea que los vínculos de documentos de biblioteca estén visibles. El valor predeterminado es [!UICONTROL Sí].</p> </li> 
       <li> <p><b>[!UICONTROL Conectores web]</b> </p> <p>Seleccione <b>[!UICONTROL Yes]</b> si desea que aparezcan los vínculos para adjuntar documentos de orígenes web. El valor predeterminado es [!UICONTROL Sí].</p> </li> 
       <li> <p><b>Vista previa seleccionada</b> </p> <p>Seleccione <b>[!UICONTROL Yes]</b> para establecer la página de composición en modo de creación.</p> </li> 
      </ul> <p> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Información de vista de usuario]</td> 
   <td> <p>Rellene los campos siguientes</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Nombre]</b> </p> <p>Seleccione el nombre de la vista de usuario solicitada.</p> </li> 
     <li> <p><b>[!UICONTROL Usuario de inicio de sesión automático]</b> </p> <p>Seleccione <b>[!UICONTROL Yes]</b> para iniciar sesión automáticamente con el usuario. Seleccione <b>[!UICONTROL No]</b> para requerir credenciales. El valor predeterminado es [!UICONTROL No].</p> </li> 
     <li> <p><b>[!UICONTROL Frame parent]</b> </p> <p>Introduzca o asigne una lista separada por comas de direcciones URL de dominio principal en la que se pueden ienmarcar las direcciones URL devueltas. Si se deja vacío, las páginas de [!DNL Adobe Acrobat Sign] no se podrán ver en el iframe.</p> </li> 
     <li> <p><b>Sin indicador de Chrome</b> </p> <p>Seleccione <b>[!UICONTROL Yes]</b> para mostrar la página incrustada sin un encabezado o pie de página de exploración.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Widget campos relacionados]</td> 
   <td> <p>Seleccione el registro relacionado que desea crear.</p> 
    <ul> 
     <li> <p>[!UICONTROL Vistas]</p> <p>Rellene los campos siguientes.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Nombre]</b> </p> <p>Seleccione el nombre de la vista de formulario web solicitada</p> </li> 
       <li> <p><b>[!UICONTROL Usuario de inicio de sesión automático]</b> </p> <p>Seleccione <b>[!UICONTROL Yes]</b> para iniciar sesión automáticamente con el usuario. Seleccione <b>[!UICONTROL No]</b> para requerir credenciales. El valor predeterminado es [!UICONTROL No].</p> </li> 
       <li> <p><b>[!UICONTROL Frame parent]</b> </p> <p>Introduzca o asigne una lista separada por comas de direcciones URL de dominio principal en la que se pueden ienmarcar las direcciones URL devueltas. Si se deja vacío, las páginas de [!DNL Adobe Acrobat Sign] no se podrán ver en el iframe.</p> </li> 
       <li> <p><b>[!UICONTROL Configuración regional]</b> </p> <p>Introduzca el idioma en el que desea crear la vista. </p> </li> 
       <li> <p><b>[!UICONTROL Sin indicador de Chrome]</b> </p> <p>Seleccione <b>[!UICONTROL Yes]</b> para mostrar la página incrustada sin un encabezado o pie de página de exploración.</p> </li> 
       <li> <p>[!UICONTROL Configuración de vista de firma personalizada]</p> <p>Si desea configurar una vista de firma personalizada, seleccione <b>[!UICONTROL Yes]</b> y rellene los campos siguientes:</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Correo electrónico]</b> </p> <p>Introduzca la dirección de correo electrónico de la persona que recibe el formulario web recién creado</p> </li> 
         <li> <p><b>[!UICONTROL Comentario]</b> </p> <p>Escriba un comentario que describa cómo el llamador de la API estableció la identidad del firmante. Esta información aparece en la pista de auditoría [!DNL Adobe Acrobat Sign].</p> </li> 
         <li> <p><b>[!UICONTROL Expiration]</b> </p> <p>Introduzca una fecha de caducidad para la personalización de este formulario web. </p> <p>Para obtener una lista de los formatos de fecha y hora admitidos, vea <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">Coerción de tipos en [!DNL Adobe Workfront Fusion]</a>.</p> </li> 
         <li> <p><b>[!UICONTROL Reutilizable]</b> </p> <p>Seleccione <b>[!UICONTROL Yes]</b> si desea que el firmante deseado pueda firmar el formulario más de una vez.</p> </li> 
        </ul> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Member share]</b> </p> <p>Para cada miembro con el que desee compartir el acuerdo, haga clic en <b>[!UICONTROL Agregar elemento]</b> e introduzca la dirección de correo electrónico del miembro y un mensaje para ese miembro.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Llamada de API personalizada]**
Este módulo le permite realizar una llamada de API personalizada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Adobe Acrobat Sign] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Introduzca una ruta relativa a <code>https://api.[region].adobesign.com/api/rest/v6/</code></p> <p>Nota: Para obtener la lista de extremos disponibles, consulte la Referencia de la API [!DNL Adobe Sign].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Método]</p> </td> 
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada de API. Para obtener más información, vea <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p> <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] agrega encabezados de autorización automáticamente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadena de consulta] </td> 
   <td> <p>Introduzca la cadena de consulta de solicitud.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cuerpo]</td> 
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Cuando utilice afirmaciones condicionales como <code>if</code> en su JSON, coloque las comillas fuera de la afirmación condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cargar un documento transitorio]</td> 
   <td> <p>Si desea cargar un documento transitorio, introduzca el archivo de origen del documento que desea cargar.</p> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Enumerar registros]**

Este módulo de acción enumera todos los registros del tipo seleccionado a los que la cuenta tiene acceso.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Adobe Acrobat Sign] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p> <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] agrega encabezados de autorización automáticamente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td>Seleccione el tipo de registro para el que desea recuperar registros relacionados.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Configuración regional]</td> 
   <td> <p>Introduzca la configuración regional del usuario. Determina el idioma de la interfaz de usuario. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID externo]</td> 
   <td>Introduzca o asigne el ID externo (un ID asignado fuera de [!DNL Adobe Acrobat Sign]) para los contratos que desea devolver.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de grupo]</td> 
   <td>Introduzca el ID del grupo asociado con los registros que desea enumerar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostrar ocultos (registros)]</td> 
   <td>Active esta opción si desea incluir registros ocultos en los resultados.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cursor] / [!UICONTROL Índice de inicio]</td> 
   <td> <p>Introduzca el número del primer registro que debe devolver el módulo. </p> <p>Nota: Este campo se combina con el campo [!UICONTROL Número máximo de registros devueltos] para la paginación. Por ejemplo, si el [!UICONTROL Número máximo de eventos devueltos] es 100 y el [!UICONTROL Índice de inicio] es 101, el módulo devuelve los registros 101-200 o la segunda página de resultados.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de registros devueltos]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo [action] ejecute durante cada ciclo de ejecución de escenario.</p> <p>Nota: Este campo se combina con el campo [!UICONTROL Cursor] o [!UICONTROL Start Index] para la paginación. Por ejemplo, si el [!UICONTROL Número máximo de eventos devueltos] es 100 y el [!UICONTROL Índice de inicio] es 101, el módulo devuelve los registros 101-200 o la segunda página de resultados.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL de dominio principal]</td> 
   <td> <p>Introduzca o asigne una lista separada por comas de direcciones URL de dominio principal en la que se pueden ienmarcar las direcciones URL devueltas. Si se deja vacío, las páginas de [!DNL Adobe Acrobat Sign] no se podrán ver en el iframe.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Leer un registro]**

Este módulo de acción recupera información de un único registro.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Adobe Acrobat Sign] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p> <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] agrega encabezados de autorización automáticamente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td>Seleccione el tipo de registro para el que desea recuperar registros relacionados.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de registro]</td> 
   <td>Introduzca o asigne el ID del registro que desea recuperar.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Leer registros relacionados]**

Leer información adicional relacionada con un único registro.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Adobe Acrobat Sign] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p> <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] agrega encabezados de autorización automáticamente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td>Seleccione el tipo de registro para el que desea recuperar registros relacionados.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record ID] (Ejemplo: [!UICONTROL Account ID])</td> 
   <td>Introduzca o asigne el ID del registro para el que desea recuperar registros relacionados.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Otros campos]</td> 
   <td>Introduzca información en campos específicos basados en el tipo de registro y campos relacionados.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Actualizar un registro]**

Este módulo de acción actualiza un único registro en [!DNL Adobe Acrobat Sign].

>[!IMPORTANT]
>
>* Como práctica recomendada, si prevé realizar cambios sustanciales en un acuerdo, le recomendamos que cree un nuevo acuerdo en lugar de actualizar el existente.
>* Algunas actualizaciones incluyen campos obligatorios. A medida que configure la actualización, asegúrese de completar todos los campos obligatorios. Los campos obligatorios están en negrita en [!DNL Workfront Fusion] módulos.
>



<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Adobe Acrobat Sign] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p> <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] agrega encabezados de autorización automáticamente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de registro] </td> 
   <td>Introduzca o asigne el ID del registro que desea actualizar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td>Seleccione el tipo de registro que desea actualizar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Otros campos]</td> 
   <td> <p>Introduzca información en campos específicos basados en el tipo de registro y campos relacionados.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Acuerdo]</b> </p> <p>Como práctica recomendada, si prevé realizar cambios sustanciales en un acuerdo, le recomendamos que cree un nuevo acuerdo en lugar de actualizar el existente.</p> </li> 
     <li> <p><b>[!UICONTROL Documento de biblioteca]</b> </p> <p>Seleccione los campos que desea actualizar y rellene los campos seleccionados:</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Estado]</b> </p> <p>Seleccione el nuevo estado del documento de biblioteca.</p> </li> 
       <li> <p><b>[!UICONTROL Nombre]</b> </p> <p>Introduzca o asigne el nombre de la plantilla de biblioteca</p> </li> 
       <li> <p><b>[!UICONTROL Modo compartido]</b> </p> <p>Especifique quién debe tener acceso al documento de biblioteca.</p> </li> 
       <li> <p><b>[!UICONTROL Tipo de plantilla de biblioteca]</b> </p> <p>Para cada tipo de plantilla de biblioteca que desee utilizar, haga clic en <b>[!UICONTROL Agregar elemento]</b> y seleccione el tipo de plantilla.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Usuario]</b> </p> <p>Seleccione los campos que desea actualizar y rellene los campos seleccionados:</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Nombre]</b> </p> <p>Introduzca el nombre del usuario.</p> </li> 
       <li> <p><b>[!UICONTROL Apellido]</b> </p> <p>Introduzca los apellidos del usuario</p> </li> 
       <li> <p><b>[!UICONTROL Company]</b> </p> <p>Introduzca el nombre de la empresa del usuario.</p> </li> 
       <li> <p><b>[!UICONTROL Teléfono]</b> </p> <p>Introduzca el número de teléfono del usuario</p> </li> 
       <li> <p><b>[!UICONTROL Id. de grupo principal]</b> </p> <p>Introduzca el grupo al que se agrega el nuevo usuario. Si no se escribe nada, el usuario se agregará al grupo predeterminado de la cuenta.</p> </li> 
       <li> <p><b>[!UICONTROL Puesto]</b> </p> <p>Introduzca el cargo del usuario.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Formulario web] ([!UICONTROL widget])</b> </p> <p>Introduzca información en campos específicos basados en el tipo de registro y campos relacionados.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Actualizar registro relacionado]**

Este módulo de acción actualiza los registros relacionados con un objeto específico.

>[!IMPORTANT]
>
>* Como práctica recomendada, si prevé realizar cambios sustanciales en un acuerdo, le recomendamos que cree un nuevo acuerdo en lugar de actualizar el existente.
>* Algunas actualizaciones incluyen campos obligatorios. A medida que configure la actualización, asegúrese de completar todos los campos obligatorios. Los campos obligatorios están en negrita en [!DNL Workfront Fusion] módulos.
>



<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Adobe Acrobat Sign] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p> <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] agrega encabezados de autorización automáticamente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td>Seleccione el tipo de registro del registro al que están asociados los campos relacionados.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Agreement]/[!UICONTROL Library document]/[!UICONTROL User]/[!UICONTROL Widget ID]</td> 
   <td>Introduzca o asigne el ID del objeto con el que desea asociar el registro creado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Otros campos]</td> 
   <td> <p>Introduzca información en campos específicos basados en el tipo de registro y campos relacionados.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Acuerdo]</b> </p> <p>Como práctica recomendada, si prevé realizar cambios sustanciales en un acuerdo, le recomendamos que cree un nuevo acuerdo en lugar de actualizar el existente.</p> </li> 
     <li> <p><b>[!UICONTROL Documento de biblioteca]</b> </p> <p>Seleccione los campos que desea actualizar y rellene los campos seleccionados:</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Estado]</b> </p> <p>Seleccione el nuevo estado del documento de biblioteca.</p> </li> 
       <li> <p><b>[!UICONTROL Nota]</b> </p> <p>Escriba o asigne el texto de la nota.</p> </li> 
       <li> <p><b>[!UICONTROL Visibilidad]</b> </p> <p>Seleccione si el documento de biblioteca se muestra o se guía.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Usuario]</b> </p> <p>Seleccione los campos que desea actualizar y rellene los campos seleccionados:</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Lista de información de grupo]</b> </p> <p>Rellene los campos siguientes</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Estado]</b> </p> <p>Seleccione el nuevo estado del usuario.</p> </li> 
         <li> <p><b>[!UICONTROL ID]</b> </p> <p>Introduzca el ID único del grupo</p> </li> 
         <li> <p><b>[!UICONTROL Es el administrador del grupo]</b> </p> <p>Seleccione <b>[!UICONTROL Yes]</b> para convertir al usuario en administrador de un grupo.</p> </li> 
         <li> <p><b>Es el grupo principal</b> </p> <p>Seleccione <b>[!UICONTROL Yes]</b> para actualizar este grupo al grupo principal del usuario.</p> </li> 
         <li> <p><b>[!UICONTROL Fecha de creación]</b> </p> <p>Introduzca la fecha de creación del grupo.</p> <p>Para obtener una lista de los formatos de fecha y hora admitidos, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">Coerción de tipos en [!UICONTROL Adobe Workfront Fusion]</a>.</p> </li> 
         <li> <p><b>[!UICONTROL Nombre]</b> </p> <p>Introduzca o asigne el nombre del grupo.</p> </li> 
         <li> <p><b>[!UICONTROL Creación de documento de biblioteca visible]</b> </p> <p>Esta configuración determina si el usuario puede crear documentos de biblioteca</p> 
          <ul> 
           <li> <p>[!UICONTROL Valor]</p> <p>Permitir</p> </li> 
           <li> <p>[!UICONTROL Heredado]</p> <p>Heredar la configuración de grupo del grupo o la cuenta</p> </li> 
          </ul> </li> 
         <li> <p><b>[!UICONTROL Enviar restringido a flujos de trabajo]</b> </p> <p>Esta configuración determina si el usuario puede crear acuerdos solo mediante flujos de trabajo.</p> 
          <ul> 
           <li> <p>[!UICONTROL Valor]</p> <p>Permitir</p> </li> 
           <li> <p>[!UICONTROL Heredado]</p> <p>Heredar la configuración de grupo del grupo o la cuenta</p> </li> 
          </ul> </li> 
         <li> <p><b>[!UICONTROL El usuario puede enviar]</b> </p> 
          <ul> 
           <li> <p>[!UICONTROL Valor]</p> <p>Permitir</p> </li> 
           <li> <p>[!UICONTROL Heredado]</p> <p>Heredar la configuración de grupo del grupo o la cuenta</p> </li> 
          </ul> </li> 
        </ul> </li> 
      </ul> 
      <ul> 
       <li> <p><b>[!UICONTROL Estado]</b> </p> <p>Seleccione el nuevo estado del usuario e introduzca un comentario sobre el motivo por el que desea activarlo o desactivarlo.</p> </li> 
       <li> <p><b>[!UICONTROL Configuración regional]</b> </p> <p>Introduzca la configuración regional del usuario. Determina el idioma de la interfaz de usuario. </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Formulario web] ([!UICONTROL widget])</b> </p> <p>Introduzca información en campos específicos basados en el tipo de registro y campos relacionados.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Cargar documento]**

Cargue un documento transitorio. Un documento transitorio está disponible durante 7 días después de cargarse.

>[!NOTE]
>
>Se recomienda cargar el documento para firmarlo como documento transitorio y, a continuación, asignarlo al campo File to send en el módulo Create an agreement.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Adobe Acrobat Sign] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p> <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] agrega encabezados de autorización automáticamente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de registro]</td> 
   <td>Introduzca o asigne el ID del registro que desea actualizar</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL tipo MIME]</td> 
   <td>Introduzca el tipo MIME del archivo original. Los tipos MIME (Extensión multipropósito de correo de Internet) son etiquetas que permiten al software identificar diferentes tipos de datos compartidos en Internet. Los servidores y exploradores web utilizan el tipo MIME para determinar qué se debe hacer con un archivo. Por ejemplo, un archivo con el tipo MIME <code>text/html</code> se procesará en un explorador de forma distinta que un archivo con el tipo MIME <code>image/jpeg</code>.</td> 
  </tr> 
 </tbody> 
</table>

**Ejemplo:** En este flujo de trabajo, el documento que se va a firmar (anteriormente descargado de Workfront) se carga como un documento transitorio.

![](assets/sign-example-1-350x308.png)

El módulo [!UICONTROL Cargar documento] proporciona al documento un ID [!DNL Adobe Acrobat Sign] al que se puede hacer referencia en módulos posteriores. Cuando se crea el acuerdo, el ID del documento cargado se incluye en el campo [!UICONTROL Archivos para enviar].

![](assets/sign-example-2-350x356.png)

+++

### Búsquedas

+++ **[!UICONTROL Buscar acuerdos]**

Este módulo de búsqueda busca los acuerdos basándose en los criterios proporcionados.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Adobe Acrobat Sign] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p> <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro de texto]</td> 
   <td> <p>Busque texto en los metadatos del acuerdo. </p> 
    <ul> 
     <li> <p><b>[!UICONTROL Buscar texto]</b> </p> <p>Escriba el texto que desea buscar en los metadatos del acuerdo. Cada palabra se trata como un elemento de texto independiente. </p> </li> 
     <li> <p><b>[!UICONTROL Buscar texto en]</b> </p> <p>Seleccione los campos de metadatos en los que desea buscar texto. Si no selecciona nada, los módulos buscan todos los metadatos.</p> </li> 
    </ul> <p>El módulo devuelve cualquier acuerdo que contenga cualquiera de los textos introducidos en cualquiera de los campos seleccionados. Ejemplo: introducir "campaña de primavera" y seleccionar las opciones Título y Nota devuelve cualquier acuerdo con las palabras "primavera" o "campaña" en Título o Nota.</p> <p>Para obtener más información sobre la búsqueda de campos en [!DNL Adobe Acrobat Sign], vea "Cómo funciona la búsqueda de texto" en Búsqueda de <a href="https://helpx.adobe.com/sign/using/adobesign-search-users-agreements.html#HowSearchWorks">[!DNL Adobe Sign] - Cómo funciona</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fecha de creación]</td> 
   <td>Seleccionar fechas. El módulo devuelve solo los registros en los que la fecha de creación coincida con este criterio.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fecha de caducidad]</td> 
   <td>Seleccionar fechas. El módulo solo devuelve registros en los que la fecha de caducidad coincida con este criterio.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL Fecha de modificación]</p> </td> 
   <td>Seleccionar fechas. El módulo devuelve solo los registros en los que la fecha de modificación coincida con este criterio.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID externo]</td> 
   <td> <p> El ID externo es un ID asignado por el remitente al acuerdo que puede ser de cualquier forma, pero normalmente en forma de "&lt;groupID&gt;:&lt;ID&gt;".</p> <p>Para cada ID externo que desee agregar, haga clic en <b>[!UICONTROL Agregar]</b> y escriba o asigne el ID externo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de grupo]</td> 
   <td> <p>El ID de grupo es un identificador asignado cuando se creó el grupo.</p> <p>Para cada ID externo que desee agregar, haga clic en <b>[!UICONTROL Agregar]</b> y escriba o asigne el ID externo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de recurso]</td> 
   <td> <p>Este es el ID asignado al acuerdo específico. </p> <p>Para cada ID externo que desee agregar, haga clic en <b>[!UICONTROL Agregar]</b> y escriba o asigne el ID externo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. principal]</td> 
   <td> <p>Este es el ID asignado al objeto principal del acuerdo. </p> <p>Para cada ID externo que desee agregar, haga clic en <b>[!UICONTROL Agregar]</b> y escriba o asigne el ID externo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Correo electrónico del participante]</td> 
   <td> <p>La dirección de correo electrónico de un participante. </p> <p>Para cada ID externo que desee agregar, haga clic en <b>[!UICONTROL Agregar]</b> y escriba o asigne el ID externo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Función]</td> 
   <td>Seleccione las funciones que desea que incluyan los resultados devueltos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordenar por]</td> 
   <td>Si desea que el módulo ordene los resultados, seleccione el campo por el que desea ordenar los resultados.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Orden]r</td> 
   <td>Si desea que el módulo ordene los resultados, seleccione si desea ordenar de forma ascendente o descendente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Estado]</td> 
   <td>Seleccione los estados que desea que incluyan los resultados devueltos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo]</td> 
   <td>Seleccione los tipos de acuerdo que desea que incluyan los resultados devueltos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subtipos]</td> 
   <td>Seleccione los subtipos de acuerdo que desea que incluyan los resultados devueltos. Solo los acuerdos de plantilla de biblioteca incluyen subtipos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de usuario]</td> 
   <td> <p>El ID del usuario con el que se comparte el acuerdo.</p> <p>Para cada ID de usuario que desee agregar, haga clic en <b>[!UICONTROL Agregar]</b> y escriba o asigne el ID de usuario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Visibilidad]</td> 
   <td>Seleccione el nivel de visibilidad que desea que incluyan los resultados devueltos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Índice de inicio]</td> 
   <td> <p>Introduzca la posición del primer resultado que desea devolver. Combine esto con los [!UICONTROL resultados máximos devueltos] para paginar resultados</p> <p>Ejemplo: si devuelve 100 resultados a la vez, introduzca 100 para que se devuelvan los resultados 100-200.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de resultados devueltos]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo [action] ejecute durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++
