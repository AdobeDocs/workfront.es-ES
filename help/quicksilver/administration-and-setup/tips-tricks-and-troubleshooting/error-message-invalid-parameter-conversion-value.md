---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Mensaje de error: Parámetro no válido: valor de conversión'
description: "Recibe el siguiente mensaje de error al intentar cambiar el formato de un campo personalizado en un formulario personalizado existente: 'Parámetro no válido: valor de conversión `&lt;..&gt;`'"
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7aac95-4afb-422d-877b-0fa49ef43883
source-git-commit: 5469598d57fec1a744ddb44cf2accb94e1f70941
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 1%

---

# Mensaje de error: Parámetro no válido: valor de conversión

## Problema

Recibe el siguiente mensaje de error cuando intenta cambiar el formato de un campo personalizado en un formulario personalizado existente: &quot;Parámetro no válido: valor de conversión &quot;&lt;...>&quot;\
![custom_field_format_invalid_parameter_error.png](assets/custom-field-format-invalid-parameter-error-350x148.png)

## Causa

Este mensaje se produce en el siguiente escenario:

Por ejemplo, tiene un campo personalizado con formato de texto.  Ahora, desea cambiar el Formato del campo personalizado a Moneda. En algún lugar de la instancia de Adobe Workfront, este campo ya está adjunto a un objeto y tiene información especificada en él. La información existente en al menos uno de estos campos ya tiene formato de Texto. Por lo tanto, el Formato del campo no se puede cambiar a Moneda.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><a href="https://www.workfront.com/plans" target="_blank">plan de Workfront</a>*</p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Información general sobre licencias heredadas</a>*</p> </td> 
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Nivel de acceso*</strong> </td> 
   <td> <p>Editar acceso a:</p> 
    <ul> 
     <li> <p>Creación de informes, tableros y calendarios</p> </li> 
     <li> <p>Crear filtros, vistas y grupos</p> </li> 
    </ul> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Solución

Haga lo siguiente:

1. Genere informes para todos los objetos que puedan tener este campo asociado con su Forms personalizado.\
   Para obtener información sobre cómo crear un informe, consulte [Crear un informe personalizado](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Incluya el campo personalizado que está intentando editar en la vista del informe, para que pueda ver qué objeto tiene este campo rellenado con un valor de texto.
1. Corrija los valores de Campo personalizado de los objetos que aparecen en formato de texto y asígneles un valor con formato de Moneda; a continuación, intente cambiar de nuevo el campo Formato del formulario personalizado.\
   O\
   Si ya tiene demasiados valores de campo rellenados con información con formato de texto, considere la posibilidad de agregar un nuevo campo personalizado al formulario personalizado y aplicarle el formato Moneda.
