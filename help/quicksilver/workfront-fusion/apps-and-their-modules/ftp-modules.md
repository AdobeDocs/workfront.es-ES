---
filename: ftp-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Módulos FTP
description: Los módulos FTP permiten supervisar los cambios de archivos en una carpeta seleccionada, cargar nuevos archivos en la carpeta deseada y modificar o eliminar archivos existentes que ya se encuentran en una carpeta.
author: Becky
exl-id: 360825a4-4580-4039-894e-583e82132ed6
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1295'
ht-degree: 0%

---

# Módulos FTP

Los módulos FTP permiten supervisar los cambios de archivos en una carpeta seleccionada, cargar nuevos archivos en la carpeta deseada y modificar o eliminar archivos existentes que ya se encuentran en una carpeta.

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

Para usar [Aplicación de fusión] con [!DNL Workfront Fusion], debe tener una cuenta de FTP.

## Creación de una conexión en un módulo FTP {#create-a-connection}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection name]</td> 
   <td> <p> Escriba el nombre de la conexión FTP.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Host] </td> 
   <td> <p>Introduzca el nombre de host del servidor FTP. E.g. <code>myftp123.server.com</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Port] </td> 
   <td> <p>Introduzca el número de puerto del servidor FTP. E.g. <code>21</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User name] </td> 
   <td> <p>Escriba el nombre de usuario de su cuenta de FTP.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Contraseña] </td> 
   <td> <p>Introduzca la contraseña de su cuenta de FTP.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Usar una conexión segura (TLS)</p> </td> 
   <td> <p>Seleccione si desea utilizar una conexión segura.</p> <p style="font-weight: bold;">[!UICONTROL No]</p> <p>La conexión no está segura.</p> <p style="font-weight: bold;">[!UICONTROL Cifrado explícito o cifrado implícito]</p> <p>La conexión está segura mediante SSL.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Rechazar certificados no autorizados]</p> </td> 
   <td> <p>Active esta opción para verificar el certificado del servidor FTP. Si la verificación falla, no se creará la conexión. Para pasar la verificación, el certificado debe cumplir uno de los siguientes criterios:</p> 
    <ul> 
     <li>estar firmado por una raíz <a href="https://en.wikipedia.org/wiki/Certificate_authority">Autoridad de certificados</a></li> 
     <li>estar firmada por una autoridad de certificación intermedia (véase, por ejemplo, <a href="https://knowledge.digicert.com/solution/SO16297.html">Funcionamiento de las cadenas de certificados</a> para obtener más información). En este caso, todos los certificados intermedios deben instalarse en el servidor FTP.</li> 
     <li>ser un certificado autofirmado suministrado en el campo [!UICONTROL Certificado autofirmado] (consulte a continuación)</li> </ul>

Si esta opción está desactivada, el certificado de servidor FTP no se verifica. Recomendamos encarecidamente que no se deshabilite la opción, ya que hace que la conexión sea insegura y plantea un grave riesgo para la seguridad.</td>
</tr> 
  <tr> 
   <td> <p>[!UICONTROL Certificado autofirmado]</p> </td> 
   <td> <p>Haga clic en el <b>[!UICONTROL Extract]</b> para abrir el cuadro de diálogo de carga.</p> <p>Cargue el certificado para utilizar el TLS con su certificado autofirmado. [!DNL Workfront Fusion] no conserva ni almacena ningún dato proporcionado, como archivos y contraseñas. El archivo y la contraseña solo se utilizan para extraer el certificado.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Módulos FTP y sus campos

