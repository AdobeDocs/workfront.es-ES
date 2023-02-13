---
filename: aem-assets-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Módulos de Adobe Experience Manager Assets
description: Con la variable [!DNL Adobe Experience Manager Assets] conector para [!DNL Adobe Workfront Fusion], you can start a scenario based on events in your [!DNL Adobe Experience Manager Assets] cuenta, crear, cargar y actualizar recursos, y copiar o mover carpetas y recursos.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 0749f230-8cab-464f-863c-9cb4870125d1
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1496'
ht-degree: 0%

---

# [!DNL Adobe Experience Manager Assets] módulos

Con la variable [!DNL Adobe Experience Manager Assets] conector para [!DNL Adobe Workfront Fusion], puede iniciar un escenario basado en los eventos del [!DNL Adobe Experience Manager Assets] cuenta, crear, cargar y actualizar recursos, y copiar o mover carpetas y recursos.

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

* Debe tener un [!DNL Adobe Experience Manager Assets] para utilizar estos módulos.
* Debe configurar [!UICONTROL Servidor a servidor] en la variable [!DNL Adobe Developer console].

   Para obtener instrucciones sobre la configuración [!UICONTROL Servidor a servidor] en la variable [!DNL Adobe Developer console], consulte [Generación de tokens de acceso para las API del servidor](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow).

## Connect [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion] {#connect-adobe-experience-manager-assets-to-workfront-fusion}

Para crear una conexión para su [!DNL Adobe Experience Manager Assets] módulos:

1. Haga clic en [!UICONTROL Agregar] junto a la variable [!UICONTROL Conexión] en la ventana

2. Seleccione el tipo de conexión que está creando:

   * **[!DNL AEM Assets as a Cloud Service]**

      Esta configuración requiere información del [!DNL Adobe Admin Console].

   * **[!DNL AEM Assets Basic]**

      Esta configuración requiere un nombre de usuario y una contraseña.

3. Rellene los campos del tipo de conexión que está creando.

   Para [!DNL AEM Assets as a Cloud Service], consulte [Configurar la conexión para [!DNL AEM Assets as a Cloud Service]](#configure-the-connection-for-aem-assets-as-a-cloud-service).

   Para [!UICONTROL AEM Assets Basic], consulte [Configurar la conexión para [!UICONTROL AEM Assets Basic]](#configure-the-connection-for-aem-assets-basic).

4. Haga clic en **[!UICONTROL Continuar]** para guardar la conexión y volver al módulo.


### Configurar la conexión para [!DNL AEM Assets as a Cloud Service]

>[!NOTE]
>
>La información de estos campos se genera como parte de la configuración [!UICONTROL Servidor a servidor] flujo en la variable [!DNL Adobe Developer Console]. Puede encontrar estos valores en el archivo JSON de credenciales de servicio generado como parte de esa configuración.
>
>Para obtener instrucciones sobre la configuración [!UICONTROL Servidor a servidor] flujo en la variable [!UICONTROL Consola de Adobe Developer], consulte [Generación de tokens de acceso para las API del servidor](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow).


<table style="table-layout:auto"> 
          <col/>
          <col/>
          <tbody>
              <tr>
                  <td role="rowheader">[!UICONTROL Connection name]</td>
                  <td>
                      <p>Escriba un nombre para esta conexión</p>
                  </td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL URL de instancia sin barra diagonal]</td>
                  <td>Introduzca la dirección URL de su [!DNL Adobe Experience Manager] instancia. No incluir una barra oblicua <code>/</code> al final de la dirección URL.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Client ID]</td>
                  <td>Introduzca el ID de cliente generado en la configuración de [!UICONTROL Server-to-server].</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Client Secret]</td>
                  <td>Introduzca el Secreto del cliente generado en la configuración de [!UICONTROL Server-to-server].</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL ID de cuenta técnica]</td>
                  <td>Introduzca el ID de la cuenta técnica. Este es el campo "[!UICONTROL id]" en el archivo JSON de credenciales de cliente.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Org ID]</td>
                  <td class="">Introduzca el ID de su organización. Este es el campo "[!UICONTROL org]" en el archivo JSON de credenciales de cliente.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Meta-Scopes]</td>
                  <td>Introduzca los metaámbitos generados en la configuración de [!UICONTROL Server-to-server].</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Clave privada]</td>
                  <td>Introduzca la Clave privada generada para obtener la configuración [!UICONTROL Server-to-server]. Para extraer la clave privada, haga clic en [!UICONTROL Extract] y, a continuación, introduzca el archivo que desea extraer y la contraseña del archivo.</td>
              </tr>
          </tbody>
      </table>


