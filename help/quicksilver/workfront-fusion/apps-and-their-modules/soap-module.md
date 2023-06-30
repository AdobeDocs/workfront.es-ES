---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulo SOAP
description: Puede utilizar el módulo SOAP para conectarse a las API de SOAP en Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 752e0766-25f2-4d22-bed5-7c931284258d
source-git-commit: e61dc6646e221cffb30aad055663dcf8fd3299e2
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 1%

---

# [!UICONTROL Módulo SOAP]

Puede usar el complemento [!UICONTROL JABÓN] módulo al que conectarse [!UICONTROL JABÓN] API en [!UICONTROL Adobe Workfront Fusion].

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
   <p>Requisito de licencia actual: No [!DNL Workfront Fusion] requisito de licencia.</p>
   <p>O</p>
   <p>Requisito de licencia heredada: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Requisito actual del producto: si tiene [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Uso del [!UICONTROL JABÓN] módulo

El [!UICONTROL JABÓN] El módulo está actualmente en fase beta y no admite:

* Redefinir elementos
* Restricciones de dígitos de fracción
* Total de restricciones de dígitos
* Restricciones de espacio en blanco
* Varias partes en los mensajes de entrada y salida. Solo se admiten mensajes de una sola parte
* Elementos de esquema XML personalizados definidos con la ayuda de [[!UICONTROL JABÓN] Codificación](http://schemas.xmlsoap.org) esquemas y elementos.

>[!INFO]
>
>**Ejemplo:**
>  
>Las siguientes no serían reconocidas correctamente por [!UICONTROL Workfront Fusion]:
>
>```
><complexType name="ArrayOfFloat">
>     <complexContent>
>           <restriction base="soapenc:Array">
>                 <attribute ref="soapenc:arrayType"
>                       wsdl:arrayType="xsd:integer[]"/>
>           </restriction>
>     </complexContent>
></complexType>
>```

Incluye el `soapenc:Array`, `soapenc:arrayType` y `wsdl:arrayType` referencias, que aún no son compatibles con [!UICONTROL Workfront Fusion].

## Solución alternativa

Si la variable [!UICONTROL JABÓN] El módulo rechaza procesar el archivo WSDL o genera varios errores en la configuración del módulo. Puede intentar utilizar el **[!UICONTROL HTTP] > [!UICONTROL Realizar una solicitud]** en su lugar:

1. Entrada [!DNL Workfront Fusion], cree un nuevo escenario.
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
      <td role="rowheader">[!UICONTROL Tipo de contenido]</td> 
      <td> <p>[!UICONTROL XML (application/xml)]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Respuesta de análisis]</td> 
      <td>[!UICONTROL Habilitado]</td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/workaround-350x443.png)

1. Abra una nueva ventana o pestaña del explorador web.
1. Pegue la URL de WSDL en la barra de direcciones del explorador web y recupere el archivo XML.

   La URL de WSDL suele terminar con `?wsdl`, pero no necesariamente, por ejemplo `http://voip.ms/api/v1/server.wsdl`.

1. Si el archivo WSDL no se muestra directamente en el explorador web, abra el archivo descargado en un editor de texto.
1. Busque la variable `<service>` o `<wsdl:service>` etiqueta:

   ![](assets/service-350x65.png)

1. Una vez localizada, copie la dirección URL del `location` atributo.
1. Entrada [!DNL Workfront Fusion], pegue la dirección URL en el campo URL del módulo HTTP.
1. Abra el [En línea [!UICONTROL JABÓN] Cliente](https://wsdlbrowser.com/) en una nueva ventana o pestaña del explorador web.
1. Pegue la URL de WSDL en el campo URL de WSDL.
1. Clic **[!UICONTROL Examinar]**.
1. Elija de la lista de funciones a la izquierda, por ejemplo `getLanguages`.
1. Copie el contenido del [!UICONTROL Solicitar XML] área de texto.
1. Entrada [!UICONTROL Workfront Fusion], pegue el contenido copiado en el campo URL del módulo.
1. Proporcione valores para los parámetros seleccionados reemplazando los signos de interrogación por valores reales:

   ![](assets/request-xml-350x172.png)

1. Cierre la configuración del módulo haciendo clic en **[!UICONTROL OK]**.
1. Ejecute el escenario o módulo.
