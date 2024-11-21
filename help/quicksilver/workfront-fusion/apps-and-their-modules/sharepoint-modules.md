---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de SharePoint
description: En un escenario de  [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan SharePoint, así como conectarlo a varias aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion
exl-id: 16d49031-06d2-4c86-bac4-f58cd9b2f1f5
source-git-commit: 2e91e9a4c691430f3c98e3cbddb30706ea57f84a
workflow-type: tm+mt
source-wordcount: '2877'
ht-degree: 0%

---

# [!DNL SharePoint] módulos

En un escenario de [!DNL Adobe Workfront Fusion], puede automatizar los flujos de trabajo que utilizan [!DNL SharePoint], así como conectarlo a varias aplicaciones y servicios de terceros.

Si necesita instrucciones para crear un escenario, consulte [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obtener información acerca de los módulos, vea [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td>
   <p>Requisito de licencia actual: no se requiere licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p>
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

Para usar módulos de [!DNL SharePoint], debe tener una cuenta de [!DNL SharePoint].

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

* [Conectar [!DNL SharePoint] a [!DNL Workfront Fusion] usando una [!DNL Microsoft] cuenta](#connect-sharepoint-to-workfront-fusion-using-a-microsoft-account)
* [Conectar [!DNL SharePoint] a [!DNL Workfront Fusion] mediante la configuración avanzada](#connect-sharepoint-to-workfront-fusion-using-advanced-settings)

### Conectar [!DNL SharePoint] a [!DNL Workfront Fusion] mediante una cuenta de [!DNL Microsoft]

Puede usar su cuenta de [!DNL Microsoft] para crear una conexión con [!DNL SharePoint]. Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Sharepoint] a [!DNL Workfront Fusion], vea [Crear una conexión a [!DNL Adobe Workfront Fusion] - Instrucciones básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

### Conectar [!DNL SharePoint] a [!DNL Workfront Fusion] mediante la configuración avanzada

Para conectar a [!DNL SharePoint] con [!DNL Workfront Fusion] sin una cuenta de [!DNL Microsoft], necesita un identificador de cliente, un secreto de cliente y un identificador de inquilino.

1. Haga clic en **[!UICONTROL Agregar]** cerca de la parte superior del cuadro **[!DNL SharePoint]** para abrir el cuadro **[!UICONTROL Crear una conexión]**.

1. (Opcional) Cambie el **[!UICONTROL nombre de conexión]** predeterminado.
1. Haga clic en **[!UICONTROL Mostrar configuración avanzada]**.
1. Escriba [!DNL SharePoint] **[!UICONTROL ID de cliente]** y **[!UICONTROL Secreto de cliente]**.

1. Haga clic en **[!UICONTROL Continuar]**.
1. En la ventana de inicio de sesión que aparece, introduzca sus credenciales para iniciar sesión en la aplicación si aún no lo ha hecho.
1. (Condicional) Si aparece un botón **[!UICONTROL Permitir]**, haga clic en el botón para conectar la aplicación a [!DNL Workfront Fusion].

## [!DNL SharePoint] módulos y sus campos

Al configurar [!DNL SharePoint] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL SharePoint] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, vea [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Elemento de unidad](#drive-item)
* [Elemento](#item)
* [Lista](#list)
* [Página (Beta)](#page-beta)
* [Sitio](#site)
* [Otro](#other)

### Elemento de unidad

* [Creación de un archivo](#create-a-file)
* [Crear una carpeta](#create-a-folder)
* [Obtener un archivo](#get-a-file)
* [Observar elementos de carpeta](#watch-folder-items)

#### Obtener cambios

Este módulo devuelve los cambios realizados en SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], vea <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escribir ID de sitio, unidad y carpeta]</td> 
   <td> <p>Seleccione cómo desea identificar la ubicación de la carpeta en la que desea recuperar los cambios.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Escriba o asigne el <strong>[!UICONTROL Id. de sitio]</strong>, <strong>[!UICONTROL Id. de lista]</strong> y <strong>[!UICONTROL Id. de carpeta]</strong> en los campos que aparecen.</p> </li> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], vea <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escribir ID de sitio, unidad y carpeta]</td> 
   <td> <p>Seleccione cómo desea identificar la ubicación de la carpeta que desea crear.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Escriba o asigne el <strong>[!UICONTROL Id. de sitio]</strong>, <strong>[!UICONTROL Id. de lista]</strong> y <strong>[!UICONTROL Id. de carpeta]</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccione en la lista que sigue]</strong> </p> <p>Seleccione la ubicación donde desea crear la carpeta. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre de carpeta]</td> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], vea <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escribir ID de sitio, unidad y carpeta]</td> 
   <td> <p>Seleccione cómo desea identificar la ubicación del archivo que desea obtener.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Escriba o asigne el <strong>[!UICONTROL Id. de sitio]</strong>, <strong>[!UICONTROL Id. de lista]</strong> y <strong>[!UICONTROL Id. de archivo]</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccione en la lista que sigue]</strong> </p> <p>Seleccione la ubicación del archivo. </p> </li> 
    </ul> </td> 
  </tr> 
</tbody> 
</table>

#### Observar elementos de carpeta

Este módulo de déclencheur inicia un escenario cuando se actualiza un elemento en una carpeta seleccionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], vea <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escribir ID de sitio, unidad y carpeta]</td> 
   <td> <p>Seleccione cómo desea identificar la ubicación del archivo que desea obtener.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Escriba o asigne el <strong>[!UICONTROL Id. de sitio]</strong>, <strong>[!UICONTROL Id. de lista]</strong> y <strong>[!UICONTROL Id. de carpeta]</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccione en la lista que sigue]</strong> </p> <p>Seleccione la ubicación de la carpeta que desea ver. </p> </li> 
    </ul> </td> 
  </tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
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
* [[!UICONTROL Elementos de lista]](#list-items)
* [[!UICONTROL Mover elemento]](#move-an-item)
* [[!UICONTROL Actualizar un elemento]](#update-an-item)
* [[!UICONTROL Artículos en seguimiento] (Programados)](#watch-items-scheduled)


#### [!UICONTROL Copiar elemento]

Este módulo de acción copia un elemento existente en una lista de SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], vea <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Introducir ID de sitio, unidad y carpeta</td> 
   <td> <p>Seleccione cómo desea identificar el sitio y la lista que contiene el elemento que desea copiar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Escriba o asigne el <strong>[!UICONTROL Id. de sitio]</strong>, <strong>[!UICONTROL Id. de lista]</strong> y <strong>[!UICONTROL Id. de elemento]</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar de la lista que sigue]</strong> </p> <p>En el campo Tipo de elemento, seleccione si va a mover un campo o una carpeta.  Seleccione el sitio que contiene el elemento que desea copiar, seleccione la lista y, a continuación, seleccione el elemento. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de destino]</td> 
   <td> Introduzca o asigne el ID de la carpeta en la que desea copiar el elemento. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nuevo nombre]</td> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], vea <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Crear un elemento]</td> 
   <td> <p>Seleccione cómo desea identificar el sitio y la lista donde desea crear un elemento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Escriba o asigne el <strong>[!UICONTROL Id. de sitio]</strong> y <strong>[!UICONTROL Id. de lista]</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccione de la lista]</strong> </p> <p>Seleccione el sitio que contiene la lista donde desea crear un elemento y, a continuación, seleccione la lista. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos]</td> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], vea <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Actualizar un elemento]</td> 
   <td> <p>Seleccione cómo desea identificar el sitio y la lista que contiene el elemento que desea eliminar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Escriba o asigne el <strong>[!UICONTROL Id. de sitio]</strong>, <strong>[!UICONTROL Id. de lista]</strong> y <strong>[!UICONTROL Id. de elemento]</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccione de la lista]</strong> </p> <p>Seleccione el sitio que contiene el elemento que desea eliminar, seleccione la lista y, a continuación, seleccione el elemento. </p> </li> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], vea <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obtener un elemento]</td> 
   <td> <p>Seleccione cómo desea identificar el sitio y la lista que contiene el elemento que desea obtener.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Escriba o asigne el <strong>[!UICONTROL Id. de sitio]</strong>, <strong>[!UICONTROL Id. de lista]</strong> y <strong>[!UICONTROL Id. de elemento]</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccione de la lista]</strong> </p> <p>Seleccione el sitio que contiene la lista de la que desea recuperar un elemento, seleccione la lista y, a continuación, seleccione el elemento. </p> </li> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], vea <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL elementos de lista]</td> 
   <td> <p>Seleccione cómo desea identificar la lista de la que desea recuperar elementos.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Escriba o asigne el <strong>[!UICONTROL Id. de sitio]</strong> y <strong>[!UICONTROL Id. de lista]</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccione de la lista]</strong> </p> <p>Seleccione el sitio que contiene la lista de la que desea recuperar elementos y, a continuación, seleccione la lista. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], vea <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Introducir ID de sitio, unidad y carpeta</td> 
   <td> <p>Seleccione cómo desea identificar el sitio y la lista que contiene el elemento que desea mover.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Escriba o asigne el <strong>[!UICONTROL Id. de sitio]</strong>, <strong>[!UICONTROL Id. de lista]</strong> y <strong>[!UICONTROL Id. de elemento]</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar de la lista que sigue]</strong> </p> <p>En el campo Tipo de elemento, seleccione si va a mover un campo o una carpeta. Seleccione el sitio que contiene el elemento que desea copiar, seleccione la lista y, a continuación, seleccione el elemento. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de destino]</td> 
   <td> Introduzca o asigne el ID de la carpeta a la que desea mover el elemento. </td> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], vea <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Actualizar un elemento]</td> 
   <td> <p>Seleccione cómo desea identificar el sitio y la lista que contiene el elemento que desea actualizar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Escriba o asigne el <strong>[!UICONTROL Id. de sitio]</strong>, <strong>[!UICONTROL Id. de lista]</strong> y <strong>[!UICONTROL Id. de elemento]</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccione de la lista]</strong> </p> <p>Seleccione el sitio que contiene el elemento que desea actualizar, seleccione la lista y, a continuación, seleccione el elemento. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos]</td> 
   <td>Para cada campo que desee actualizar para el nuevo elemento, introduzca la clave del campo (identifica el campo) y el nuevo valor que desea que tenga el elemento para ese campo.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Artículos en seguimiento] (Programados)

