---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Mensaje de error: Parámetro no válido: valor de conversión"
description: "Recibirá el siguiente mensaje de error al intentar cambiar el formato de un campo personalizado en un formulario personalizado existente: 'Parámetro no válido: conversion value `&lt;...&gt;`'"
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7aac95-4afb-422d-877b-0fa49ef43883
source-git-commit: 62d1b9563d83bd82b569e143f69e379e2f4ffbc2
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# Mensaje de error: Parámetro no válido: valor de conversión

## Problema

Recibirá el siguiente mensaje de error al intentar cambiar el formato de un campo personalizado en un formulario personalizado existente: &quot;Parámetro no válido: valor de conversión &quot;&lt;...>&quot;&quot;\
![custom_field_format_invalid_parameter_error.png](assets/custom-field-format-invalid-parameter-error-350x148.png)

## Causa

Este mensaje se produce en el siguiente escenario:

Por ejemplo, supongamos que tiene un campo personalizado con el formato Texto.  Ahora, desea cambiar el Formato del campo personalizado a Moneda. En algún lugar de la instancia de Adobe Workfront, este campo ya está adjunto a un objeto y tiene información ya especificada en él. La información existente en al menos un campo de este tipo ya tiene el formato Texto. Por lo tanto, el formato del campo no se puede cambiar a Currency.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><a href="https://www.workfront.com/plans" target="_blank">plan Workfront</a>*</p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Resumen de licencias</a>*</p> </td> 
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Nivel de acceso*</strong> </td> 
   <td> <p>Editar acceso a:</p> 
    <ul> 
     <li> <p>Creación de informes, tableros y calendarios</p> </li> 
     <li> <p>Creación de filtros, vistas y agrupaciones</p> </li> 
    </ul> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, vea <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Solución

Haga lo siguiente:

1. Generar informes de todos los objetos que puedan tener este campo asociado a su Forms personalizado.\
   Para obtener información sobre cómo generar un informe, consulte [Crear un informe personalizado](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Incluya el campo personalizado que está intentando editar en la vista del informe, para que pueda ver qué objeto tiene este campo rellenado con un valor de texto.
1. Corrija los valores de Campo personalizado de los objetos que se muestran en formato de texto y asígneles un valor con el formato Moneda; a continuación, intente cambiar de nuevo el campo Formato en el Formulario personalizado.\
   O\
   Si ya se han rellenado demasiados valores de campo con información con formato de texto, considere la posibilidad de agregar un nuevo campo personalizado al formulario personalizado y aplicarle el formato Moneda.