### Configurar la conexión para [!DNL AEM Assets Basic]

<table style="table-layout:auto"> 
        <col/>
        <col />
        <tbody>
            <tr>
                <td role="rowheader">[!UICONTROL Connection name]</td>
                <td>
                    <p>Escriba un nombre para esta conexión</p>
                </td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL URL de instancia sin barra diagonal]</td>
                <td>Introduzca la dirección URL de su [!DNL Adobe Experience Manager] instancia. No incluir una barra oblicua <code>/</code> al final de la dirección URL.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Username]</td>
                <td>Introduzca el nombre de usuario de la variable [!DNL AEM Assets] cuenta que utiliza esta conexión.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Contraseña]</td>
                <td>Escriba la contraseña para la variable [!DNL AEM Assets] cuenta que utiliza esta conexión.</td>
            </tr>
        </tbody>
    </table>


## [!DNL Adobe Experience Manager Assets] módulos y sus campos

Al configurar [!DNL Adobe Experience Manager Essentials] módulos, [!DNL Workfront Fusion] muestra los campos que se enumeran a continuación. Además de estos, se incluyen [!DNL Adobe Experience Manager Essentials] pueden mostrarse los campos, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón de asignación encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### [!UICONTROL Copiar una carpeta o un recurso]

Este módulo de acción copia una carpeta o un recurso en otra ubicación de la cuenta de Adobe Experience Manager Assets.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Adobe Experience Manager Assets] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione si desea copiar una carpeta o un recurso.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder] / [!UICONTROL Asset selection]</td> 
   <td>Seleccione o asigne la carpeta o el recurso que desea copiar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ruta de destino]</td> 
   <td>Seleccione o asigne la ruta a la ubicación de la nueva carpeta o recurso.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre de la carpeta copiada] / [!UICONTROL asset]</td> 
   <td>Introduzca un nombre para la nueva carpeta o recurso. El nombre de la carpeta que se muestra en [!DNL Adobe Experience Manager Assets] es el mismo que el nombre original. El nombre introducido aquí aparece en la dirección URL de la nueva carpeta o recurso.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copiar elementos secundarios]</td> 
   <td>Active esta opción para copiar subcarpetas o recursos dentro de la carpeta.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sobrescribir]</td> 
   <td>Active esta opción para sobrescribir cualquier carpeta o recurso de la ubicación de destino que tenga el mismo nombre que la carpeta o el recurso que se está copiando.</td> 
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
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Adobe Experience Manager Assets] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de objeto]</td> 
   <td> <p>Seleccione si desea crear una carpeta o un comentario en un recurso.</p> 
    <ul> 
     <li> <p>[!UICONTROL Folder]</p> <p>Complete los campos siguientes:</p> 
      <ul> 
       <li> <p>[!UICONTROL Name]</p> <p>Escriba un nombre para la carpeta. Este nombre aparecerá en la ruta del archivo, por lo que no debe incluir espacios ni otros caracteres. </p> </li> 
       <li> <p>[!UICONTROL Title]</p> <p>Introduzca un título para la carpeta, que se puede mostrar en lugar del nombre.</p> </li> 
      </ul> </li> 
     <li> <p>[!UICONTROL Asset comment]</p> <p>Complete los campos siguientes:</p> 
      <ul> 
       <li> <p>[!UICONTROL Selección de recursos]</p> <p>Seleccione o asigne el ID del recurso al que desee agregar un comentario.</p> </li> 
       <li> <p>[!UICONTROL Comentario]</p> <p>Introduzca el texto del comentario.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Eliminar un registro]

