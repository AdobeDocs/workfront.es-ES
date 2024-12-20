---
filename: aem-assets-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de Adobe Experience Manager Assets
description: Con el conector  [!DNL Adobe Experience Manager Assets] para la cuenta de { [!DNL Adobe Workfront Fusion], you can start a scenario based on events in your [!DNL Adobe Experience Manager Assets] }, cree, cargue y actualice recursos, y copie o mueva carpetas y recursos.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 0749f230-8cab-464f-863c-9cb4870125d1
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1724'
ht-degree: 0%

---

# [!DNL Adobe Experience Manager Assets] módulos

Con el conector [!DNL Adobe Experience Manager Assets] de [!DNL Adobe Workfront Fusion], puede iniciar un escenario basado en los eventos de su cuenta de [!DNL Adobe Experience Manager Assets], crear, cargar y actualizar recursos, y copiar o mover carpetas y recursos.

Para ver una introducción al conector de Adobe Experience Manager Assets, consulte:

* [Adobe Experience Manager Assets](https://video.tv.adobe.com/v/3427034/){target=_blank}

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

* Debe tener una cuenta de [!DNL Adobe Experience Manager Assets] para utilizar estos módulos.
* Debe configurar el flujo de [!UICONTROL servidor a servidor] en [!DNL Adobe Developer console].

  Para obtener instrucciones sobre la configuración del flujo de [!UICONTROL servidor a servidor] en [!DNL Adobe Developer console], consulte [Generación de tokens de acceso para las API del servidor](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow).
* La cuenta técnica de Adobe Experience Manager debe tener permisos de escritura.

  Para obtener instrucciones sobre cómo agregar permisos de escritura a su cuenta técnica de Adobe Experience Manager, consulte [Credenciales de servicio](https://experienceleague.adobe.com/en/docs/experience-manager-learn/getting-started-with-aem-headless/authentication/service-credentials) en la documentación de Adobe Experience Manager.

## Información de API de Adobe Experience Manager Assets

El conector de Adobe Experience Manager Assets utiliza lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Etiqueta de API</td> 
   <td>Versión 1.8.61</td> 
  </tr>
 </tbody> 
 </table>

## Conectar [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion] {#connect-adobe-experience-manager-assets-to-workfront-fusion}

Para crear una conexión para los módulos de [!DNL Adobe Experience Manager Assets]:

1. Haga clic en [!UICONTROL Agregar] junto al cuadro [!UICONTROL Conexión].

2. Seleccione el tipo de conexión que está creando:

   * **[!DNL AEM Assets as a Cloud Service]**

     Esta configuración requiere información de [!DNL Adobe Admin Console].

   * **[!DNL AEM Assets Basic]([!DNL Adobe Managed Services])**

     Esta configuración requiere un nombre de usuario y una contraseña.

3. Rellene los campos del tipo de conexión que está creando.

   Para [!DNL AEM Assets as a Cloud Service], consulte [Configurar la conexión para [!DNL AEM Assets as a Cloud Service]](#configure-the-connection-for-aem-assets-as-a-cloud-service).

   Para [!UICONTROL AEM Assets básicos] ([!DNL Adobe Managed Services]), consulte [Configuración de la conexión para [!UICONTROL AEM Assets básicos]](#configure-the-connection-for-aem-assets-basic).

4. Haga clic en **[!UICONTROL Continuar]** para guardar la conexión y volver al módulo.


### Configurar la conexión de [!DNL AEM Assets as a Cloud Service]

>[!NOTE]
>
>* La información de estos campos se genera como parte del flujo de configuración de [!UICONTROL servidor a servidor] en [!DNL Adobe Developer Console]. Puede encontrar estos valores en el archivo JSON de credenciales de servicio generado como parte de esa configuración.
>
>   Para obtener instrucciones sobre cómo configurar el flujo de [!UICONTROL servidor a servidor] en [!UICONTROL Adobe Developer Console], consulte [Generación de tokens de acceso para las API del servidor](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow).
>
>* La cuenta técnica de Adobe Experience Manager debe tener permisos de escritura.
>
>   Para obtener instrucciones sobre cómo agregar permisos de escritura a su cuenta técnica de Adobe Experience Manager, consulte [Credenciales de servicio](https://experienceleague.adobe.com/en/docs/experience-manager-learn/getting-started-with-aem-headless/authentication/service-credentials) en la documentación de Adobe Experience Manager.


<table style="table-layout:auto"> 
          <col/>
          <col/>
          <tbody>
              <tr>
                  <td role="rowheader">[!UICONTROL Nombre de conexión]</td>
                  <td>
                      <p>Escriba un nombre para esta conexión</p>
                  </td>
              </tr>
              <tr>
                  <td role="rowheader">URL de instancia de [!UICONTROL sin barra diagonal]</td>
                  <td>Escriba la dirección URL de la instancia [!DNL Adobe Experience Manager]. No incluya una barra diagonal <code>/</code> al final de la dirección URL.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Detalles de cuenta, opciones de relleno]</td>
                  <td>Seleccione si desea proporcionar un archivo JSON que describa los detalles de su cuenta o si desea introducir los detalles manualmente.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Detalles técnicos de la cuenta en formato JSON]</td>
                  <td>Si proporciona JSON, introduzca o pegue el JSON que describe los detalles de la cuenta.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL ID de cliente]</td>
                  <td>Si introduce los detalles manualmente, introduzca el ID de cliente generado en la configuración de [!UICONTROL Servidor a servidor].</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Secreto de cliente]</td>
                  <td>Si introduce los detalles manualmente, introduzca el Secreto de cliente generado en la configuración de [!UICONTROL Servidor a servidor].</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL ID de cuenta técnica]</td>
                  <td>Si introduce los detalles manualmente, introduzca el ID de la cuenta técnica. Este es el campo "[!UICONTROL id]" en el archivo JSON de credenciales del cliente.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Org ID]</td>
                  <td class="">Si introduce los detalles manualmente, introduzca el ID de su organización. Este es el campo "[!UICONTROL org]" en el archivo JSON de credenciales del cliente.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL MetaÁmbitos]</td>
                  <td>Introduzca los metaámbitos generados en la configuración de [!UICONTROL Servidor a servidor].</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Clave privada]</td>
                  <td>Introduzca la clave privada generada durante la instalación de [!UICONTROL Servidor a servidor]. Para extraer la clave privada, haga clic en [!UICONTROL Extraer] y, a continuación, introduzca el archivo que desea extraer y la contraseña del archivo.</td>
              </tr>
          </tbody>
      </table>


