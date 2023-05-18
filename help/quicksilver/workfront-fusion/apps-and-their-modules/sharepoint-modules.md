---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Módulos de SharePoint
description: En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan SharePoint, así como conectarlos a varias aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion
exl-id: 16d49031-06d2-4c86-bac4-f58cd9b2f1f5
source-git-commit: 83914e54638ffbef2b3ccee12c71b84ca7cc61d2
workflow-type: tm+mt
source-wordcount: '2660'
ht-degree: 0%

---

# [!DNL SharePoint] módulos

En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL SharePoint], así como conectarlo a varias aplicaciones y servicios de terceros.

Si necesita instrucciones para crear un escenario, consulte [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obtener información sobre los módulos, consulte [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Requisitos previos

Para usar [!DNL SharePoint] módulos, debe tener un [!DNL SharePoint] cuenta.

## Connect [!DNL SharePoint] a [!DNL Workfront Fusion] {#connect-sharepoint-to-workfront-fusion}

* [Connect [!DNL SharePoint] a [!DNL Workfront Fusion] usando un [!DNL Microsoft] account](#connect-sharepoint-to-workfront-fusion-using-a-microsoft-account)
* [Connect [!DNL SharePoint] a [!DNL Workfront Fusion] uso de la configuración avanzada](#connect-sharepoint-to-workfront-fusion-using-advanced-settings)

### Connect [!DNL SharePoint] a [!DNL Workfront Fusion] usando un [!DNL Microsoft] account

Puede usar su [!DNL Microsoft] cuenta para crear una conexión con [!DNL SharePoint]. Para obtener instrucciones sobre cómo conectar su [!DNL Sharepoint] cuenta para [!DNL Workfront Fusion], consulte [Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

### Connect [!DNL SharePoint] a [!DNL Workfront Fusion] uso de la configuración avanzada

Para conectar [!DNL SharePoint] a [!DNL Workfront Fusion] sin [!DNL Microsoft] cuenta, necesita un ID de cliente, un Secreto de cliente y un ID de inquilino.

1. Haga clic en **[!UICONTROL Agregar]** cerca de la parte superior del **[!DNL SharePoint]** para abrir el **[!UICONTROL Crear una conexión]** en la ventana

1. (Opcional) Cambiar el valor predeterminado **[!UICONTROL Nombre de la conexión]**.
1. Haga clic en **[!UICONTROL Mostrar configuración avanzada]**.
1. Introduzca la variable [!DNL SharePoint] **[!UICONTROL ID de cliente]** y **[!UICONTROL Secreto del cliente]**.

1. Haga clic en **[!UICONTROL Continuar]**.
1. En la ventana de inicio de sesión que se muestra, introduzca sus credenciales para iniciar sesión en la aplicación si aún no lo ha hecho.
1. (Condicional) Si **[!UICONTROL Permitir]** , haga clic en el botón para conectar la aplicación a [!DNL Workfront Fusion].

## [!DNL SharePoint] módulos y sus campos

Al configurar [!DNL SharePoint] módulos, [!DNL Workfront Fusion] muestra los campos que se enumeran a continuación. Además de estos, se incluyen [!DNL SharePoint] pueden mostrarse los campos, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón de asignación encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Elemento de unidad](#drive-item)
* [Elemento](#item)
* [Lista](#list)
* [Página (Beta)](#page-beta)
* [Sitio](#site)
* [Otro](#other)

### Elemento de unidad

* [Crear un archivo](#create-a-file)
* [Crear una carpeta](#create-a-folder)
* [Obtener un archivo](#get-a-file)
* [Elementos de carpeta de inspección](#watch-folder-items)

#### Obtener cambios

Este módulo devuelve los cambios realizados en SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL SharePoint] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Introducir ID de sitio, unidad y carpeta]</td> 
   <td> <p>Seleccione cómo desea identificar la ubicación de la carpeta en la que desea recuperar los cambios.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Introduzca o asigne la variable <strong>[!UICONTROL ID del sitio]</strong>, <strong>[!UICONTROL List ID]</strong>y <strong>[!UICONTROL Folder ID]</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccione en la lista que sigue]</strong> </p> <p>Seleccione la ubicación donde desea recuperar los cambios. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Token]</td> 
   <td> </td> 
  </tr>  </tbody> 
</table>

#### Crear una carpeta

Este módulo de acción crea una nueva carpeta en SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL SharePoint] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Introducir ID de sitio, unidad y carpeta]</td> 
   <td> <p>Seleccione cómo desea identificar la ubicación de la carpeta que desea crear.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Introduzca o asigne la variable <strong>[!UICONTROL ID del sitio]</strong>, <strong>[!UICONTROL List ID]</strong>y <strong>[!UICONTROL Folder ID]</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccione en la lista que sigue]</strong> </p> <p>Seleccione la ubicación en la que desea crear la carpeta. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder name]</td> 
   <td>Introduzca o asigne un nombre para la nueva carpeta.</td> 
  </tr>
  </tbody> 
</table>

#### Obtener un archivo

Este módulo de acción recupera el archivo SharePoint especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL SharePoint] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Introducir ID de sitio, unidad y carpeta]</td> 
   <td> <p>Seleccione cómo desea identificar la ubicación del archivo que desea obtener.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Introduzca o asigne la variable <strong>[!UICONTROL ID del sitio]</strong>, <strong>[!UICONTROL List ID]</strong>y <strong>[!UICONTROL File ID]</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccione en la lista que sigue]</strong> </p> <p>Seleccione la ubicación del archivo. </p> </li> 
    </ul> </td> 
  </tr> 
</tbody> 
</table>

#### Elementos de carpeta de inspección

Este módulo de déclencheur inicia un escenario cuando se actualiza un elemento en una carpeta seleccionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL SharePoint] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Introducir ID de sitio, unidad y carpeta]</td> 
   <td> <p>Seleccione cómo desea identificar la ubicación del archivo que desea obtener.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Introduzca o asigne la variable <strong>[!UICONTROL ID del sitio]</strong>, <strong>[!UICONTROL List ID]</strong>y <strong>[!UICONTROL folder ID]</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccione en la lista que sigue]</strong> </p> <p>Seleccione la ubicación de la carpeta que desee ver. </p> </li> 
    </ul> </td> 
  </tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td>Introduzca el número máximo de elementos [!DNL Workfront Fusion] debe volver durante un ciclo de ejecución de escenario.</td> 
  <tr>
  </tr>
