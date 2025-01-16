---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos SharePoint
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 16d49031-06d2-4c86-bac4-f58cd9b2f1f5
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '2929'
ht-degree: 95%

---

# Módulos de [!DNL SharePoint]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Módulos SharePoint](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/sharepoint-modules.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

En un escenario de [!DNL Adobe Workfront Fusion], puede automatizar los flujos de trabajo que utilizan [!DNL SharePoint], así como conectarlo a varias aplicaciones y servicios de terceros.

Si necesita instrucciones para crear un escenario, consulte [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obtener información acerca de los módulos, consulte [Módulos de  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Requisitos de acceso

Para utilizar la funcionalidad de este artículo debe tener el siguiente acceso:

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
   <td>
   <p>Requisito de licencia actual: no se requiere ninguna licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Producto</td> 
   <td>
   <p>Requisito de producto actual: si tiene el plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], su organización debe adquirir [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en el plan [!DNL Workfront] de [!UICONTROL Ultimate].</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] y [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Requisitos previos

Para usar módulos [!DNL SharePoint], debe tener una cuenta de [!DNL SharePoint].

## Información de API de SharePoint

El conector de SharePoint utiliza lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL básica</td> 
   <td> https://graph.microsoft.com/v1.0</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Versión de API</td> 
   <td> Versión 1.0 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Etiqueta de API</td> 
   <td>Versión 1.14.2</td> 
  </tr>
 </tbody> 
 </table>

## Conectar [!DNL SharePoint] a [!DNL Workfront Fusion] {#connect-sharepoint-to-workfront-fusion}

* [Conectar [!DNL SharePoint] a [!DNL Workfront Fusion] mediante una cuenta de [!DNL Microsoft] ](#connect-sharepoint-to-workfront-fusion-using-a-microsoft-account)
* [Conectar [!DNL SharePoint] a [!DNL Workfront Fusion] mediante ajustes avanzados](#connect-sharepoint-to-workfront-fusion-using-advanced-settings)

### Conectar [!DNL SharePoint] a [!DNL Workfront Fusion] mediante una cuenta de [!DNL Microsoft]

Puede usar su cuenta de [!DNL Microsoft] para crear una conexión con [!DNL SharePoint]. Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL Sharepoint] a [!DNL Workfront Fusion], consulte [Crear una conexión con [!DNL Adobe Workfront Fusion] : instrucciones básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

### Conectar [!DNL SharePoint] a [!DNL Workfront Fusion] mediante ajustes avanzados

Para conectar [!DNL SharePoint] con [!DNL Workfront Fusion] sin una cuenta de [!DNL Microsoft], necesita un ID de cliente, un secreto de cliente y un identificador de inquilino.

1. Haga clic en **[!UICONTROL Añadir]** cerca de la parte superior del cuadro **[!DNL SharePoint]** para abrir el cuadro **[!UICONTROL Crear una conexión]**.

1. (Opcional) Cambie el **[!UICONTROL Nombre de conexión]** predeterminado.
1. Haga clic en **[!UICONTROL Mostrar ajustes avanzados]**.
1. Escriba el **[!UICONTROL ID de cliente]** y **[!UICONTROL Secreto de cliente]** de [!DNL SharePoint].

1. Haga clic en **[!UICONTROL Continuar]**.
1. En la ventana de inicio de sesión que aparece, introduzca sus credenciales para iniciar sesión en la aplicación si aún no lo ha hecho.
1. (Condicional) Si aparece un botón **[!UICONTROL Permitir]**, haga clic en el botón para conectar la aplicación a [!DNL Workfront Fusion].

## Módulos de [!DNL SharePoint] y sus campos

Al configurar módulos de [!DNL SharePoint], [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL SharePoint] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. El título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Elemento de Drive](#drive-item)
* [Elemento](#item)
* [Lista](#list)
* [Página (Beta)](#page-beta)
* [Sitio](#site)
* [Otro](#other)

### Elemento de Drive

* [Crear un archivo](#create-a-file)
* [Crear una carpeta](#create-a-folder)
* [Obtener un archivo](#get-a-file)
* [Ver elementos de la carpeta](#watch-folder-items)

#### Obtener cambios

Este módulo devuelve los cambios realizados en SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter Site, Drive, and Folder IDs]</td> 
   <td> <p>Seleccione cómo desea identificar la ubicación de la carpeta en la que desea recuperar los cambios.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Escriba o asigne el <strong>[!UICONTROL Site ID]</strong>, <strong>[!UICONTROL List ID]</strong> e <strong>[!UICONTROL Folder ID]</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list that you follow]</strong> </p> <p>Seleccione la ubicación donde desea recuperar los cambios. </p> </li> 
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
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter Site, Drive, and Folder IDs]</td> 
   <td> <p>Seleccione cómo identificar la ubicación de la carpeta que desea crear.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Escriba o asigne el <strong>[!UICONTROL Site ID]</strong>, <strong>[!UICONTROL List ID]</strong> e <strong>[!UICONTROL Folder ID]</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list that you follow]</strong> </p> <p>Seleccione la ubicación donde desea crear la carpeta. </p> </li> 
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
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter Site, Drive, and Folder IDs]</td> 
   <td> <p>Seleccione cómo identificar la ubicación del archivo que desea obtener.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Escriba o asigne el <strong>[!UICONTROL Site ID]</strong>, <strong>[!UICONTROL List ID]</strong> e <strong>[!UICONTROL File ID]</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list that you follow]</strong> </p> <p>Seleccione la ubicación del archivo. </p> </li> 
    </ul> </td> 
  </tr> 
</tbody> 
</table>

#### Ver elementos de la carpeta

Este módulo de activación inicia un escenario cuando se actualiza un elemento en una carpeta seleccionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter Site, Drive, and Folder IDs]</td> 
   <td> <p>Seleccione cómo identificar la ubicación del archivo que desea obtener.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Escriba o asigne el <strong>[!UICONTROL Site ID]</strong>, <strong>[!UICONTROL List ID]</strong> e <strong>[!UICONTROL folder ID]</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list that you follow]</strong> </p> <p>Seleccione la ubicación de la carpeta que desea ver. </p> </li> 
    </ul> </td> 
  </tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Introduzca el número máximo de elementos que [!DNL Workfront Fusion] debe devolver durante un ciclo de ejecución de escenario.</td> 
  <tr>
  </tr>
</tbody> 
</table>

### Elemento

* [[!UICONTROL Copiar un elemento]](#copy-an-item)
* [[!UICONTROL Crear un elemento]](#create-an-item)
* [[!UICONTROL Eliminar un elemento]](#delete-an-item)
* [[!UICONTROL Obtener un elemento]](#get-an-item)
* [[!UICONTROL Enumerar elementos]](#list-items)
* [[!UICONTROL Mover elemento]](#move-an-item)
* [[!UICONTROL Actualizar un elemento]](#update-an-item)
* [[!UICONTROL Ver elementos] (Programados)](#watch-items-scheduled)


#### [!UICONTROL Copiar elemento]

Este módulo de acción copia un elemento existente en una lista de SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], vea <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Introducir ID de sitio, unidad y carpeta</td> 
   <td> <p>Seleccione cómo desea identificar el sitio y la lista que contiene el elemento que desea copiar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Introduzca o asigne el <strong>[!UICONTROL Site ID]</strong>, <strong>[!UICONTROL List ID]</strong> y <strong>[!UICONTROL Item ID]</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from list that you follow]</strong> </p> <p>En el campo Tipo de elemento, seleccione si va a mover un campo o una carpeta.  Seleccione el sitio que contiene el elemento que desea copiar, seleccione la lista y, a continuación, seleccione el elemento. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destination ID]</td> 
   <td> Introduzca o asigne el ID de la carpeta en la que desea copiar el elemento. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL New name]</td> 
   <td>Introduzca o asigne un nombre para la nueva copia del elemento. </td> 
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
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], vea <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Create an Item]</td> 
   <td> <p>Seleccione cómo desea identificar el sitio y la lista donde desea crear un elemento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Introduzca o asigne el <strong>[!UICONTROL Site ID]</strong> y <strong>[!UICONTROL List ID]</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Seleccione el sitio que contiene la lista donde desea crear un elemento y, a continuación, seleccione la lista. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields]</td> 
   <td>Para cada campo que desee establecer para el nuevo elemento, introduzca la clave del campo (identifica el campo) y el valor que desea que tenga el nuevo elemento para ese campo.</td> 
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
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], vea <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Update an Item]</td> 
   <td> <p>Seleccione cómo desea identificar el sitio y la lista que contiene el elemento que desea eliminar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Introduzca o asigne el <strong>[!UICONTROL Site ID]</strong>, <strong>[!UICONTROL List ID]</strong> y <strong>[!UICONTROL Item ID]</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Seleccione el sitio que contiene el elemento que desea eliminar, seleccione la lista y, a continuación, seleccione el elemento. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener un elemento]

Este módulo de acción devuelve los datos de un elemento especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], vea <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Get an Item]</td> 
   <td> <p>Seleccione cómo desea identificar el sitio y la lista que contiene el elemento que desea obtener.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Introduzca o asigne el <strong>[!UICONTROL Site ID]</strong>, <strong>[!UICONTROL List ID]</strong> y <strong>[!UICONTROL Item ID]</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Seleccione el sitio que contiene la lista de la que desea recuperar un elemento, seleccione la lista y, a continuación, seleccione el elemento. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Enumerar elementos]