* [Déclencheur](#triggers)
* [Acciones](#actions)

### Déclencheur

#### [!UICONTROL Archivos de Watch]

[!UICONTROL Archivos de Watch] es el único módulo de déclencheur para FTP. Supervisa el contenido del archivo de la carpeta seleccionada. El déclencheur se ejecuta cuando se inserta un nuevo archivo en la carpeta especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo establecer una conexión con la cuenta de FTP, consulte <a href="#create-a-connection" class="MCXref xref">[!UICONTROL Crear una conexión] en un módulo FTP</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Folder]</p> </td> 
   <td> <p>Seleccione la carpeta que desee ver.</p> <p><b>Nota:</b> Solo se permite una carpeta por escenario. Las subcarpetas se ignoran.</p> <p><b>Sugerencia:</b> Para realizar un seguimiento de varias carpetas, cree un escenario independiente para cada una de ellas.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de archivos devueltos] </td> 
   <td> <p>Establezca el número máximo de resultados que [!DNL Workfront Fusion] funcionará con durante un ciclo. Si el valor se establece demasiado alto, la conexión se puede interrumpir en el lado del servicio de terceros dado (tiempo de espera). [!DNL Workfront Fusion] no tiene influencia en esto. Se recomienda establecer un valor inferior y definir un valor mayor para el número máximo de ciclos o ejecutar el escenario con más frecuencia.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Acciones

* [[!UICONTROL Cambiar permisos]](#change-permissions)
* [[!UICONTROL Crear una carpeta]](#create-a-folder)
* [[!UICONTROL Eliminar un archivo]](#delete-a-file)
* [[!UICONTROL Eliminar una carpeta]](#delete-a-folder)
* [[!UICONTROL Obtener un archivo]](#get-a-file)
* [[!UICONTROL Lista de archivos de una carpeta]](#list-of-files-in-a-folder)
* [[!UICONTROL Mover un archivo o carpeta]](#move-a-file-or-folder)
* [[!UICONTROL Cargar] un archivo](#upload-a-file)

#### [!UICONTROL Cambiar permisos]

Este módulo de acción cambia la configuración de permisos de un archivo o carpeta.

<table style="width: 100%;" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" />
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2" />
   <tbody>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">[!UICONTROL Connection]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Para obtener instrucciones sobre cómo establecer una conexión con la cuenta de FTP, consulte <a href="#Create" class="MCXref xref" >[!UICONTROL Crear una conexión] en un módulo FTP</a> en este artículo.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">[!UICONTROL Cambiar la configuración de permisos de]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">
               <p>Seleccione si desea cambiar la configuración de un archivo o carpeta.</p>
            </td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">[!UICONTROL Ruta del archivo]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Introduzca o asigne la ruta del archivo a la carpeta o al archivo.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Permisos]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
               <p>Establezca los permisos de archivo o carpeta que desee. Utilice los parámetros chmod. Por ejemplo: <code>777 </code>o <code>-rwxrwxrwx</code>.</p>
               <p>Los permisos deben coincidir con el patrón <code> /(.?([r-][w-][x-]){3})|[0-7]{3,4}/</code>.</p>
            </td>
         </tr>
   </tbody>
</table>

#### [!UICONTROL Crear una carpeta]

Este módulo de acción crea una nueva carpeta.

<table style="width: 100%;" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" />
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2" />
   <tbody>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">[!UICONTROL Connection]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Para obtener instrucciones sobre cómo establecer una conexión con la cuenta de FTP, consulte <a href="#Create" class="MCXref xref" >[!UICONTROL Crear una conexión] en un módulo FTP</a> en este artículo.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">[!UICONTROL Folder path]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Introduzca o asigne la ruta del archivo a la nueva carpeta.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">[!UICONTROL Nuevo nombre de carpeta]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">
               <p>Introduzca o asigne un nombre para la nueva carpeta.</p>
            </td>
         </tr>
   </tbody>
</table>

#### [!UICONTROL Eliminar un archivo]

Elimina un archivo de la carpeta especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Para obtener instrucciones sobre cómo establecer una conexión con la cuenta de FTP, consulte <a href="#Create" class="MCXref xref" >[!UICONTROL Crear una conexión] en un módulo FTP</a> en este artículo.</td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Seleccione la carpeta FTP desde la que desea eliminar un archivo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File name]</td> 
   <td> <p> Introduzca el nombre de archivo, incluida la extensión de nombre de archivo. Ejemplo: <code>[!DNL image].png</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar una carpeta]

Este módulo de acción elimina permanentemente la carpeta especificada.

<table style="width: 100%;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15">
   <col style="width: 301px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <tbody>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">[!UICONTROL Connection]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Para obtener instrucciones sobre cómo establecer una conexión con la cuenta de FTP, consulte <a href="#Create" class="MCXref xref" >[!UICONTROL Crear una conexión] en un módulo FTP</a> en este artículo.</td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="font-weight: bold;">[!UICONTROL Folder]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray">
               <p>Seleccione la carpeta FTP desde la que desea eliminar un archivo.</p>
            </td>
         </tr>
   </tbody>
</table>

#### [!UICONTROL Obtener un archivo]

Recupera un archivo del servidor FTP que se puede seguir procesando, por ejemplo, cargado en la variable [!DNL Dropbox].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo establecer una conexión con la cuenta de FTP, consulte <a href="#creating-the-ftp-connection" class="MCXref xref">Creación de la conexión FTP</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ruta del archivo]</td> 
   <td> <p> Introduzca la ruta del archivo que desea obtener.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Lista de archivos de una carpeta]

Recupera información de archivos o carpetas.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo establecer una conexión con la cuenta de FTP, consulte <a href="#creating-the-ftp-connection" class="MCXref xref">Creación de la conexión FTP</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Seleccione la carpeta FTP en la que desee buscar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Show] </td> 
   <td> <p>Seleccione si desea recuperar información sobre archivos, carpetas o ambos.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Buscar] </td> 
   <td> <p>Introduzca el término de búsqueda. Si no se introduce ningún término de búsqueda, se recuperarán todos los archivos y carpetas de la carpeta especificada.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de archivos devueltos]</td> 
   <td> <p> Establezca el número máximo de archivos recuperados por este módulo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mover un archivo o carpeta]