### Configurar la conexión de [!DNL AEM Assets Basic] ([!DNL Adobe Managed Services])

<table style="table-layout:auto"> 
        <col/>
        <col />
        <tbody>
            <tr>
                <td role="rowheader">[!UICONTROL Nombre de conexión]</td>
                <td>
                    <p>Escriba un nombre para esta conexión</p>
                </td>
            </tr>
            <tr>
                <td role="rowheader">URL de instancia de [!UICONTROL sin barra diagonal]</td>
                <td>Escriba la dirección URL de la instancia [!DNL Adobe Experience Manager]. No incluya una barra diagonal <code>/</code> al final de la dirección URL.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Nombre de usuario]</td>
                <td>Escriba el nombre de usuario de la cuenta [!DNL AEM Assets] que utiliza esta conexión.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Contraseña]</td>
                <td>Escriba la contraseña de la cuenta de [!DNL AEM Assets] que utiliza esta conexión.</td>
            </tr>
        </tbody>
    </table>


## [!DNL Adobe Experience Manager Assets] módulos y sus campos

Al configurar [!DNL Adobe Experience Manager Essentials] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL Adobe Experience Manager Essentials] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, vea [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Copiar una carpeta o un recurso](#copy-a-folder-or-asset)
* [Creación de un registro](#create-a-record)
* [Eliminar una carpeta, un recurso o una representación](#delete-a-folder-asset-or-rendition)
* [Obtener una lista de carpetas](#get-a-folder-listing)
* [Realizar una llamada de API personalizada](#make-a-custom-api-call)
* [Mover una carpeta o un recurso](#move-a-folder-or-asset)
* [Actualización de un registro](#update-a-record)
* [Cargar un recurso](#upload-an-asset)

### [!UICONTROL Copiar una carpeta o un recurso]

Este módulo de acción copia una carpeta o un recurso en otra ubicación de su cuenta de Adobe Experience Manager Assets.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion], vea <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione si desea copiar una carpeta o un recurso.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Carpeta] / [!UICONTROL Selección de recursos]</td> 
   <td>Seleccione o asigne la carpeta o el recurso que desee copiar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ruta de destino]</td> 
   <td>Seleccione o asigne la ruta a la ubicación de la nueva carpeta o recurso.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre de la carpeta copiada] / [!UICONTROL recurso]</td> 
   <td>Introduzca un nombre para la nueva carpeta o recurso. El nombre de carpeta que se muestra en [!DNL Adobe Experience Manager Assets] es el mismo que el nombre original. El nombre introducido aquí aparece en la dirección URL de la nueva carpeta o recurso.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copiar elementos secundarios]</td> 
   <td>Active esta opción para copiar subcarpetas o recursos dentro de la carpeta.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sobrescribir]</td> 
   <td>Active esta opción para sobrescribir cualquier carpeta o recurso en la ubicación de destino que tenga el mismo nombre que la carpeta o el recurso que se está copiando.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Crear un registro]

Este módulo de acción crea una carpeta o un comentario de recurso.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion], vea <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de objeto]</td> 
   <td> <p>Seleccione si desea crear una carpeta o un comentario en un recurso.</p> 
    <ul> 
     <li> <p>[!UICONTROL Carpeta]</p> <p>Rellene los campos siguientes:</p> 
      <ul> 
       <li> <p>[!UICONTROL Nombre]</p> <p>Introduzca un nombre para la carpeta. Este nombre aparecerá en la ruta de archivo, por lo que no debe incluir espacios ni otros caracteres. </p> </li> 
       <li> <p>[!UICONTROL Título]</p> <p>Introduzca un título para la carpeta, que se puede mostrar en lugar del nombre.</p> </li> 
      </ul> </li> 
     <li> <p>[!UICONTROL Comentario de recurso]</p> <p>Rellene los campos siguientes:</p> 
      <ul> 
       <li> <p>[!UICONTROL Selección de recursos]</p> <p>Seleccione o asigne el ID del recurso al que desea agregar un comentario.</p> </li> 
       <li> <p>[!UICONTROL Comentario]</p> <p>Introduzca el texto del comentario.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Eliminar una carpeta, recurso o representación]