</tbody> 
</table>

### Elemento

* [[!UICONTROL Copiar elemento]](#copy-an-item)
* [[!UICONTROL Crear un elemento]](#create-an-item)
* [[!UICONTROL Eliminar un elemento]](#delete-an-item)
* [[!UICONTROL Obtener un artículo]](#get-an-item)
* [[!UICONTROL Elementos de lista]](#list-items)
* [[!UICONTROL Mover elemento]](#move-an-item)
* [[!UICONTROL Actualizar un elemento]](#update-an-item)
* [[!UICONTROL Artículos de inspección] (Programado)](#watch-items-scheduled)


#### [!UICONTROL Copiar elemento]

Este módulo de acción copia un elemento existente en una lista de SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL SharePoint] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Especifique los ID de sitio, unidad y carpeta</td> 
   <td> <p>Seleccione cómo desea identificar el sitio y la lista que contienen el elemento que desea copiar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Introduzca o asigne la variable <strong>[!UICONTROL ID del sitio]</strong>, <strong>[!UICONTROL List ID]</strong>y <strong>[!UICONTROL ID del elemento]</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar de la lista que sigue]</strong> </p> <p>En el campo Copiar tipo de elemento , seleccione si va a mover un campo o una carpeta.  Seleccione el sitio que contiene el elemento que desea copiar, luego seleccione la lista y luego seleccione el elemento. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de destino]</td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nuevo nombre]</td> 
   <td>Introduzca o asigne un nombre para la nueva copia del artículo. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear un elemento]

Este módulo de acción crea un nuevo elemento en una lista de SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL SharePoint] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Crear un elemento]</td> 
   <td> <p>Seleccione cómo desea identificar el sitio y la lista donde desea crear un elemento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Introduzca o asigne la variable <strong>[!UICONTROL ID del sitio]</strong> y <strong>[!UICONTROL List ID]</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar de la lista]</strong> </p> <p>Seleccione el sitio que contiene la lista donde desea crear un elemento y, a continuación, seleccione la lista. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields]</td> 
   <td>Para cada campo que desee configurar para el nuevo elemento, introduzca la clave del campo (identifica el campo) y el valor que desea que tenga el nuevo elemento para ese campo.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar un elemento]

Este módulo de acción elimina un elemento existente de una lista de SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL SharePoint] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Actualizar un elemento]</td> 
   <td> <p>Seleccione cómo desea identificar el sitio y la lista que contienen el elemento que desea eliminar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Introduzca o asigne la variable <strong>[!UICONTROL ID del sitio]</strong>, <strong>[!UICONTROL List ID]</strong>y <strong>[!UICONTROL ID del elemento]</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar de la lista]</strong> </p> <p>Seleccione el sitio que contiene el elemento que desea eliminar, luego seleccione la lista y luego seleccione el elemento. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener un artículo]

