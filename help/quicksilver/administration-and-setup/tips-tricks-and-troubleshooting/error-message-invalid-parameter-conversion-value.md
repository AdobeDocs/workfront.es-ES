---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Mensaje de error: Parámetro no válido: Valor de conversión"
description: "Recibirá el siguiente mensaje de error al intentar cambiar el formato de un campo personalizado en un formulario personalizado existente: 'Parámetro no válido: conversion value `&lt;...&gt;`'"
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4f7aac95-4afb-422d-877b-0fa49ef43883
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Mensaje de error: Parámetro no válido: valor de conversión

## Problema

Recibirá el siguiente mensaje de error al intentar cambiar el formato de un campo personalizado en un formulario personalizado existente: &quot;Parámetro no válido: valor de conversión &quot;&lt;...>&quot;&quot;\
![custom_field_format_invalid_parameter_error.png](assets/custom-field-format-invalid-parameter-error-350x148.png)

## Causa

Este mensaje se produce en el siguiente escenario:

Por ejemplo, supongamos que tiene un campo personalizado con el formato Texto.  Ahora, desea cambiar el Formato del campo personalizado a Moneda. En algún lugar de la instancia de Adobe Workfront, este campo ya está adjunto a un objeto y tiene información ya especificada en él. La información existente en al menos un campo de este tipo ya tiene el formato Texto. Por lo tanto, el formato del campo no se puede cambiar a Currency.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td>
   <p>Nuevo: estándar</p>
   <p>o</p>
   <p>Actual: plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a:</p> 
    <ul> 
     <li> <p>Creación de informes, tableros y calendarios</p> </li> 
     <li> <p>Creación de filtros, vistas y agrupaciones</p> </li> 
    </ul>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Solución

Haga lo siguiente:

1. Generar informes de todos los objetos que puedan tener este campo asociado a su Forms personalizado.\
   Para obtener información sobre cómo generar un informe, consulte [Crear un informe personalizado](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Incluya el campo personalizado que está intentando editar en la vista del informe, para que pueda ver qué objeto tiene este campo rellenado con un valor de texto.
1. Corrija los valores de Campo personalizado de los objetos que se muestran en formato de texto y asígneles un valor con el formato Moneda; a continuación, intente cambiar de nuevo el campo Formato en el Formulario personalizado.\
   O\
   Si ya se han rellenado demasiados valores de campo con información con formato de texto, considere la posibilidad de agregar un nuevo campo personalizado al formulario personalizado y aplicarle el formato Moneda.