Este módulo de acción mueve un archivo o carpeta a una ubicación diferente.

<table style="width: 100%;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15">
   <col style="width: 301px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <tbody>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">[!UICONTROL Connection]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Para obtener instrucciones sobre cómo establecer una conexión con la cuenta de FTP, consulte <a href="#Create" class="MCXref xref" >[!UICONTROL Crear una conexión] en un módulo FTP</a> en este artículo.</td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">[!UICONTROL Ruta de archivo antigua]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">
               <p>Introduzca la ruta de acceso desde la que desea mover el archivo. Ejemplo: <code>/folder1/document.txt</code>.</p>
            </td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray" style="font-weight: bold;">[!UICONTROL Nueva ruta de archivo]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray">
               <p>Introduzca la ruta a la que desea mover el archivo. Ejemplo: <code>/folder2/document.txt</code>.</p>
            </td>
         </tr>
   </tbody>
</table>


#### [!UICONTROL Cargar un archivo]

Carga un archivo en el servidor FTP.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td>Para obtener instrucciones sobre cómo establecer una conexión con la cuenta de FTP, consulte <a href="#creating-the-ftp-connection" class="MCXref xref">Creación de la conexión FTP</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Seleccione la carpeta FTP a la que desee cargar el archivo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Archivo de origen] </td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Anexar a un archivo existente]</td> 
   <td> <p>Si esta opción está habilitada y el archivo ya existe en el servidor FTP, el contenido del archivo se añade al archivo existente. Si esta opción no está activada, se sobrescribirá el contenido del archivo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Crear carpetas si no existen] </td> 
   <td> <p>Si esta opción está habilitada y la carpeta que ha introducido en el campo Folder no existe en el servidor FTP, el módulo crea la carpeta</p> </td> 
  </tr> 
 </tbody> 
</table>

## Resolución de problemas {#troubleshooting}

Si tiene problemas con la aplicación FTP durante la creación de la conexión o durante la operación de un módulo, intente utilizar uno de los clientes FTP más populares e intente realizar la misma acción (por ejemplo, crear una conexión o mostrar archivos en una carpeta). con el cliente FTP. Si tiene los mismos problemas con el cliente FTP, es posible que se deba a una configuración incorrecta del servidor FTP.
