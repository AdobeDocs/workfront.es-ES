---
content-type: api
navigation-topic: api-navigation-topic
title: Caracteres escapados en las respuestas de API
description: Caracteres escapados en las respuestas de API
author: Becky
feature: Workfront API
role: Developer
exl-id: 1477b98e-1cdc-4661-b3ee-0b6ab1e8c3ee
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 5%

---

# Caracteres escapados en las respuestas de API

La sintaxis de algunas respuestas API puede contener el carácter de escape `\` (barra invertida). Un carácter de escape indica que el carácter o cadena de caracteres que siguen inmediatamente al carácter de escape tiene un valor especial. Por ejemplo, `\t` indica al dispositivo de lectura que `t` debe interpretarse como `tab` y no como la letra &quot;t&quot;. Una cadena de uno o más caracteres después de la barra invertida se denomina secuencia de escape.

Las secuencias de escape hexadecimales requieren el uso de dígitos hexadecimales válidos. En la tabla siguiente se enumeran las secuencias de escape codificadas en las respuestas de la API de Adobe Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Secuencia de escape</strong> </th> 
   <th><strong>Carácter Unicode</strong> </th> 
   <th><strong>Representa</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>\u000<em>x</em></p> <p>Donde, <em>x</em> es el código hexadecimal de los números del 0 al 7</p> </td> 
   <td>0-7</td> 
   <td>Caracteres Unicode representados por los puntos de código 0 a 7</td> 
  </tr> 
  <tr> 
   <td>\b</td> 
   <td>8</td> 
   <td>Retroceder</td> 
  </tr> 
  <tr> 
   <td>\t</td> 
   <td>9</td> 
   <td>Ficha</td> 
  </tr> 
  <tr> 
   <td>\n</td> 
   <td>10</td> 
   <td>Nueva línea</td> 
  </tr> 
  <tr> 
   <td>\u000b</td> 
   <td>11</td> 
   <td>Pestaña vertical</td> 
  </tr> 
  <tr> 
   <td>\f</td> 
   <td>12</td> 
   <td>Avance de página</td> 
  </tr> 
  <tr> 
   <td>\r</td> 
   <td>13</td> 
   <td>Retorno de carro</td> 
  </tr> 
  <tr> 
   <td> <p>\u00<em>xx</em></p> <p><em>Donde, xx es el código hexadecimal de  números del 14 al 31</em> </p> </td> 
   <td>De 14 a 31</td> 
   <td>Caracteres Unicode representados por los puntos de código 14 a 31</td> 
  </tr> 
  <tr> 
   <td> <p>\/</p> </td> 
   <td>47</td> 
   <td>/ (Barra diagonal)</td> 
  </tr> 
  <tr> 
   <td> <p>\u003c</p> </td> 
   <td>60</td> 
   <td>&lt; (Menor que)</td> 
  </tr> 
  <tr> 
   <td> <p>\\</p> </td> 
   <td>92</td> 
   <td>\ (Barra invertida)</td> 
  </tr> 
  <tr> 
   <td> <p>\u<em>xxxx</em></p> <p>Donde, <em>xxxx</em> es el código hexadecimal de cualquier número superior a 127</p> </td> 
   <td>128+</td> 
   <td>Caracteres Unicode para cualquier punto de código superior a 127</td> 
  </tr> 
 </tbody> 
</table>
