---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Módulos de archivo
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: e29b6d39-3666-4d6d-a178-1983ae9f3aa9
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 87%

---

# Módulos de [!UICONTROL Archivo]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Módulos de archivo](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/tools-and-transformers/archive-modules.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

En un escenario de [!DNL Adobe Workfront Fusion], puede usar un archivo, como un archivo comprimido, en su escenario, lo que le permite utilizarlo en sus automatizaciones o integraciones.

Si necesita instrucciones para crear un escenario, consulte [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Para obtener información sobre los módulos, consulte [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Módulos de [!UICONTROL Archivo] y sus campos

Al configurar los módulos de [!UICONTROL Archivo], [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con ellos, podrían mostrarse campos adicionales de [!UICONTROL Archivo], según determinados factores como su nivel de acceso en la aplicación o el servicio. El título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Extraer un archivo]](#extract-an-archive)
* [[!UICONTROL Crear un archivo]](#create-an-archive)
* [[!UICONTROL Inflar]](#inflate)
* [[!UICONTROL Desinflar]](#deflate)

## [!UICONTROL Extraer un archivo]

Este módulo de acción extrae un archivo que usted identifica en un archivo.

El módulo devuelve el identificador del archivo y cualquier campo asociado, junto con cualquier otro campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Source file]</td> 
   <td> <p> Seleccione el archivo que desee extraer. Este archivo se puede asignar desde un módulo anterior (como el módulo &gt;[!UICONTROL Download a document] de [!DNL Workfront]).</p>  </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Ejemplo:** obtenga el archivo ZIP de la carpeta [!DNL Dropbox] definida (por ejemplo, Archivos), extráigalo mediante el módulo de [!UICONTROL Archivo] y envíe los archivos extraídos a la dirección de correo electrónico deseada como archivos adjuntos con el módulo de [!UICONTROL Correo electrónico] o de [!DNL Gmail].
>
>![](assets/example-dropbox-350x134.png)

## [!UICONTROL Crear un archivo]

Este módulo de agregación añade los archivos deseados a un archivo [!UICONTROL ZIP] o [!UICONTROL TAR].

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Source module]</td> 
   <td> <p> Seleccione el módulo del que desea recuperar los archivos.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type] </td> 
   <td> <p>Seleccione si desea añadir los archivos a un archivo [!UICONTROL ZIP] o a un archivo [!UICONTROL TAR].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Comment]</td> 
   <td>Escriba cualquier comentario que desee añadir al archivo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Group by]</td> 
   <td> <p>Defina una expresión por la cual desea agrupar la salida agregada. Esta expresión puede contener uno o varios elementos asignados. Los datos agregados se separarán entonces en grupos utilizando el valor de esta expresión. Cada grupo genera como un paquete independiente con una clave (la expresión evaluada) y un valor (el texto añadido). Puede utilizar la clave como filtro en módulos posteriores.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Stop processing after an empty aggregation]</td> 
   <td>Seleccione esta opción para detener el escenario cuando no haya resultados.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Archive name]</td> 
   <td> <p> Introduzca un nombre para el archivo creado. No añada ninguna extensión.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source file]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Ejemplo:** Vea los correos electrónicos entrantes con el módulo [!DNL Gmail] > [!UICONTROL Ver correos electrónicos]. Si se recibe un correo electrónico, los archivos adjuntos se repiten en paquetes individuales y, a continuación, se archivan en el archivo [!DNL ZIP] y se guardan en la carpeta Dropbox definida.
>
>![](assets/example-gmail-350x102.png)

## [!UICONTROL Inflar]

Este módulo transformador descomprime datos binarios usando un algoritmo de inflación.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data] </td> 
   <td> <p>Introduzca o asigne los datos que desea descomprimir con la función de inflado.</p> </td> 
  </tr> 
 </tbody> 
</table>

## [!UICONTROL Desinflar]

Este módulo transformador comprime datos binarios usando un algoritmo de desinflado.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data] </td> 
   <td> <p>Introduzca o asigne los datos que desea comprimir con la función de desinflado.</p> </td> 
  </tr> 
 </tbody> 
</table>
