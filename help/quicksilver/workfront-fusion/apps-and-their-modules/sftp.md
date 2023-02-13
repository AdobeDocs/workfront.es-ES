---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Módulos SFTP
description: La variable [!DNL Adobe Workfront Fusion SFTP] Los módulos permiten controlar los cambios de archivo en una carpeta o subcarpeta seleccionada, cargar nuevos archivos a la carpeta deseada, modificar o eliminar archivos existentes que ya se encuentran en una carpeta o cambiar los permisos de archivo.
author: Becky
feature: Workfront Fusion
exl-id: aacc61f8-ffc3-48db-9f54-188685c52067
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '1883'
ht-degree: 0%

---

# Módulos SFTP

La variable [!DNL Adobe Workfront Fusion] SFLos módulos TP permiten controlar los cambios de archivos en una carpeta o subcarpeta seleccionada, cargar nuevos archivos a la carpeta deseada, modificar o eliminar archivos existentes que ya se encuentran en una carpeta o cambiar los permisos de archivos.

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

Para utilizar SFTP con [!DNL Workfront Fusion], es necesario tener una cuenta SFTP (como [!DNL GoDaddy] alojamiento web).

## Conectar SFTP a [!DNL Workfront Fusion] {#connect-sftp-to-workfront-fusion}

Para conectar su cuenta SFTP a [!DNL Workfront Fusion] debe introducir el host de destino y las credenciales de SFTP (nombre de usuario y contraseña, nombre de usuario y clave) en el [!UICONTROL Crear una conexión] diálogo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection name]</td> 
   <td> <p> Escriba el nombre de la conexión SFTP.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Host]</p> </td> 
   <td> <p>Introduzca el nombre de host del servidor SFTP que desea conectar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Port] </td> 
   <td> <p>Introduzca el puerto del servidor SFTP. Por ejemplo, 22.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo autenticación]</p> </td> 
   <td> <p>Seleccione el método de autorización que desea utilizar para conectarse al servidor SFTP.</p> 
    <ul> 
     <li><strong>[!UICONTROL Nombre de usuario y contraseña]</strong>: Introduzca sus credenciales.</li> 
     <li> <p><strong>[!UICONTROL Nombre de usuario y clave]</strong>: Introduzca su nombre de usuario y la clave privada o el certificado</p> <p>Cargue la clave privada para utilizar la autorización del lado del cliente o cargue el certificado (archivo P12 o PFX) si desea utilizar TLS con su certificado autofirmado. Si utiliza la autorización de certificados del lado del cliente, puede introducir aquí el certificado de CA.</p> <p>[!DNL Workfront Fusion] no conserva ni almacena ningún dato (archivos, contraseñas) que proporcione aquí. El archivo y la contraseña solo se utilizan para extraer una clave privada o un certificado.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Después de introducir la información de conexión, haga clic en **[!UICONTROL Continuar]** para establecer una conexión.

## [!UICONTROL SFTP] módulos y sus campos

Al configurar [!UICONTROL SFTP] módulos, [!DNL Workfront Fusion] muestra los campos que se enumeran a continuación. Además de estos, se incluyen [!UICONTROL SFTP] pueden mostrarse los campos, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón de asignación encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Déclencheur

#### [!UICONTROL Ver archivos en una carpeta]

Devuelve archivos con detalles cuando se crea o cambia un archivo en una carpeta especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta SFTP a [!DNL Workfront Fusion], consulte <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Conectar SFTP a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Escriba o asigne la carpeta que desee ver. Puede especificar una ruta absoluta como <code>/home/user/</code>. O puede especificar una ruta relativa que señale a una carpeta específica del usuario que ha iniciado sesión, como <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>Tamaño del búfer [B]</td> 
   <td> <p> Introduzca el tamaño del búfer en bytes. El valor define el tamaño de los fragmentos transferidos desde el servidor. Algunos servidores pueden causar problemas o archivos dañados cuando el valor es demasiado alto.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de archivos devueltos]</td> 
   <td> <p> Establezca el número máximo de archivos que [!DNL Workfront Fusion] funcionará con durante un ciclo</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ver subcarpetas en una carpeta]

Devuelve carpetas con detalles cuando se crea o cambia una carpeta en una carpeta especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta SFTP a [!DNL Workfront Fusion], consulte <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Conectar SFTP a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Escriba o asigne la carpeta que desee ver. Puede especificar una ruta absoluta como <code>/home/user/</code>. O puede especificar una ruta relativa que señale a una carpeta específica del usuario que ha iniciado sesión, como <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de archivos devueltos]</td> 
   <td> <p> Establezca el número máximo de carpetas que [!DNL Workfront Fusion] volverá durante un ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Acciones