Este módulo de déclencheur inicia un escenario cuando se crea o modifica un elemento.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], vea <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Listas de observación]</td> 
   <td>Seleccione si desea inspeccionar listas por hora de creación (elementos nuevos) o por hora de modificación (elementos actualizados).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Introducir sitio e ID de lista]</td> 
   <td> <p>Seleccione cómo desea identificar el sitio y la lista que desea ver.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Escriba o asigne el <strong>[!UICONTROL Id. de sitio]</strong> y <strong>[!UICONTROL Id. de lista]</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccione en la lista que sigue]</strong> </p> <p>Seleccione el sitio que desea ver y, a continuación, seleccione la lista. Estos desplegables solo recuperan los sitios seguidos.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de elementos que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Lista

* [[!UICONTROL Crear una lista]](#create-a-list)
* [[!UICONTROL Obtener una lista]](#get-a-list)
* [[!UICONTROL Listas de listas]](#list-lists)
* [[!UICONTROL Listas de observación]](#watch-lists)

#### [!UICONTROL Crear una lista]

Este módulo de acción crea una nueva lista en SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], vea <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escriba un Id. de sitio]</td> 
   <td> <p>Seleccione cómo desea identificar el sitio y la lista donde desea crear una lista.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Escriba o asigne el <strong>[!UICONTROL Id. de sitio]</strong> donde desee crear una lista.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccione de la lista]</strong> </p> <p>Seleccione el sitio en el que desea crear una lista. </p> </li> 
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
   <td>Para cada columna que desee establecer para la nueva lista, escriba un <strong>[!UICONTROL Nombre]</strong> para el campo y seleccione el <strong>[!UICONTROL Tipo]</strong> del valor que desea que tenga la nueva columna.</td> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], vea <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obtener una lista]</td> 
   <td> <p>Seleccione cómo desea identificar el sitio y la lista que contiene el elemento que desea obtener.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Escriba o asigne <strong>[!UICONTROL Id. de sitio]</strong> y <strong>Id. de lista</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccione de la lista]</strong> </p> <p>Seleccione el sitio que contiene la lista que desea recuperar y, a continuación, seleccione la lista. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listas de listas]