Este módulo de acción devuelve los datos de un elemento especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL SharePoint] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obtener un elemento]</td> 
   <td> <p>Seleccione cómo desea identificar el sitio y la lista que contienen el elemento que desea obtener.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Introduzca o asigne la variable <strong>[!UICONTROL ID del sitio]</strong>, <strong>[!UICONTROL List ID]</strong>y <strong>[!UICONTROL ID del elemento]</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar de la lista]</strong> </p> <p>Seleccione el sitio que contiene la lista desde la que desea recuperar un elemento, luego seleccione la lista y luego seleccione el elemento. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elementos de lista]

Este módulo de acción recupera una lista de todos los elementos de una lista especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL SharePoint] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Lista Elementos]</td> 
   <td> <p>Seleccione cómo desea identificar la lista de la que desea recuperar los elementos.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Introduzca o asigne la variable <strong>[!UICONTROL ID del sitio]</strong> y <strong>[!UICONTROL List ID]</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar de la lista]</strong> </p> <p>Seleccione el sitio que contiene la lista de la que desea recuperar elementos y, a continuación, seleccione la lista. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de elementos que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mover un elemento]

Este módulo de acción copia un elemento existente en una lista de SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL SharePoint] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Especifique los ID de sitio, unidad y carpeta</td> 
   <td> <p>Seleccione cómo desea identificar el sitio y la lista que contienen el elemento que desea mover.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Introduzca o asigne la variable <strong>[!UICONTROL ID del sitio]</strong>, <strong>[!UICONTROL List ID]</strong>y <strong>[!UICONTROL ID del elemento]</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar de la lista que sigue]</strong> </p> <p>En el campo Copiar tipo de elemento , seleccione si va a mover un campo o una carpeta. Seleccione el sitio que contiene el elemento que desea copiar, luego seleccione la lista y luego seleccione el elemento. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de destino]</td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nuevo nombre]</td> 
   <td>Introduzca o asigne un nombre para el elemento movido. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actualizar un elemento]

Este módulo de acción actualiza un elemento existente en una lista de SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL SharePoint] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Actualizar un elemento]</td> 
   <td> <p>Seleccione cómo desea identificar el sitio y la lista que contienen el elemento que desea actualizar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Introduzca o asigne la variable <strong>[!UICONTROL ID del sitio]</strong>, <strong>[!UICONTROL List ID]</strong>y <strong>[!UICONTROL ID del elemento]</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar de la lista]</strong> </p> <p>Seleccione el sitio que contiene el elemento que desea actualizar, luego seleccione la lista y luego seleccione el elemento. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields]</td> 
   <td>Para cada campo que desee actualizar para el nuevo elemento, introduzca la clave del campo (identifica el campo) y el nuevo valor que desea que tenga el elemento para ese campo.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Artículos de inspección] (Programado)

Este módulo de déclencheur inicia un escenario cuando se crea o modifica un elemento.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL SharePoint] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Listas de inspección]</td> 
   <td>Seleccione si desea ver las listas por tiempo de creación (elementos nuevos) o por tiempo de modificación (elementos actualizados).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrar en el sitio y en el ID de lista]</td> 
   <td> <p>Seleccione cómo desea identificar el sitio y la lista que desea ver.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Introduzca o asigne la variable <strong>[!UICONTROL ID del sitio]</strong> y <strong>[!UICONTROL List ID]</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccione en la lista que sigue]</strong> </p> <p>Seleccione el sitio que desea ver y, a continuación, seleccione la lista. Estos desplegables solo recuperan los sitios seguidos.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de elementos que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Lista

* [[!UICONTROL Crear una lista]](#create-a-list)
* [[!UICONTROL Obtener una lista]](#get-a-list)
* [[!UICONTROL Listas]](#list-lists)
* [[!UICONTROL Listas de inspección]](#watch-lists)

#### [!UICONTROL Crear una lista]

Este módulo de acción crea una nueva lista en SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL SharePoint] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Introducir un ID de sitio]</td> 
   <td> <p>Seleccione cómo desea identificar el sitio y la lista donde desea crear una lista.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Introduzca o asigne la variable <strong>[!UICONTROL ID del sitio]</strong> donde desea crear una lista.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar de la lista]</strong> </p> <p>Seleccione el sitio en el que desea crear una lista. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre para mostrar]</td> 
   <td>Introduzca o asigne un nombre para la nueva lista.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descripción]</td> 
   <td>Introduzca o asigne una descripción para la nueva lista.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Agregar columnas]</td> 
   <td>Para cada columna que desee configurar para la nueva lista, introduzca un <strong>[!UICONTROL Name]</strong> para el campo y seleccione la <strong>[!UICONTROL Type]</strong> del valor que desea que tenga la nueva columna.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener una lista]