#### [!UICONTROL Enumerar el contenido de una carpeta]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta SFTP a [!DNL Workfront Fusion], consulte <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Conectar SFTP a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Show] </td> 
   <td> <p>Seleccione si desea recuperar archivos, carpetas o ambos.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Introduzca o asigne la carpeta que contiene los archivos o carpetas que desea enumerar. Puede especificar una ruta absoluta como <code>/home/user/</code>. O puede especificar una ruta relativa que señale a una carpeta específica del usuario que ha iniciado sesión, como <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Buscar] </td> 
   <td> <p>Introduzca o asigne el término de búsqueda. Por ejemplo, si desea buscar archivos con la extensión .txt, introduzca <code>.txt</code>.También puede introducir o asignar el nombre del archivo que desea buscar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordenar por]</td> 
   <td> <p> Seleccione si desea ordenar los resultados por nombre de archivo, tamaño, fecha de último acceso o fecha de la última modificación.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Orden] </td> 
   <td> <p>Seleccione si el resultado debe devolverse en orden ascendente o descendente.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Continúe con la ejecución de la ruta aunque el módulo no devuelva ningún resultado]</p> </td> 
   <td>Active esta opción para asegurarse de que este módulo no detenga el escenario si no devuelve resultados.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de resultados devueltos]</td> 
   <td> <p> Establezca el número máximo de resultados que [!DNL Workfront Fusion] volverá durante un ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener archivos]

Este módulo enumera los archivos de una carpeta especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta SFTP a [!DNL Workfront Fusion], consulte <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Conectar SFTP a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tamaño del búfer [B]]</td> 
   <td> <p> Introduzca el tamaño del búfer en bytes. El valor define el tamaño de los fragmentos transferidos desde el servidor. Algunos servidores pueden causar problemas o archivos dañados cuando el valor es demasiado alto.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Introduzca o asigne la carpeta que contiene los archivos o carpetas que desea enumerar. Puede especificar una ruta absoluta como <code>/home/user/</code>. O puede especificar una ruta relativa que señale a una carpeta específica del usuario que ha iniciado sesión, como <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Buscar] </td> 
   <td> <p>Introduzca o asigne el término de búsqueda. Por ejemplo, si desea buscar archivos con la extensión .txt, introduzca <code>.txt</code>.También puede introducir o asignar el nombre del archivo que desea buscar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordenar por]</td> 
   <td> <p> Seleccione si desea ordenar los resultados por nombre de archivo, tamaño, fecha de último acceso o fecha de la última modificación.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Orden]</td> 
   <td> <p> Seleccione si el resultado debe devolverse en orden ascendente o descendente.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Continúe con la ejecución de la ruta aunque el módulo no devuelva ningún resultado]</p> </td> 
   <td>Active esta opción para asegurarse de que este módulo no detenga el escenario si no devuelve resultados.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de resultados devueltos]</td> 
   <td> <p> Establezca el número máximo de archivos que [!DNL Workfront Fusion] volverá durante un ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener un archivo]

Este módulo recupera los detalles del archivo, incluidos los datos de un archivo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta SFTP a [!DNL Workfront Fusion], consulte <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Conectar SFTP a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tamaño del búfer [B]]</td> 
   <td> <p> Introduzca el tamaño del búfer en bytes. El valor define el tamaño de los fragmentos transferidos desde el servidor. Algunos servidores pueden causar problemas o archivos dañados cuando el valor es demasiado alto.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ruta de archivo] </td> 
   <td> <p>Introduzca la ruta al archivo. Puede especificar una ruta absoluta como <code>/home/user/file.txt</code>. O puede especificar una ruta relativa que señale a una carpeta específica del usuario que ha iniciado sesión, como <code>./file.txt</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Cargar un archivo]

Este módulo le permite cargar un archivo en el servidor SFTP.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta SFTP a [!DNL Workfront Fusion], consulte <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Conectar SFTP a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Especifique una carpeta existente como ubicación de almacenamiento del archivo. Puede especificar una ruta absoluta como <code>/home/user/</code>. O puede especificar una ruta relativa que señale a una carpeta específica del usuario que ha iniciado sesión, como <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Archivo de origen]</td> 
   <td> <p> Asigne el archivo de origen de un módulo anterior, como [!UICONTROL Dropbox] &gt; [!UICONTROL Get File]. También puede introducir o asignar el nombre de archivo y los datos del archivo.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Permisos]</p> </td> 
   <td> <p>Establezca los permisos deseados para el archivo o la carpeta. Utilice parámetros de chmod. Por ejemplo: <code>777 </code>o <code>-rwxrwxrwx</code>.</p> <p>Para obtener más información sobre chmod, consulte la <a href="https://ss64.com/bash/chmod.html">documentación de chmod</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Cambiar el nombre de un archivo]

