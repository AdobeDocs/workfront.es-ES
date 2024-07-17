---
content-type: tips-tricks-troubleshooting
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Solución de problemas del analizador de texto en  [!DNL Adobe Workfront Fusion]
description: Utilice esta información si no puede obtener un analizador de texto para generar ningún resultado.
author: Becky
feature: Workfront Fusion
exl-id: 8a3821cf-d0c6-4917-86e7-90a4872a5795
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# Solución de problemas del analizador de texto en [!DNL Adobe Workfront Fusion]

Utilice esta información si no puede obtener un analizador de texto para generar ningún resultado.

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Requisito de licencia actual: no se requiere licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
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

## Resolución de problemas

Por ejemplo, si desea analizar el tipo de archivo de un documento de archivo &quot;filename.docx&quot; y la extensión del nombre de archivo siempre varía de DOCX a PDF o CSV.

La expresión que puede elegir usar en este caso es [!DNL \..+]

Si tuviera que utilizar esto en la expresión regex en regex101.com, obtendría una coincidencia completa.

![](assets/regex-expression-350x130.png)

En la imagen anterior, la extensión de archivo coincidía correctamente. Si toma esto e intenta implementarlo en su analizador de texto:

![](assets/text-parser-350x602.png)

no obtendrá ninguna coincidencia:

![](assets/text-parser-you-dont-get-a-match-350x365.png)

La razón de esto es que la &quot;i&quot; muestra solo el número de coincidencias por coincidencia, así que en este caso, tenemos 2 coincidencias, por lo tanto después de la &quot;i&quot; hay un valor numérico 1 y 2. El caso de uso para esto es que, en caso de que alguna vez necesite hacer coincidir o pasar datos a través de un filtro, solo el segundo valor coincidente, puede especificar qué valor que se representa mediante el valor numérico.

![](assets/text-parser-matches-350x355.png)

Para poder obtener los valores de coincidencia necesarios para agregar corchetes a la parte que desea analizar (por ejemplo, para extraer solo de &quot;filename.docx&quot; - &quot;docx&quot;), los corchetes deben aplicarse en \ según la expresión regex que se utilice en este escenario de caso.(.+)

Esto captura el DOCX, lo coloca en un grupo y deja el &quot;&quot;. fuera de él.

![](assets/text-parser-get-matches-350x592.png)

En la salida que se muestra en la imagen siguiente, el grupo de captura coincidirá con cualquier carácter (excepto para los terminadores de línea).

![](assets/text-parser-output-350x389.png)

Otra solución que también incorpora regex es utilizar la función de reemplazo

`{{replace("abcdefghijklmno pqr stuvw xyz.docx"; "/.\./"; ".")}}`

A continuación, reemplace `abcdefghijklmno pqr stuvw xyz.docx` por la variable de nombre de archivo real.
