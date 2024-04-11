---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Módulos JWT
description: El [!DNL Adobe Workfront Fusion] [!UICONTROL JWT] La aplicación proporciona un módulo que crea tokens JWT basados en el algoritmo proporcionado.
author: Becky
feature: Workfront Fusion
source-git-commit: d4f6f5d4919120e37fb94a23ac834a3896019584
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 0%

---

# [!UICONTROL JWT] módulo

El [!DNL Adobe Workfront Fusion] [!UICONTROL JWT] La aplicación proporciona un módulo que crea tokens JWT basados en el algoritmo proporcionado.

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
   <p>Requisito de licencia heredada: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo], [!UICONTROL [!DNL Workfront Fusion] para automatización de trabajo]</p>
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

## Módulo JWT y sus campos

### Generar JWT

Este módulo genera un JWT basado en el algoritmo seleccionado.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Algoritmo]</td> 
   <td> <p>Seleccione el algoritmo con el que desea generar el JWT.</p> <ul>
   <li><b>HS256</b>: HMAC con algoritmo hash SHA-256</li>
   <li><b>HS384</b>: HMAC con algoritmo hash SHA-384</li>
   <li><b>HS512</b>: HMAC con algoritmo hash SHA-512</li>
   <li><b>RS256</b>: RSASSA-PKCS1-v1_5 con algoritmo hash SHA-256</li>
   <li><b>RS384</b>: RSASSA-PKCS1-v1_5 con algoritmo hash SHA-384</li>
   <li><b>RS512</b>: RSASSA-PKCS1-v1_5 con algoritmo hash SHA-512</li>
   <li><b>PS256</b>: RSASSA-PSS que utiliza el algoritmo hash SHA-256 (solo nodo ^6.12.0 O &gt;=8.0.0)</li>
   <li><b>PS384</b>: RSASSA-PSS que utiliza el algoritmo hash SHA-384 (solo nodo ^6.12.0 O &gt;=8.0.0)</li>
   <li><b>PS512</b>: RSASSA-PSS que utiliza el algoritmo hash SHA-512 (solo nodo ^6.12.0 O &gt;=8.0.0)</li>
   <li><b>ES256</b>: ECDSA utilizando la curva P-256 y el algoritmo hash SHA-256</li>
   <li><b>ES384</b>: ECDSA utilizando la curva P-384 y el algoritmo hash SHA-384</li>
   <li><b>ES512</b>: ECDSA utilizando la curva P-521 y el algoritmo hash SHA-512</li>
   </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Carga útil] </td> 
   <td> <p>Para cada elemento de carga útil que desee añadir, haga clic en <b>Añadir elemento</b> e introduzca la clave y el valor del elemento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Opciones] </td> 
   <td> <p>Para cada elemento de opción que desee agregar, haga clic en <b>Añadir elemento</b> e introduzca la clave y el valor del elemento.</p> <p>Las claves disponibles son las siguientes:
   <ul>
   <li><b>algoritmo</b>: (predeterminado: RS256)</li>
   <li><b>expiresIn</b>: se expresa en segundos o en una cadena que describe un lapso de tiempo (por ejemplo, 2 días, 10 horas, 7 días). Un valor numérico se interpreta como un recuento de segundos. Si utiliza una cadena, asegúrese de proporcionar las unidades de tiempo (días, horas, etc.); de lo contrario, se utiliza la unidad de milisegundos de forma predeterminada (120 es igual a 120 ms).</li>
   <li><b>notBefore</b>: se expresa en segundos o en una cadena que describe un lapso de tiempo (por ejemplo, 2 días, 10 horas, 7 días). Un valor numérico se interpreta como un recuento de segundos. Si utiliza una cadena, asegúrese de proporcionar las unidades de tiempo (días, horas, etc.); de lo contrario, se utiliza la unidad de milisegundos de forma predeterminada (120 es igual a 120 ms).
</li>
   <li><b>audiencia</b></li>
   <li><b>emisor</b></li>
   <li><b>jwtid</b></li>
   <li><b>sujeto</b></li>
   <li><b>noTimestamp</b></li>
   <li><b>encabezado</b></li>
   <li><b>keyid</b></li>
   <li><b>mutatePayload</b>: Si <code>true</code>, la función de firma modificará directamente el objeto de carga útil. Esto resulta útil si necesita una referencia sin procesar a la carga útil después de que se le hayan aplicado notificaciones, pero antes de que se haya codificado en un token.</li>
   <li><b>allowInsecureKeySizes</b>: Si <code>true</code>, permite utilizar claves privadas con un módulo inferior a 2048 para RSA.</li>
   <li><b>allowInvalidAsymmetricKeyTypes</b>: Si <code>true</code>, permite claves asimétricas que no coinciden con el algoritmo especificado. Esta opción está diseñada únicamente para la compatibilidad con versiones anteriores y debe evitarse.</li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>

