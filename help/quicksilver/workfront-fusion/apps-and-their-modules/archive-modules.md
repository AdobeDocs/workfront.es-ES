---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Archivar módulos
description: En un  [!DNL Adobe Workfront Fusion] escenario, puede conectar un archivo, como un archivo comprimido, a varias aplicaciones y servicios de terceros. Por ejemplo, puede configurar un escenario que
author: Becky
feature: Workfront Fusion
exl-id: e29b6d39-3666-4d6d-a178-1983ae9f3aa9
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---

# [!UICONTROL Archivar] módulos

En un escenario de [!DNL Adobe Workfront Fusion], puede usar un archivo, como un archivo comprimido, en su escenario, lo que le permite utilizarlo en sus automatizaciones o integraciones.

Si necesita instrucciones para crear un escenario, consulte [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Para obtener información acerca de los módulos, vea [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## [!UICONTROL Archivar] módulos y sus campos

Al configurar los módulos [!UICONTROL Archive], [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con ellos, podrían mostrarse [!UICONTROL Archivar] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, vea [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Extraer un archivo]](#extract-an-archive)
* [[!UICONTROL Crear un archivo]](#create-an-archive)
* [[!UICONTROL Inflar]](#inflate)
* [[!UICONTROL Deflación]](#deflate)

## [!UICONTROL Extraer un archivo]

Este módulo de acción extrae un archivo que identifica de un archivo.

El módulo devuelve el ID del archivo y cualquier campo asociado, junto con cualquier campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL archivo Source]</td> 
   <td> <p> Seleccione el archivo que desee extraer. Este archivo se puede asignar desde un módulo anterior (como el módulo [!DNL Workfront] &gt;[!UICONTROL Descargar un documento]).</p>  </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Ejemplo:** Obtenga el archivo ZIP de la carpeta [!DNL Dropbox] definida (por ejemplo, Archivos), extráigalo mediante el módulo [!UICONTROL Archivar] y envíe los archivos extraídos a la dirección de correo electrónico deseada como archivos adjuntos con el módulo [!UICONTROL Correo electrónico] o [!DNL Gmail].
>
>![](assets/example-dropbox-350x134.png)

## [!UICONTROL Crear un archivo]

Este módulo de agregador agrega los archivos deseados a un archivo [!UICONTROL ZIP] o [!UICONTROL TAR].

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Source module]</td> 
   <td> <p> Seleccione el módulo desde el que desea recuperar los archivos.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo] </td> 
   <td> <p>Seleccione si desea agregar archivos a un archivo [!UICONTROL ZIP] o a un archivo [!UICONTROL TAR].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Comentario]</td> 
   <td>Escriba un comentario que desee agregar al archivo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Agrupar por]</td> 
   <td> <p>Defina una expresión por la que desee agrupar la salida agregada. Esta expresión puede contener uno o varios elementos asignados. Los datos agregados se separan en grupos utilizando el valor de esta expresión. Cada grupo genera como un paquete independiente con una clave (la expresión evaluada) y un valor (el texto agregado). Puede utilizar la clave como filtro en módulos posteriores.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Detener procesamiento después de una agregación vacía]</td> 
   <td>Seleccione esta opción para detener el escenario cuando no haya resultados.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre de archivo]</td> 
   <td> <p> Introduzca un nombre para el archivo creado. No añada una extensión.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL archivo Source]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Ejemplo:** Vea los correos electrónicos entrantes usando el módulo [!DNL Gmail] >[!UICONTROL Ver correos electrónicos]. Si se recibe un correo electrónico, los archivos adjuntos se iteran en paquetes individuales y, a continuación, se archivan en el archivo [!DNL ZIP] y se guardan en la carpeta del Dropbox definida.
>
>![](assets/example-gmail-350x102.png)

## [!UICONTROL Inflar]

Este módulo transformador descomprime datos binarios usando un algoritmo de inflación.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Datos] </td> 
   <td> <p>Introduzca o asigne los datos que desea descomprimir con la función de inflado.</p> </td> 
  </tr> 
 </tbody> 
</table>

## [!UICONTROL Deflación]

Este módulo transformador comprime datos binarios usando un algoritmo de deflación.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Datos] </td> 
   <td> <p>Introduzca o asigne los datos que desea comprimir con la función deflate.</p> </td> 
  </tr> 
 </tbody> 
</table>