Este módulo de acción recupera una lista de todos los elementos de una lista especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], vea <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List Items]</td> 
   <td> <p>Seleccione cómo desea identificar la lista de la que desea recuperar elementos.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Introduzca o asigne el <strong>[!UICONTROL Site ID]</strong> y <strong>[!UICONTROL List ID]</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Seleccione el sitio que contiene la lista de la que desea recuperar elementos y, a continuación, seleccione la lista. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Introduzca o asigne el número máximo de elementos que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
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
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], vea <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Introducir ID de sitio, unidad y carpeta</td> 
   <td> <p>Seleccione cómo desea identificar el sitio y la lista que contiene el elemento que desea mover.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Introduzca o asigne el <strong>[!UICONTROL Site ID]</strong>, <strong>[!UICONTROL List ID]</strong> y <strong>[!UICONTROL Item ID]</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from list that you follow]</strong> </p> <p>En el campo Tipo de elemento, seleccione si va a mover un campo o una carpeta. Seleccione el sitio que contiene el elemento que desea copiar, seleccione la lista y, a continuación, seleccione el elemento. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destination ID]</td> 
   <td> Introduzca o asigne el ID de la carpeta a la que desea mover el elemento. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL New name]</td> 
   <td>Introduzca o asigne un nombre para el elemento movido. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actualice un elemento]

