---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Solución de problemas de la promoción del entorno
description: Solucione problemas comunes con la promoción del entorno.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 830dd573-d954-4ba2-a1d3-d1645b3fbac8
TQID: https://experienceleague.adobe.com/N6spdHNxoRMwUjQY6HrHPm11d7kZaYHMbDGAkeqbyvY
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 330
ht-degree: 44%

---

# Solución de problemas de la promoción del entorno

Este artículo describe cómo solucionar problemas de promoción del entorno.

## Problema: El paquete de promoción del entorno se está demorando o falla

Si el paquete de promoción del entorno se bloquea o falla, pruebe lo siguiente:

* Si la instalación de un paquete se detiene después de 10-15 minutos, o si la instalación de un paquete falla, vuelva a montar el paquete existente o cree uno nuevo.

* Si falla la instalación de un paquete, puede haber un problema con uno o más objetos. Compruebe los mensajes de error que identifican el objeto y pueden ayudar a identificar el problema. Una vez solucionado el problema con el objeto, vuelva a montar el paquete y vuelva a intentar la instalación.

* Si sigue teniendo problemas con una instalación, intente replicar la instalación en un entorno de destino diferente. Manténgase lo más cerca posible de la instalación original, incluidos los objetos y las acciones de instalación seleccionados.

* Se recomienda comprobar siempre el contenido del paquete después de montarlo para confirmar que contenga los objetos esperados.


## Problema: El formulario personalizado no se promociona

Esto puede ocurrir porque el formulario personalizado incluye un campo calculado. Si un campo calculado hace referencia a un campo que no está referenciado en un formulario personalizado, un paquete que incluye este formulario no se promociona y el usuario puede ver el siguiente mensaje:

&quot;Los campos siguientes no son válidos: Expresión personalizada no válida Expresión no válida: Expresión personalizada no válida.&quot;

Este problema puede surgir al hacer referencia a un campo existente que no está adjunto a ningún formulario personalizado en el entorno de destino o con un campo recién creado.

Para resolver este problema, realice una de las siguientes acciones:

* Cree un paquete con un formulario personalizado de tipo de proyecto que incluya el campo al que se hace referencia. Después de promocionar este paquete en el entorno de destino, promocione el paquete deseado originalmente que contiene el campo calculado.
* Cree manualmente el campo al que se hace referencia en el entorno de destino y asócielo a un formulario personalizado de tipo de proyecto. Una vez hecho esto, se reconoce el campo y puede promocionar el paquete sin encontrar el error.
