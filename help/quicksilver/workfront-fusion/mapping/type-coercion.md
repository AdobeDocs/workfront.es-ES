---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Coerción de tipo en Adobe Workfront Fusion
description: Este documento describe cómo [!DNL Adobe Workfront Fusion] se comporta en situaciones en las que recibe valores en formatos de datos esperados e inesperados.
author: Becky
feature: Workfront Fusion
exl-id: 847a17c9-bd67-4132-81a8-2a5fe8d516cb
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 1%

---

# Coerción de tipo en [!DNL Adobe Workfront Fusion]

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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de [!UICONTROL Adobe Workfront Fusion**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

### Coerción de tipo

Este documento describe cómo [!DNL Adobe Workfront Fusion] se comporta en situaciones en las que recibe valores en formatos de datos esperados e inesperados.

<table style="table-layout:auto">
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Previsto</th> 
   <th>Recibido</th> 
   <th> <p>Descripción</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>matriz </td> 
   <td>matriz </td> 
   <td> <p>El valor se entrega sin cambios.</p> </td> 
  </tr> 
  <tr> 
   <td>matriz </td> 
   <td>other </td> 
   <td> <p>Si el valor recibido no es del tipo de matriz, [!DNL Workfront Fusion] creará una matriz y el primer elemento (y el único) será el valor recibido.</p> </td> 
  </tr> 
  <tr> 
   <td>booleano </td> 
   <td>booleano </td> 
   <td> <p>El valor se entrega sin cambios.</p> </td> 
  </tr> 
  <tr> 
   <td>booleano </td> 
   <td>number </td> 
   <td> <p>El valor se convierte en Sí lógico, incluso si el valor es 0.</p> </td> 
  </tr> 
  <tr> 
   <td>booleano </td> 
   <td>text </td> 
   <td> <p>Si el valor es igual a false o si el valor está vacío, se convierte en No lógico. Si no es así, se convierte en Sí lógico.</p> </td> 
  </tr> 
  <tr> 
   <td>booleano </td> 
   <td>other </td> 
   <td> <p>El valor se convierte en Sí lógico siempre que exista el valor recibido (no es nulo).</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>buffer </td> 
   <td> <p>El valor se entrega sin cambios solo si la página de códigos se ajusta a lo esperado. Si la página de códigos es diferente, [!DNL Workfront Fusion] intentará convertir el valor recibido a la página de códigos solicitada. Si no se admite esta conversión, [!DNL Workfront Fusion] devolverá un error de validación.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>booleano </td> 
   <td> <p>El valor se convierte en texto (true/false) y, a continuación, en datos binarios siguiendo los pasos mencionados anteriormente para la conversión a texto.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>date </td> 
   <td> <p>El valor se convierte a texto ISO 8601 y, a continuación, a datos binarios siguiendo los pasos mencionados para convertir a texto.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>number </td> 
   <td> <p>El valor se convierte en texto y, a continuación, en datos binarios siguiendo los pasos mencionados anteriormente para la conversión a texto.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>text </td> 
   <td> <p>El valor se convierte en datos binarios y se codifica según lo esperado. Si no se especifica la codificación esperada, se utilizará la codificación utf8.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>other </td> 
   <td> <p>[!DNL Workfront Fusion] devuelve un error de validación.</p> </td> 
  </tr> 
  <tr> 
   <td>colección </td> 
   <td>colección </td> 
   <td> <p>El valor se entrega sin cambios.</p> </td> 
  </tr> 
  <tr> 
   <td>colección </td> 
   <td>other </td> 
   <td> <p>[!DNL Workfront Fusion] devuelve un error de validación.</p> </td> 
  </tr> 
  <tr> 
   <td>date </td> 
   <td>date </td> 
   <td> <p>El valor se entrega sin cambios.</p> </td> 
  </tr> 
  <tr> 
   <td>date </td> 
   <td>text </td> 
   <td> <p>[!DNL Workfront Fusion] intentará convertir el texto a una fecha. Si la conversión falla, devolverá un error de validación. La fecha debe contener día, mes y año. La fecha puede contener zona horaria y horaria. La zona horaria predeterminada se basa en su configuración. Ejemplos:</p> <p><code>2016-06-20T17:26:44.356Z</code> </p> <p><code>2016-06-20 19:26:44 GMT+02:00</code> </p> <p><code>2016-06-20 19:26+0200</code> </p> <p><code>2016-06-20 17:26:44</code> </p> <p><code>2016-06-20</code> </p> <p><code>2016/06/20 17:26:44</code> </p> <p><code>2016/06/20 19:26:44+02:00</code> </p> <p><code>2016/06/20 17:26</code> </p> <p><code>2016/06/20 5:26 PM</code> </p> <p><code>2016/06/20</code> </p> <p><code>06/20/2016 17:26:44</code> </p> <p><code>06/20/2016 19:26:44+02:00</code> </p> <p><code>06/20/2016 17:26</code> </p> <p><code>06/20/2016 5:26 PM</code> </p> <p><code>06/20/2016</code> </p> <p><code>20.6.2016 17:26:44</code> </p> <p><code>20.6.2016 19:26:44+02:00</code> </p> <p><code>20.6.2016 17:26</code> </p> <p><code>20.6.2016</code> </p> </td> 
  </tr> 
  <tr> 
   <td>date </td> 
   <td>other </td> 
   <td> <p>[!DNL Workfront Fusion] devuelve un error de validación.</p> </td> 
  </tr> 
  <tr> 
   <td>number </td> 
   <td>number </td> 
   <td> <p>El valor se entrega sin cambios.</p> </td> 
  </tr> 
  <tr> 
   <td>number </td> 
   <td>text </td> 
   <td> <p>[!DNL Workfront Fusion] intentará convertir el texto en un número. Si la conversión falla, devolverá un error de validación.</p> </td> 
  </tr> 
  <tr> 
   <td>number </td> 
   <td>other </td> 
   <td> <p>[!DNL Workfront Fusion] devuelve un error de validación.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>text </td> 
   <td> <p>El valor se entrega sin cambios.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>matriz </td> 
   <td> <p>Si la matriz dada admite la conversión a texto, el valor se convertirá. Si no, [!DNL Workfront Fusion] devolverá un error de validación.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>booleano </td> 
   <td> <p>El valor se convierte en texto (verdadero/falso).</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>buffer </td> 
   <td> <p>Si se especifica la codificación de texto para los datos binarios, el valor se convertirá a texto. Si no, [!DNL Workfront Fusion] devolverá un error de validación.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>date </td> 
   <td> <p>El valor se convierte al texto ISO 8601.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>number </td> 
   <td> <p>El valor se convierte en texto.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>other </td> 
   <td> <p>[!DNL Workfront Fusion] devuelve un error de validación.</p> </td> 
  </tr> 
  <tr> 
   <td>hora </td> 
   <td>hora </td> 
   <td> <p>El valor se entrega sin cambios.</p> </td> 
  </tr> 
  <tr> 
   <td>hora </td> 
   <td>text </td> 
   <td> <p>[!DNL Workfront Fusion] intentará convertir el tiempo a las horas:minutes:formato de segundos. Si la conversión falla, devolverá un error de validación.</p> </td> 
  </tr> 
  <tr> 
   <td>hora </td> 
   <td>other </td> 
   <td> <p>[!DNL Workfront Fusion] devuelve un error de validación.</p> </td> 
  </tr> 
 </tbody> 
</table>