Este módulo de acción recupera una lista de todos los elementos de una lista especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], vea <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Listas de listas]</td> 
   <td> <p>Seleccione cómo desea identificar el sitio del que desea recuperar listas.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Escriba o asigne el <strong>[!UICONTROL Id. de sitio]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccione de la lista]</strong> </p> <p>Seleccione el sitio que contiene las listas que desea recuperar. La lista desplegable recupera solo los sitios que sigue.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de listas que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listas de observación]

Este módulo de déclencheur inicia un escenario cuando se crea o modifica una lista.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], vea <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Listas de observación]</td> 
   <td>Seleccione si desea inspeccionar listas por hora de creación (elementos nuevos) o por hora de modificación (elementos actualizados).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Introducir sitio e ID de lista]</td> 
   <td> <p>Seleccione cómo desea identificar el sitio y la lista que desea ver.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Escriba o asigne el <strong>[!UICONTROL Id. de sitio]</strong> donde se encuentra la lista que desea ver.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccione en la lista que sigue]</strong> </p> <p>Seleccione el sitio que desea ver. La lista desplegable solo recupera el sitio que sigue.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], vea <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obtener una página]</td> 
   <td> <p>Seleccione cómo desea identificar la página que desea recuperar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Escriba o asigne el <strong>[!UICONTROL Id. de sitio]</strong> y <strong>[!UICONTROL Id. de página]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccione de la lista]</strong> </p> <p>Seleccione el sitio que contiene la página que desea recuperar y, a continuación, seleccione la página.</p> </li> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], vea <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obtener un sitio]</td> 
   <td> <p>Seleccione cómo desea identificar la página que desea recuperar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Escriba o asigne el <strong>[!UICONTROL Id. de sitio]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccione de la lista]</strong> </p> <p>Seleccione el sitio que desea recuperar.</p> </li> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], vea <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Palabra clave [!UICONTROL del nombre para mostrar]</td> 
   <td> <p>Escriba o asigne el término de búsqueda que desea buscar en los sitios.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], vea <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escribir ID de sitio, unidad y carpeta]</td> 
   <td> <p>Seleccione cómo desea identificar el sitio y la lista que contiene el elemento que desea actualizar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Escriba o asigne el <strong>[!UICONTROL Id. de sitio]</strong>, <strong>[!UICONTROL Id. de unidad]</strong> y <strong>[!UICONTROL Id. de carpeta]</strong> en los campos que aparecen.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccione de la lista]</strong> </p> <p>Seleccione el sitio que contiene el elemento que desea actualizar, seleccione la unidad y, a continuación, seleccione la carpeta. </p> </li> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL SharePoint] a [!DNL Workfront Fusion], vea <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Escriba una ruta relativa a <code>https://graph.microsoft.com</code>. Ejemplo:<code> /beta/sites</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Método]</p> </td> 
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada de API. Para obtener más información, vea <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Agregue los encabezados de la solicitud en forma de objeto JSON estándar. Por ejemplo, <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] agrega los encabezados de autorización por usted.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadena de consulta]</td> 
   <td> <p> Añada la consulta para la llamada de API en forma de objeto JSON estándar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo]</td> 
   <td>Seleccione el tipo de datos que desea enviar en la llamada de API.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cuerpo]</td> 
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Cuando utilice afirmaciones condicionales como <code>if</code> en su JSON, coloque las comillas fuera de la afirmación condicional.</p> 
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
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Seleccione un webhook existente o haga clic en Agregar para crear un nuevo webhook.</p> 
   </td> 
  </tr> 
 </tbody> 
</table>