Este módulo de acción devuelve los datos de una lista especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL SharePoint] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obtener una lista]</td> 
   <td> <p>Seleccione cómo desea identificar el sitio y la lista que contienen el elemento que desea obtener.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Introduzca o asigne la variable <strong>[!UICONTROL ID del sitio]</strong> y <strong>ID de lista</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar de la lista]</strong> </p> <p>Seleccione el sitio que contiene la lista que desea recuperar y, a continuación, seleccione la lista. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listas]

Este módulo de acción recupera una lista de todos los elementos de una lista especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL SharePoint] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Lista Listas]</td> 
   <td> <p>Seleccione cómo desea identificar el sitio desde el que desea recuperar las listas.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Introduzca o asigne la variable <strong>[!UICONTROL ID del sitio]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar de la lista]</strong> </p> <p>Seleccione el sitio que contiene las listas que desea recuperar. La lista desplegable recupera solo los sitios que sigue.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de listas que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listas de inspección]

Este módulo de déclencheur inicia un escenario cuando se crea o modifica una lista.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL SharePoint] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Listas de inspección]</td> 
   <td>Seleccione si desea ver las listas por tiempo de creación (elementos nuevos) o por tiempo de modificación (elementos actualizados).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrar en el sitio y en el ID de lista]</td> 
   <td> <p>Seleccione cómo desea identificar el sitio y la lista que desea ver.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Introduzca o asigne la variable <strong>[!UICONTROL ID del sitio]</strong> donde se encuentra la lista que desea ver.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccione en la lista que sigue]</strong> </p> <p>Seleccione el sitio que desee ver. La lista desplegable solo recupera el sitio que sigue.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de listas que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Página (Beta)

>[!NOTE]
>
>API en el `beta` versión en [!DNL Microsoft Graph] están sujetas a cambios. No se admite el uso de estas API en aplicaciones de producción.

#### [!UICONTROL Obtener una página]

Este módulo de acción devuelve los datos de una página especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL SharePoint] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obtener una página]</td> 
   <td> <p>Seleccione cómo desea identificar la página que desea recuperar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Introduzca o asigne la variable <strong>[!UICONTROL ID del sitio]</strong>y <strong>[!UICONTROL ID de página]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar de la lista]</strong> </p> <p>Seleccione el sitio que contiene la página que desea recuperar y, a continuación, seleccione la página.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Sitio

* [[!UICONTROL Obtener un sitio]](#get-a-site)
* [[!UICONTROL Buscar sitios]](#search-sites)

#### [!UICONTROL Obtener un sitio]

Este módulo de acción devuelve los datos de un sitio especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL SharePoint] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obtener un sitio]</td> 
   <td> <p>Seleccione cómo desea identificar la página que desea recuperar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Introduzca o asigne la variable <strong>[!UICONTROL ID del sitio]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar de la lista]</strong> </p> <p>Seleccione el sitio que desee recuperar.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Buscar sitios]

Este módulo de acción busca sitios según el parámetro que especifique.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL SharePoint] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Palabra clave del nombre para mostrar]</td> 
   <td> <p>Escriba o asigne el término de búsqueda que desee buscar en los sitios.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de sitios que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Otro

#### [!UICONTROL Realizar una llamada de API]

Este módulo le permite realizar una llamada API personalizada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL SharePoint] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Especifique una ruta relativa a <code>https://graph.microsoft.com</code>. Ejemplo:<code> /beta/sites</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Método]</p> </td> 
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada a la API. Para obtener más información, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de un objeto JSON estándar. Por ejemplo, <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] añade los encabezados de autorización por usted.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadena de consulta]</td> 
   <td> <p> Añada la consulta para la llamada de API en forma de objeto JSON estándar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td>Seleccione el tipo de datos que desea enviar en su llamada de API.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Al utilizar afirmaciones condicionales como <code>if</code> en su JSON, ponga las comillas fuera de la afirmación condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### Ver eventos

Este módulo de déclencheur instantáneo inicia un escenario cuando se agrega, actualiza o elimina un elemento en SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
  <!--
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL SharePoint] account to [!DNL Workfront Fusion], see <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  -->
  <tr> 
   <td role="rowheader">[!UICONTROL Weblock]</td> 
   <td> <p>Seleccione un vínculo web existente o haga clic en Add para crear un nuevo vínculo web.</p> 
   </td> 
  </tr> 
 </tbody> 
</table>

