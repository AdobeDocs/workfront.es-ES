---
content-type: api
navigation-topic: api-navigation-topic
title: Caracteres de escape en las respuestas de API
description: Caracteres de escape en las respuestas de API
author: Becky
feature: Workfront API
exl-id: 1477b98e-1cdc-4661-b3ee-0b6ab1e8c3ee
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 8%

---

# Caracteres de escape en las respuestas de API

La sintaxis de algunas respuestas de API puede contener el carácter de escape, `\` (barra invertida). Un carácter de escape indica que el carácter o la cadena de caracteres que siguen inmediatamente al carácter de escape tienen un valor especial. Por ejemplo, `\t` indica al dispositivo de lectura que `t` debe interpretarse como `tab` y no como la letra &quot;t&quot;. Una cadena de uno o más caracteres que siguen a la barra invertida se denomina secuencia de escape.

Las secuencias de escape hexadecimales requieren el uso de dígitos hexadecimales válidos. La tabla siguiente muestra las secuencias de escape codificadas en las respuestas de la API de Adobe Workfront:

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
   <td> <p>\u000<em>x</em></p> <p>Donde, <em>x</em> es el código hexadecimal para los números 0 a 7</p> </td> 
   <td>0-7</td> 
   <td>Caracteres Unicode representados en los puntos de código de 0 a 7</td> 
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
   <td>Ficha Vertical</td> 
  </tr> 
  <tr> 
   <td>\f</td> 
   <td>12</td> 
   <td>Fuente de formulario</td> 
  </tr> 
  <tr> 
   <td>\r</td> 
   <td>13</td> 
   <td>Retorno de carro</td> 
  </tr> 
  <tr> 
   <td> <p>\u00<em>xx</em></p> <p><em>Donde, xx es el código hexadecimal para los números 14 a 31</em> </p> </td> 
   <td>14 - 31</td> 
   <td>Caracteres Unicode representados por puntos de código 14 a 31</td> 
  </tr> 
  <tr> 
   <td> <p>\/</p> </td> 
   <td>47</td> 
   <td>/ (Barra oblicua)</td> 
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
   <td> <p>\u<em>xxxx</em></p> <p>Donde, <em>xxxx</em> es el código hexadecimal para cualquier número superior a 127</p> </td> 
   <td>128+</td> 
   <td>Caracteres Unicode para cualquier punto de código superior a 127</td> 
  </tr> 
 </tbody> 
</table>
