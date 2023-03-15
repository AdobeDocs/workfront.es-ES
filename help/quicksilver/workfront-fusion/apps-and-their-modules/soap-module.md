---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Módulo SOAP
description: Puede utilizar el módulo SOAP para conectarse a las API SOAP en Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 752e0766-25f2-4d22-bed5-7c931284258d
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

# [!UICONTROL SOAP] módulo

Puede usar la variable [!UICONTROL SOAP] módulo a conectar [!UICONTROL SOAP] API en [!UICONTROL Adobe Workfront Fusion].

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

## Al usar la variable [!UICONTROL SOAP] módulo

La variable [!UICONTROL SOAP] está actualmente en fase beta y no admite:

* Redefinir elementos
* Restricciones de dígitos de fracción
* Restricciones totales de dígitos
* Restricciones de espacio en blanco
* Múltiples partes en mensajes de entrada y salida. Solo se admiten mensajes de una sola parte
* Elementos de esquema XML personalizados definidos con la ayuda de [[!UICONTROL SOAP] Codificación](http://schemas.xmlsoap.org) esquemas y elementos.

>[!INFO]
>
>**Ejemplo:**
>  
>Los siguientes no serían reconocidos correctamente por [!UICONTROL Workfront Fusion]:
>
>```
><complexType name="ArrayOfFloat">
>
>     <complexContent>
>
>          <restriction base="soapenc:Array">
>
>               <attribute ref="soapenc:arrayType"
>
>                       wsdl:arrayType="xsd:integer[]"/>
>
>           </restriction>
>
>     </complexContent>
>
></complexType>
>```

Incluye el `soapenc:Array`, `soapenc:arrayType` y `wsdl:arrayType` referencias, que aún no son compatibles con [!UICONTROL Workfront Fusion].

## Solución alternativa

Si la variable [!UICONTROL SOAP] El módulo de se niega a procesar el archivo WSDL o genera varios errores en la configuración del módulo, puede intentar usar el **[!UICONTROL HTTP] > [!UICONTROL Realizar una solicitud]** en su lugar:

1. En [!DNL Workfront Fusion], cree un nuevo escenario.
1. Inserte el **[!UICONTROL HTTP] > [!UICONTROL Realizar una solicitud]** en el escenario.
1. Abra la configuración del módulo y rellene los campos siguientes:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Método]</td> 
      <td> <p>[!UICONTROL POST]</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Tipo de cuerpo]</td> 
      <td> <p>[!UICONTROL Raw]</p> </td> [!UICONTROL ]
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Content type]</td> 
      <td> <p>[!UICONTROL XML (application/xml)]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Parse response]</td> 
      <td>[!UICONTROL Habilitado]</td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/workaround-350x443.png)

1. Abra una nueva ventana o pestaña del explorador web.
1. Pegue la dirección URL de WSDL en la barra de direcciones del explorador web y busque el archivo XML.

   La URL WSDL normalmente termina con `?wsdl`, pero no necesariamente, por ejemplo `http://voip.ms/api/v1/server.wsdl`.

1. Si el archivo WSDL no se muestra directamente en el explorador web, abra el archivo descargado en un editor de texto.
1. Busque la variable `<service>` o `<wsdl:service>` etiqueta:

   ![](assets/service-350x65.png)

1. Una vez localizada, copie la dirección URL de la página `location` atributo.
1. En [!DNL Workfront Fusion], pegue la dirección URL en el campo URL del módulo HTTP.
1. Abra el [En línea [!UICONTROL SOAP] Cliente](https://wsdlbrowser.com/) en una nueva ventana o pestaña del explorador web.
1. Pegue la URL WSDL en el campo URL WSDL .
1. Haga clic en **[!UICONTROL Examinar]**.
1. Elija entre la lista de funciones y la izquierda, por ejemplo `getLanguages`.
1. Copie el contenido del [!UICONTROL Solicitar XML] área de texto.
1. En [!UICONTROL Workfront Fusion], pegue el contenido copiado en el campo URL del módulo.
1. Proporcione valores para los parámetros seleccionados reemplazando los signos de interrogación por valores reales:

   ![](assets/request-xml-350x172.png)

1. Cierre la configuración del módulo haciendo clic en **[!UICONTROL OK]**.
1. Ejecute el escenario o módulo.
