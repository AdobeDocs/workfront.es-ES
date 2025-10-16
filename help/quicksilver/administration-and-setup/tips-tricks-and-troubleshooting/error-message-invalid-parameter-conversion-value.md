---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Mensaje de error: Parámetro no válido: Valor de conversión'
description: 'Recibirá el siguiente mensaje de error al intentar cambiar el formato de un campo personalizado en un formulario personalizado existente: "Parámetro no válido: valor de conversión `&lt;...&gt;`"'
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4f7aac95-4afb-422d-877b-0fa49ef43883
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 88%

---

# Mensaje de error: Parámetro no válido: valor de conversión

## Problema

Recibirá el siguiente mensaje de error al intentar cambiar el formato de un campo personalizado en un formulario personalizado existente: “Parámetro no válido: valor de conversión &#39;&lt;...>&#39;”\
![custom_field_format_invalid_parameter_error.png](assets/custom-field-format-invalid-parameter-error-350x148.png)

## Causa

Este mensaje se genera en el siguiente escenario:

Por ejemplo, supongamos que tiene un campo personalizado con el formato Texto.  Ahora, desea cambiar el Formato del campo personalizado a Divisa. En algún lugar de su instancia de Adobe Workfront, este campo ya está adjunto a un objeto y tiene información ya especificada en él. La información existente en al menos un campo de este tipo ya tiene el formato de texto. Por lo tanto, el formato del campo no se puede cambiar a Divisa.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquete</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licencia</td> 
   <td><p>Estándar</p>
       <p>Plan</p></td>
  </tr>
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a:</p> 
    <ul> 
     <li> <p>Creación de informes, paneles de control y calendarios</p> </li> 
     <li> <p>Creación de filtros, vistas y agrupaciones</p> </li> 
    </ul>
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Solución

Haga lo siguiente:

1. Generar informes de todos los objetos que puedan tener este campo asociado a sus formularios personalizados.\
   Para obtener información sobre cómo generar un informe, consulte [Crear un informe personalizado](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Incluya el campo personalizado que está intentando editar en la vista del informe, para que pueda ver qué objeto tiene este campo rellenado con un valor de texto.
1. Corrija los valores de campo personalizado de los objetos que se muestran en formato de texto y asígneles un valor con el formato divisa; a continuación, intente cambiar de nuevo el campo formato en el formulario personalizado.\
   O\
   Si ya se han rellenado demasiados valores de campo con información con formato de texto, considere la posibilidad de añadir un nuevo campo personalizado al formulario personalizado y aplicarle el formato divisa.