Este módulo de acción actualiza un elemento existente en una lista de SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], vea <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Update an Item]</td> 
   <td> <p>Seleccione cómo desea identificar el sitio y la lista que contiene el elemento que desea actualizar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Introduzca o asigne el <strong>[!UICONTROL Site ID]</strong>, <strong>[!UICONTROL List ID]</strong> y <strong>[!UICONTROL Item ID]</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Seleccione el sitio que contiene el elemento que desea actualizar, seleccione la lista y, a continuación, seleccione el elemento. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields]</td> 
   <td>Para cada campo que desee actualizar para el nuevo elemento, introduzca la clave del campo (identifica el campo) y el nuevo valor que desea que tenga el elemento para ese campo.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ver artículos] (Programados)

Este módulo de activación inicia un escenario cuando se crea o modifica un elemento.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], vea <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch Lists]</td> 
   <td>Seleccione si desea ver listas por hora de creación (elementos nuevos) o por hora de modificación (elementos actualizados).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter Site and List ID]</td> 
   <td> <p>Seleccione cómo desea identificar el sitio y la lista que desea ver.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Introduzca o asigne el <strong>[!UICONTROL Site ID]</strong> y <strong>[!UICONTROL List ID]</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list that you follow]</strong> </p> <p>Seleccione el sitio que desea ver y, a continuación, seleccione la lista. Estos desplegables solo recuperan los sitios seguidos.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Introduzca o asigne el número máximo de elementos que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Lista

* [[!UICONTROL Crear una lista]](#create-a-list)
* [[!UICONTROL Obtener una lista]](#get-a-list)
* [[!UICONTROL Enumerar listas]](#list-lists)
* [[!UICONTROL Ver listas]](#watch-lists)

#### [!UICONTROL Crear una lista]

Este módulo de acción crea una nueva lista en SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], vea <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter a Site ID]</td> 
   <td> <p>Seleccione cómo desea identificar el sitio y la lista donde desea crear una lista.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Introduzca o asigne el <strong>[!UICONTROL Site ID]</strong> donde desee crear una lista.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Seleccione el sitio en el que desea crear una lista. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Display Name]</td> 
   <td>Introduzca o asigne un nombre para la nueva lista.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>Introduzca o asigne una descripción para la nueva lista.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Add Columns]</td> 
   <td>Para cada columna que desee establecer para la nueva lista, introduzca un <strong>[!UICONTROL Name]</strong> para el campo y seleccione el <strong>[!UICONTROL Type]</strong> del valor que desea que tenga la nueva columna.</td> 
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
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], vea <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Get a List]</td> 
   <td> <p>Seleccione cómo desea identificar el sitio y la lista que contiene el elemento que desea obtener.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Introduzca o asigne <strong>[!UICONTROL Site ID]</strong> e <strong>ID de lista</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Seleccione el sitio que contiene la lista que desea recuperar y, a continuación, seleccione la lista. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Enumerar listas]