Este módulo de acción elimina una carpeta, un recurso o una representación.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Adobe Experience Manager Assets] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione si desea eliminar una carpeta, un recurso o una representación.</p> 
    <ul> 
     <li> <p>[!UICONTROL Folder]</p> <p>Seleccione la carpeta que desea eliminar seleccionando las carpetas de su ruta.</p> </li> 
     <li> <p>[!UICONTROL Asset] </p> <p>Seleccione el recurso seleccionando las carpetas en su ruta y el recurso que desea eliminar.</p> </li> 
     <li> <p>[!UICONTROL Representación]</p> <p>Seleccione la representación seleccionando las carpetas en su ruta.</p> <p>Introduzca o asigne el nombre de la representación.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Obtener una lista de carpetas]

Este módulo de acción recupera una representación de una carpeta existente y de sus entidades secundarias (carpetas o recursos).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Adobe Experience Manager Assets] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>Seleccione o asigne la carpeta que desee recuperar. Para añadir subcarpetas a la ruta, haga clic en el icono del signo más y seleccione la subcarpeta .</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Realizar una llamada API personalizada]

Este módulo de acción realiza una llamada API personalizada a la variable [!DNL Adobe Experience Manager Assets] API.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Adobe Experience Manager Assets] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Introduzca una ruta relativa a su [!DNL Adobe Experience Manager] URL base.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Método]</p> </td> 
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada a la API. Para obtener más información, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p> <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] añade encabezados de autorización automáticamente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadena de consulta] </td> 
   <td> <p>Introduzca la cadena de consulta de solicitud. Para cada par clave/valor, haga clic en <b>[!UICONTROL Agregar elemento]</b> e introduzca [!UICONTROL Key] y [!UICONTROL Value].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Al utilizar afirmaciones condicionales como <code>if</code> en su JSON, ponga las comillas fuera de la afirmación condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Mover una carpeta o un recurso]

Este módulo de acción mueve el recurso o la carpeta de la ruta dada a una nueva ubicación.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Adobe Experience Manager Assets] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione si desea mover una carpeta o un recurso.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder] / [!UICONTROL Asset]</td> 
   <td>Seleccione o asigne la carpeta o el recurso que desee mover.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ruta de destino]</td> 
   <td>Seleccione o asigne la ruta a la ubicación a la que desea mover la carpeta o el recurso.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre de la carpeta movida] / [!UICONTROL asset]</td> 
   <td>Introduzca un nuevo nombre para la carpeta o el recurso que se ha movido. El nombre de la carpeta que se muestra en [!DNL Adobe Experience Manager Assets] es el mismo que el nombre original. El nombre introducido aquí aparece en la dirección URL de la carpeta o el recurso movidos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sobrescribir]</td> 
   <td>Active esta opción para sobrescribir cualquier carpeta o recurso de la ubicación de destino que tenga el mismo nombre que la carpeta o el recurso que se está copiando.</td> 
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
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Adobe Experience Manager Assets] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione si desea eliminar metadatos de recursos o una representación de recursos.</p> 
    <ul> 
     <li> <p>[!UICONTROL Metadatos de recursos]</p> 
      <ul> 
       <li> <p>Seleccione el recurso para el que desea actualizar los metadatos.</p> </li> 
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

Este módulo de acción carga un recurso en su [!DNL Adobe Experience Manager Assets] cuenta.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Adobe Experience Manager Assets] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destino]</td> 
   <td> <p>Seleccione la carpeta en la que desea cargar un recurso.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td>Introduzca o asigne el nombre y los datos del archivo de origen.</td> 
  </tr> 
 </tbody> 
</table>