Este módulo de acción elimina una carpeta, un recurso o una representación.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion], vea <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione si desea eliminar una carpeta, un recurso o una representación.</p> 
    <ul> 
     <li> <p>[!UICONTROL Carpeta]</p> <p>Seleccione la carpeta que desea eliminar seleccionando las carpetas en su ruta.</p> </li> 
     <li> <p>[!UICONTROL Recurso] </p> <p>Seleccione el recurso seleccionando las carpetas de su ruta y, a continuación, el recurso que desee eliminar.</p> </li> 
     <li> <p>[!UICONTROL Rendition]</p> <p>Seleccione la representación seleccionando las carpetas en su ruta.</p> <p>Introduzca o asigne el nombre de la representación.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Obtener un listado de carpetas]

Este módulo de acción recupera una representación de una carpeta existente y de sus entidades secundarias (carpetas o recursos).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion], vea <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Carpeta]</td> 
   <td>Seleccione o asigne la carpeta que desea recuperar. Para agregar subcarpetas a la ruta, haga clic en el icono de signo más y seleccione la subcarpeta.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Realizar una llamada de API personalizada]

Este módulo de acción realiza una llamada de API personalizada a la API [!DNL Adobe Experience Manager Assets].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion], vea <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Escriba una ruta relativa a la dirección URL base [!DNL Adobe Experience Manager].</p> </td> 
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
   <td> <p>Introduzca la cadena de consulta de solicitud. Para cada par clave/valor, haga clic en <b>[!UICONTROL Agregar elemento]</b> e introduzca la [!UICONTROL Clave] y el [!UICONTROL Valor].</p> </td> 
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

### [!UICONTROL Mover una carpeta o un recurso]

Este módulo de acción mueve el recurso o la carpeta en la ruta dada a una nueva ubicación.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion], vea <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione si desea mover una carpeta o un recurso.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Carpeta] / [!UICONTROL Recurso]</td> 
   <td>Seleccione o asigne la carpeta o el recurso que desee mover.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ruta de destino]</td> 
   <td>Seleccione o asigne la ruta a la ubicación a la que desee mover la carpeta o el recurso.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre de la carpeta desplazada] / [!UICONTROL recurso]</td> 
   <td>Introduzca un nombre nuevo para la carpeta o el recurso movido. El nombre de carpeta que se muestra en [!DNL Adobe Experience Manager Assets] es el mismo que el nombre original. El nombre introducido aquí aparece en la dirección URL de la carpeta o el recurso movido.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sobrescribir]</td> 
   <td>Active esta opción para sobrescribir cualquier carpeta o recurso en la ubicación de destino que tenga el mismo nombre que la carpeta o el recurso que se está copiando.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Actualizar un registro]

Este módulo de acción actualiza un registro existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion], vea <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione si desea eliminar los metadatos del recurso o una representación del recurso.</p> 
    <ul> 
     <li> <p>[!UICONTROL Metadatos de recursos]</p> 
      <ul> 
       <li> <p>Seleccione el recurso cuyos metadatos desea actualizar.</p> </li> 
       <li> <p>Introduzca el nuevo título del recurso.</p> </li> 
      </ul> </li> 
     <li> <p>[!UICONTROL Representación de recursos]</p> 
      <ul> 
       <li> <p>Seleccione el recurso para el que desea actualizar la representación.</p> </li> 
       <li> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Cargar un recurso]

Este módulo de acción carga un recurso en su cuenta de [!DNL Adobe Experience Manager Assets].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion], vea <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destino]</td> 
   <td> <p>Seleccione la carpeta en la que desea cargar un recurso.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL archivo Source]</td> 
   <td>Introduzca o asigne el nombre y los datos del archivo de origen.</td> 
  </tr> 
 </tbody> 
</table>
