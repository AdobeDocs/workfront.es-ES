---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Tipos de datos de elementos en [!DNL Adobe Workfront Fusion]
description: Su [!DNL Adobe Workfront Fusion] los escenarios pueden contener los tipos de elementos enumerados a continuación en un paquete.
author: Becky
feature: Workfront Fusion
exl-id: 36c25a86-0d05-4871-a6a6-4fd54cfcc4b1
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 0%

---

# Tipos de datos de elementos en [!DNL Adobe Workfront Fusion]

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

## Tipos de datos de elementos

Puede contener los tipos de elementos enumerados a continuación en un paquete.

Para obtener información sobre qué tipos de elementos [!DNL Workfront Fusion] permite la conversión entre sí, consulte [Coerción de tipo en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Texto</p> </td> 
   <td> <p>El tipo de elemento más común. Para algunos elementos de texto, [!DNL Adobe Workfront Fusion] comprueba si se cumple la longitud máxima o mínima permitida o si el elemento realiza una validación de formato (correo electrónico, URL o nombre de archivo).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Número</p> </td> 
   <td> <p>Para algunos elementos numéricos, [!DNL Workfront Fusion] puede validar la entrada para un rango especificado (el valor mínimo o máximo permitido).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Booleano (Sí/No)</p> </td> 
   <td> <p>Este tipo se utiliza para elementos con solo dos valores posibles: true o false. </p> <p>Al configurar los módulos, el tipo booleano puede aparecer en dos formas diferentes:</p> 
    <ul> 
     <li> <p>La casilla de verificación obligatoria se muestra en caso de que el campo sea obligatorio y deba rellenarse.</p> <p> <img src="assets/boolean-checkbox-350x158.jpg" style="width: 350;height: 158;"> </p> </li> 
     <li> <p>Los campos opcionales que se pueden dejar en blanco se muestran como un cuadro de selección, lo que permite seleccionar entre tres valores: <code>Yes</code>, <code>No</code>y <code>Not defined</code> (predeterminado).</p> <p> <img src="assets/boolean-convert-file-350x129.jpg" style="width: 350;height: 129;"> </p> </li> 
    </ul> <p>Puede hacer clic en <strong>[!UICONTROL Map]</strong> si necesita asignar el valor a un elemento de otro módulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Fecha</p> </td> 
   <td> <p>Las fechas se introducen en el formato de fecha ISO 8601, por ejemplo, <code>2015-09-18T11:58Z</code>. Puede cambiar la zona horaria en la configuración del perfil, tal como se explica en <a href="../../workfront-fusion/workfront-fusion-basics/change-profile-settings.md" class="MCXref xref">Cambiar la configuración de perfil en [!DNL Adobe Workfront Fusion]</a>. </p> <p>Si hace clic en un campo que requiere una fecha, aparece un calendario emergente en la configuración del módulo. No se requiere el tiempo para algunos elementos.</p> <p>Los valores de los elementos Fecha tienen formato mediante la zona horaria local y web seleccionada en el perfil. Puede mostrar la versión ISO 8601 del valor de un elemento de fecha pasando el ratón sobre él.</p> <p>Nota: Si el valor ISO no se muestra, es probable que el elemento sea texto, no una fecha.</p> <p>La hora se introduce en la variable <code>hours:minutes:seconds</code> formato, por ejemplo,<code>14:03:52</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Búfer (datos binarios)</p> </td> 
   <td> <p>El contenido del archivo se suele enviar como contenido de tipo búfer (contenido de imagen, archivo de vídeo, etc.). En algunos casos, los datos de texto se incluyen en este tipo (por ejemplo, un archivo de texto). [!DNL Workfront Fusion] puede convertir automáticamente datos de texto en código binario a datos de texto y texto en código binario. Para obtener más información, consulte <a href="../../workfront-fusion/mapping/about-mapping-files.md" class="MCXref xref">Acerca de la asignación de archivos en [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Colección</p> </td> 
   <td> <p>Una colección es un elemento que consta de varios subelementos. El elemento Remitente de un mensaje de correo electrónico es un ejemplo de una colección: contiene el nombre del remitente (tipo de texto) y la dirección de correo electrónico del remitente (tipo de texto).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Seleccionar (menú)</p> </td> 
   <td> <p>Cuando configure los ajustes del módulo como se describe en <a href="../../workfront-fusion/modules/configure-a-modules-settings.md" class="MCXref xref">Configure las opciones de un módulo en [!DNL Adobe Workfront Fusion]</a>, puede seleccionar entre varios elementos del mismo tipo. Un ejemplo es el menú de selección de carpetas en la configuración de [!DNL Dropbox] módulos. </p> <p>Al configurar los módulos, el menú de selección puede aparecer en dos formularios:</p> <p> <p>Si es posible realizar varias selecciones, aparecen varios elementos con casillas de verificación.</p> <p> <img src="assets/image-kb-type-list-multi-350x232.jpg" style="width: 350;height: 232;"> </p> </p> <p>Si solo es posible una opción, aparece un menú desplegable.</p> <p> <img src="assets/select-menu-dropdown-350x130.jpg" style="width: 350;height: 130;"> </p> <p>Si necesita asignar un elemento de otro módulo, use el <strong>Mapa</strong> botón. Este botón abre un campo de texto en lugar del menú de selección. Para obtener más información, consulte <a href="../../workfront-fusion/mapping/map-information-between-modules.md" class="MCXref xref">Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Matriz</p> </td> 
   <td> <p>Puede utilizar el tipo de matriz para trabajar con varios valores del mismo tipo, incluidas colecciones. Un ejemplo son los módulos [!UICONTROL Email]: devuelven una matriz de archivos adjuntos y cada uno de ellos contiene nombre, contenido, tamaño, etc. Para obtener más información, consulte <a href="../../workfront-fusion/mapping/map-an-array.md" class="MCXref xref">Asignación de una matriz en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Validación</p> </td> 
   <td> <p>[!DNL Workfront Fusion] puede realizar la validación en cada tipo de elemento. Si un elemento no pasa la validación, el módulo detendrá el procesamiento debido a un error de datos. Para obtener más información, consulte <a href="../../workfront-fusion/errors/error-processing.md" class="MCXref xref">Error de procesamiento en [!DNL Adobe Workfront Fusion]</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