Cambia el nombre de un archivo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta SFTP a [!DNL Workfront Fusion], consulte <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Conectar SFTP a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ruta de archivo]</td> 
   <td> <p> Introduzca la ruta al archivo al que desea cambiar el nombre. Puede especificar una ruta absoluta como <code>/home/user/file.txt</code>. O puede especificar una ruta relativa que señale a una carpeta específica del usuario que ha iniciado sesión, como <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nuevo nombre de archivo]</td> 
   <td> <p> Introduzca el nuevo nombre del archivo, incluida la extensión de archivo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mover un archivo]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta SFTP a [!DNL Workfront Fusion], consulte <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Conectar SFTP a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ruta de archivo]</td> 
   <td> <p> Introduzca la ruta al archivo que desea mover. Puede especificar una ruta absoluta como <code>/home/user/file.txt</code>. O puede especificar una ruta relativa que señale a una carpeta específica del usuario que ha iniciado sesión, como <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nueva carpeta]</td> 
   <td> <p> Introduzca la ruta a la nueva ubicación del archivo. Puede especificar una ruta absoluta como <code>/home/user/</code>. O puede especificar una ruta relativa que señale a una carpeta específica del usuario que ha iniciado sesión, como <code>./.</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar un archivo]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta SFTP a [!DNL Workfront Fusion], consulte <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Conectar SFTP a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ruta de archivo]</td> 
   <td> <p> Introduzca la ruta al archivo que desea eliminar. Puede especificar una ruta absoluta como <code>/home/user/file.txt</code>. O puede especificar una ruta relativa que señale a una carpeta específica del usuario que ha iniciado sesión, como <code>./file.txt</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actualizar permisos de archivos]

Permite cambiar los permisos del archivo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta SFTP a [!DNL Workfront Fusion], consulte <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Conectar SFTP a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ruta de archivo]</td> 
   <td> <p> Introduzca la ruta al archivo que desea mover. Puede especificar una ruta absoluta como <code>/home/user/file.txt</code>. O puede especificar una ruta relativa que señale a una carpeta específica del usuario que ha iniciado sesión, como <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Permisos]</p> </td> 
   <td> <p>Establezca los permisos de archivo que desee. Utilice los parámetros chmod. Por ejemplo, <code>777 </code>o <code>-rwxrwxrwx</code>.</p> <p>Debe coincidir con el patrón <code> /(.?([r-][w-][x-]){3})|[0-7]{3}/.</code></p> <p>Para obtener más información sobre chmod, consulte la <a href="https://ss64.com/bash/chmod.html">documentación de chmod</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear carpeta]

Crea una nueva carpeta en la ubicación especificada.

>[!NOTE]
>
>Si la carpeta ya existe, el módulo generará un error. Para continuar con el flujo sin pausarlo, adjunte una ruta de controlador de error al módulo para captar el error y emplee la variable [!UICONTROL Reanudar] para continuar con el flujo. Para obtener información sobre cómo adjuntar una ruta de controlador de error, consulte [Gestión de errores en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md). Para obtener información sobre la ruta del controlador de errores, consulte [Directivas para la gestión de errores en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta SFTP a [!DNL Workfront Fusion], consulte <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Conectar SFTP a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Especifique una carpeta existente como ubicación de almacenamiento para la nueva carpeta. Puede especificar una ruta absoluta como <code>/home/user/file.txt</code>. O puede especificar una ruta relativa que señale a una carpeta específica del usuario que ha iniciado sesión, como <code>./</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder Name]</td> 
   <td> <p> Introduzca el nombre de la carpeta.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Permisos]</p> </td> 
   <td> <p>Establezca los permisos de carpeta deseados. Utilice parámetros de chmod. Por ejemplo, <code>777 </code>o <code>-rwxrwxrwx</code>.</p> <p>Debe coincidir con el patrón <code>/(.?([r-][w-][x-]){3})|[0-7]{3}/.</code></p> <p>Para obtener más información sobre chmod, consulte la <a href="https://ss64.com/bash/chmod.html">Página principal de chmod</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar una carpeta]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta SFTP a [!DNL Workfront Fusion], consulte <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Conectar SFTP a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Folder Path]</td> 
   <td> <p> Especifique la ruta a la carpeta que desea eliminar. Puede especificar una ruta absoluta como <code>/home/user/</code>. O puede especificar una ruta relativa que señale a una carpeta específica del usuario que ha iniciado sesión, como <code>./.</code></p> </td> 
  </tr> 
 </tbody> 
</table>