Este módulo de acción recupera una lista de todos los elementos de una lista especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], vea <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List Lists]</td> 
   <td> <p>Seleccione cómo desea identificar el sitio del que desea recuperar listas.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Introduzca o asigne el <strong>[!UICONTROL Site ID]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Seleccione el sitio que contiene las listas que desea recuperar. La lista desplegable recupera solo los sitios que sigue.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Introduzca o asigne el número máximo de listas que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ver listas]

Este módulo de activación inicia un escenario cuando se crea o modifica una lista.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], vea <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch Lists]</td> 
   <td>Seleccione si desea ver listas por hora de creación (elementos nuevos) o por hora de modificación (elementos actualizados).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter Site and List ID]</td> 
   <td> <p>Seleccione cómo desea identificar el sitio y la lista que desea ver.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Introduzca o asigne el <strong>[!UICONTROL Site ID]</strong> donde se encuentra la lista que desea ver.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list that you follow]</strong> </p> <p>Seleccione el sitio que desea ver. La lista desplegable solo recupera el sitio que sigue.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Introduzca o asigne el número máximo de listas que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Página (Beta)

>[!NOTE]
>
>Las API de la versión `beta` en [!DNL Microsoft Graph] están sujetas a cambios. No se admite el uso de estas API en aplicaciones de producción.

#### [!UICONTROL Obtener una página]

Este módulo de acción devuelve los datos de una página especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], vea <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Get a Page]</td> 
   <td> <p>Seleccione cómo desea identificar la página que desea recuperar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Introduzca o asigne el <strong>[!UICONTROL Site ID]</strong>y <strong>[!UICONTROL Page ID]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Seleccione el sitio que contiene la página que desea recuperar y, a continuación, seleccione la página.</p> </li> 
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
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], vea <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Get a Site]</td> 
   <td> <p>Seleccione cómo desea identificar la página que desea recuperar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Introduzca o asigne el <strong>[!UICONTROL Site ID]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Seleccione el sitio que desea recuperar.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Buscar sitios]

Este módulo de acción busca los sitios según el parámetro que especifique.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], vea <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Keyword of Display Name]</td> 
   <td> <p>Introduzca o asigne el término de búsqueda que desea buscar en los sitios.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Introduzca o asigne el número máximo de sitios que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Otro

* [Obtener cambios](#get-changes)
* [Realizar una llamada de API](#make-an-api-call)
* [Ver eventos](#watch-events)

#### Obtener cambios

Este módulo recupera las adiciones, actualizaciones y eliminaciones realizadas en la carpeta SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter Site, Drive, and Folder IDs]</td> 
   <td> <p>Seleccione cómo desea identificar el sitio y la lista que contiene el elemento que desea actualizar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Escriba o asigne el <strong>[!UICONTROL Site ID]</strong>, <strong>[!UICONTROL Drive ID]</strong> y <strong>[!UICONTROL Folder ID]</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Seleccione el sitio que contiene el elemento que desea actualizar, seleccione la unidad y, a continuación, seleccione la carpeta. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Token]</td> 
   <td> El token identifica desde qué punto el módulo debe comenzar a recuperar los cambios.  </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Realizar una llamada API]

Este módulo le permite realizar una llamada de API personalizada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], consulte <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Introduzca una ruta relativa a <code>https://graph.microsoft.com</code>. Ejemplo:<code> /beta/sites</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   <td> <p>Seleccione el método de petición HTTP que necesita para configurar la llamada de la API. Para obtener más información, vea <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de petición HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar. Por ejemplo, <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] añade los encabezados de autorización en su lugar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Añada la consulta para la llamada de API en forma de objeto JSON estándar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td>Seleccione el tipo de datos que desea enviar en la llamada de API.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Cuando utilice afirmaciones condicionales como <code>if</code> en su JSON, coloque las comillas fuera de la afirmación condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### Ver eventos

Este módulo de activación instantáneo inicia un escenario cuando se agrega, actualiza o elimina un elemento en SharePoint.

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
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Seleccione un webhook existente o haga clic en Agregar para crear un nuevo webhook.</p> 
   </td> 
  </tr> 
 </tbody> 
</table>

