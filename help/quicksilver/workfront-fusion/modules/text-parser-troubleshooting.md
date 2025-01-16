---
content-type: tips-tricks-troubleshooting
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Solución de problemas del analizador de texto en  [!DNL Adobe Workfront Fusion]
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 8a3821cf-d0c6-4917-86e7-90a4872a5795
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 85%

---

# Solución de problemas del analizador de texto en [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Analizador de texto](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/tools-and-transformers/text-parser.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

Utilice esta información si no consigue que el analizador de texto genere ninguna salida.

## Requisitos de acceso

Para utilizar la funcionalidad de este artículo debe tener el siguiente acceso:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] o superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia** de [!UICONTROL Adobe Workfront Fusion]</td> 
   <td>
   <p>Requisito de licencia actual: no se requiere la licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Producto</td> 
   <td>
   <p>Requisito de producto actual: si tiene el plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] su organización debe adquirir [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en el plan [!DNL Workfront] de [!UICONTROL Ultimate].</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] y [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Resolución de problemas

Ejemplo de escenario de caso: desea analizar el tipo de archivo de un documento de archivo “filename.docx” y la extensión del nombre de archivo siempre varía de DOCX a PDF o CSV.

La expresión que puede elegir usar en este caso es [!DNL \..+]

Si la tuviera que utilizar en la expresión regex en regex101.com, obtendría una coincidencia completa.

![](assets/regex-expression-350x130.png)

En la imagen anterior, la extensión de archivo coincidía correctamente. Si intenta implementarlo en el analizador de texto:

![](assets/text-parser-350x602.png)

no obtendrá ninguna coincidencia:

![](assets/text-parser-you-dont-get-a-match-350x365.png)

La razón es que la “i” muestra solo el número de coincidencias por coincidencia, así que en este caso tenemos 2 coincidencias, por lo que después de la “i” hay un valor numérico 1 y 2. El caso de uso es que, si alguna vez necesita hacer coincidir o transferir datos a través de un filtro, solo el segundo valor coincidente puede especificar qué valor está representado mediante el valor numérico.

![](assets/text-parser-matches-350x355.png)

Para poder obtener los valores de coincidencia necesarios para añadir corchetes a la parte que desea analizar (por ejemplo, para extraer de “filename.docx” solo “docx”), los corchetes deben aplicarse en \, de acuerdo con la expresión regex que se utiliza en este escenario de caso.(.+)

Esto captura el DOCX, lo coloca en un grupo y deja el “.” fuera.

![](assets/text-parser-get-matches-350x592.png)

En la salida que se muestra en la imagen siguiente, el grupo de captura coincidirá con cualquier carácter (excepto para los terminadores de línea).

![](assets/text-parser-output-350x389.png)

Otra solución que también incorpora regex es utilizar la función de reemplazo

`{{replace("abcdefghijklmno pqr stuvw xyz.docx"; "/.\./"; ".")}}`

A continuación, reemplace `abcdefghijklmno pqr stuvw xyz.docx` por la variable de nombre de archivo real.
