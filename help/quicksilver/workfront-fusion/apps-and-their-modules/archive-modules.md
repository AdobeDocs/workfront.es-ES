---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Archivar módulos
description: En un [!DNL Adobe Workfront Fusion] en este caso, puede conectar un archivo, como un archivo comprimido, a varias aplicaciones y servicios de terceros. Por ejemplo, puede configurar un escenario que
author: Becky
feature: Workfront Fusion
exl-id: e29b6d39-3666-4d6d-a178-1983ae9f3aa9
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---

# [!UICONTROL Archivo] módulos

En un [!DNL Adobe Workfront Fusion] , puede utilizar un archivo, como un archivo comprimido, en su situación, lo que le permite utilizarlo en sus automatizaciones o integraciones.

Si necesita instrucciones para crear un escenario, consulte [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Para obtener información sobre los módulos, consulte [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## [!UICONTROL Archivo] módulos y sus campos

Al configurar [!UICONTROL Archivo] módulos, [!DNL Workfront Fusion] muestra los campos que se enumeran a continuación. Además de estos, se incluyen [!UICONTROL Archivo] pueden mostrarse los campos, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón de asignación encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Extraer un archivo]](#extract-an-archive)
* [[!UICONTROL Crear un archivo]](#create-an-archive)
* [[!UICONTROL Inflar]](#inflate)
* [[!UICONTROL Desglosar]](#deflate)

## [!UICONTROL Extraer un archivo]

Este módulo de acción extrae un archivo que se identifica de un archivo.

El módulo devuelve el ID del archivo y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Archivo de origen]</td> 
   <td> <p> Seleccione el archivo que desea extraer. Este archivo se puede asignar desde un módulo anterior (como el [!DNL Workfront] &gt;[!UICONTROL Descargar un módulo de documento]).</p>  </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Ejemplo:** Obtenga el archivo ZIP de la [!DNL Dropbox] carpeta (por ejemplo, Archives), extráigala utilizando la [!UICONTROL Archivo] y enviar archivos extraídos a la dirección de correo electrónico deseada como archivos adjuntos con la variable [!UICONTROL Correo electrónico] o [!DNL Gmail] módulo.
>
>![](assets/example-dropbox-350x134.png)

## [!UICONTROL Crear un archivo]

Este módulo de agregador agrega los archivos deseados a un [!UICONTROL ZIP] o [!UICONTROL TAR] archivo.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Source module]</td> 
   <td> <p> Seleccione el módulo desde el que desea recuperar los archivos.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type] </td> 
   <td> <p>Seleccione si desea añadir archivos a un archivo [!UICONTROL ZIP] o a un archivo [!UICONTROL TAR].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Comentario]</td> 
   <td>Escriba un comentario que desee agregar al archivo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Group by]</td> 
   <td> <p>Defina una expresión por la que desee agrupar la salida agregada. Esta expresión puede contener uno o más elementos asignados. Los datos agregados se separan en grupos utilizando el valor de esta expresión. Cada grupo genera un paquete independiente con una clave (la expresión evaluada) y un valor (el texto agregado). Puede utilizar la clave como filtro en los módulos siguientes.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Detenga el procesamiento después de una agregación vacía]</td> 
   <td>Seleccione esta opción para detener el escenario cuando no haya resultados.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre del archivo]</td> 
   <td> <p> Introduzca un nombre para el archivo creado. No agregue ninguna extensión.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Ejemplo:** Vea los correos electrónicos entrantes usando el [!DNL Gmail] >[!UICONTROL Ver correos electrónicos] módulo. Si se recibe un correo electrónico, sus archivos adjuntos se iteran en paquetes individuales y luego se archivan en el [!DNL ZIP] y se guarda en la carpeta de Dropbox definida.
>
>![](assets/example-gmail-350x102.png)

## [!UICONTROL Inflar]

Este módulo de transformador descomprime los datos binarios usando un algoritmo de inflación.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data] </td> 
   <td> <p>Introduzca o asigne los datos que desea descomprimir utilizando la función inflate .</p> </td> 
  </tr> 
 </tbody> 
</table>

## [!UICONTROL Desglosar]

Este módulo de transformador comprime los datos binarios utilizando un algoritmo de deflación.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data] </td> 
   <td> <p>Introduzca o asigne los datos que desea comprimir con la función deflate .</p> </td> 
  </tr> 
 </tbody> 
</table>
