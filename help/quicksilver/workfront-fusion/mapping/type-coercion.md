---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Coerción de tipos en Adobe Workfront Fusion
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 847a17c9-bd67-4132-81a8-2a5fe8d516cb
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 23%

---

# Coerción de tipos en [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Coerción de tipos](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/mapping-panel/data-types/type-coercion.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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

+++

### Coerción de tipo

Este documento describe cómo se comporta [!DNL Adobe Workfront Fusion] en situaciones en las que recibe valores en formatos de datos esperados e inesperados.

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
   <td>otro </td> 
   <td> <p>Si el valor recibido no es del tipo de matriz, [!DNL Workfront Fusion] creará una matriz y el primer (y único) elemento será el valor recibido.</p> </td> 
  </tr> 
  <tr> 
   <td>booleano </td> 
   <td>booleano </td> 
   <td> <p>El valor se entrega sin cambios.</p> </td> 
  </tr> 
  <tr> 
   <td>booleano </td> 
   <td>number </td> 
   <td> <p>El valor se convierte en lógico Sí, incluso si el valor es 0.</p> </td> 
  </tr> 
  <tr> 
   <td>booleano </td> 
   <td>texto </td> 
   <td> <p>Si el valor es igual a falso o el valor está vacío, se convierte en el valor lógico No. Si no es así, se convierte en un Sí lógico.</p> </td> 
  </tr> 
  <tr> 
   <td>booleano </td> 
   <td>otro </td> 
   <td> <p>El valor se convierte en lógico Sí siempre que exista el valor recibido (no es nulo).</p> </td> 
  </tr> 
  <tr> 
   <td>amortiguador </td> 
   <td>amortiguador </td> 
   <td> <p>El valor se entrega sin cambios solo si la página de códigos cumple lo esperado. Si la página de códigos difiere, [!DNL Workfront Fusion] intentará convertir el valor recibido a la página de códigos solicitada. Si no se admite esta conversión, [!DNL Workfront Fusion] devolverá un error de validación.</p> </td> 
  </tr> 
  <tr> 
   <td>amortiguador </td> 
   <td>booleano </td> 
   <td> <p>El valor se convierte en texto (true/false) y, a continuación, en datos binarios, siguiendo los pasos mencionados anteriormente para la conversión a texto.</p> </td> 
  </tr> 
  <tr> 
   <td>amortiguador </td> 
   <td>fecha </td> 
   <td> <p>El valor se convierte a texto ISO 8601 y, a continuación, a datos binarios siguiendo los pasos mencionados para la conversión a texto.</p> </td> 
  </tr> 
  <tr> 
   <td>amortiguador </td> 
   <td>number </td> 
   <td> <p>El valor se convierte en texto y, a continuación, en datos binarios, siguiendo los pasos mencionados anteriormente para la conversión a texto.</p> </td> 
  </tr> 
  <tr> 
   <td>amortiguador </td> 
   <td>texto </td> 
   <td> <p>El valor se convierte en datos binarios y se codifica según lo esperado. Si no se especifica la codificación esperada, se utilizará la codificación utf8.</p> </td> 
  </tr> 
  <tr> 
   <td>amortiguador </td> 
   <td>otro </td> 
   <td> <p>[!DNL Workfront Fusion] devuelve un error de validación.</p> </td> 
  </tr> 
  <tr> 
   <td>colección </td> 
   <td>colección </td> 
   <td> <p>El valor se entrega sin cambios.</p> </td> 
  </tr> 
  <tr> 
   <td>colección </td> 
   <td>otro </td> 
   <td> <p>[!DNL Workfront Fusion] devuelve un error de validación.</p> </td> 
  </tr> 
  <tr> 
   <td>fecha </td> 
   <td>fecha </td> 
   <td> <p>El valor se entrega sin cambios.</p> </td> 
  </tr> 
  <tr> 
   <td>fecha </td> 
   <td>texto </td> 
   <td> <p>[!DNL Workfront Fusion] intentará convertir el texto en una fecha. Si la conversión falla, devolverá un error de validación. La fecha debe incluir día, mes y año. La fecha puede contener hora y zona horaria. La zona horaria predeterminada depende de la configuración. Ejemplos:</p> <p><code>2016-06-20T17:26:44.356Z</code> </p> <p><code>2016-06-20 19:26:44 GMT+02:00</code> </p> <p><code>2016-06-20 19:26+0200</code> </p> <p><code>2016-06-20 17:26:44</code> </p> <p><code>2016-06-20</code> </p> <p><code>2016/06/20 17:26:44</code> </p> <p><code>2016/06/20 19:26:44+02:00</code> </p> <p><code>2016/06/20 17:26</code> </p> <p><code>2016/06/20 5:26 PM</code> </p> <p><code>2016/06/20</code> </p> <p><code>06/20/2016 17:26:44</code> </p> <p><code>06/20/2016 19:26:44+02:00</code> </p> <p><code>06/20/2016 17:26</code> </p> <p><code>06/20/2016 5:26 PM</code> </p> <p><code>06/20/2016</code> </p> <p><code>20.6.2016 17:26:44</code> </p> <p><code>20.6.2016 19:26:44+02:00</code> </p> <p><code>20.6.2016 17:26</code> </p> <p><code>20.6.2016</code> </p> </td> 
  </tr> 
  <tr> 
   <td>fecha </td> 
   <td>otro </td> 
   <td> <p>[!DNL Workfront Fusion] devuelve un error de validación.</p> </td> 
  </tr> 
  <tr> 
   <td>number </td> 
   <td>number </td> 
   <td> <p>El valor se entrega sin cambios.</p> </td> 
  </tr> 
  <tr> 
   <td>number </td> 
   <td>texto </td> 
   <td> <p>[!DNL Workfront Fusion] intentará convertir el texto en un número. Si la conversión falla, devolverá un error de validación.</p> </td> 
  </tr> 
  <tr> 
   <td>number </td> 
   <td>otro </td> 
   <td> <p>[!DNL Workfront Fusion] devuelve un error de validación.</p> </td> 
  </tr> 
  <tr> 
   <td>texto </td> 
   <td>texto </td> 
   <td> <p>El valor se entrega sin cambios.</p> </td> 
  </tr> 
  <tr> 
   <td>texto </td> 
   <td>matriz </td> 
   <td> <p>Si la matriz dada admite la conversión a texto, el valor se convertirá. Si no es así, [!DNL Workfront Fusion] devolverá un error de validación.</p> </td> 
  </tr> 
  <tr> 
   <td>texto </td> 
   <td>booleano </td> 
   <td> <p>El valor se convierte en texto (true/false).</p> </td> 
  </tr> 
  <tr> 
   <td>texto </td> 
   <td>amortiguador </td> 
   <td> <p>Si se especifica la codificación de texto para los datos binarios, el valor se convertirá en texto. Si no es así, [!DNL Workfront Fusion] devolverá un error de validación.</p> </td> 
  </tr> 
  <tr> 
   <td>texto </td> 
   <td>fecha </td> 
   <td> <p>El valor se convierte a texto ISO 8601.</p> </td> 
  </tr> 
  <tr> 
   <td>texto </td> 
   <td>number </td> 
   <td> <p>El valor se convierte en texto.</p> </td> 
  </tr> 
  <tr> 
   <td>texto </td> 
   <td>otro </td> 
   <td> <p>[!DNL Workfront Fusion] devuelve un error de validación.</p> </td> 
  </tr> 
  <tr> 
   <td>hora </td> 
   <td>hora </td> 
   <td> <p>El valor se entrega sin cambios.</p> </td> 
  </tr> 
  <tr> 
   <td>hora </td> 
   <td>texto </td> 
   <td> <p>[!DNL Workfront Fusion] intentará convertir la hora al formato de horas:minutes:segundos. Si la conversión falla, devolverá un error de validación.</p> </td> 
  </tr> 
  <tr> 
   <td>hora </td> 
   <td>otro </td> 
   <td> <p>[!DNL Workfront Fusion] devuelve un error de validación.</p> </td> 
  </tr> 
 </tbody> 
</table>
