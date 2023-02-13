---
title: Módulos Intacct
description: Módulos Intacct
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: fa1aa943-fbda-4eb4-bfa1-ab94a56785a7
source-git-commit: 9a4a847b542783845a3f896ec4e35d5efc7c122b
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 1%

---

# Módulos Intacct

En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan Intacct, así como conectarlos a varias aplicaciones y servicios de terceros.

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

Para utilizar módulos de Intacct, debe tener una cuenta de Intacct.

## Conectar Intacct a Workfront Fusion

### Autorización [!DNL Workfront Fusion] para realizar cambios en Intacct

Antes [!DNL Workfront Fusion] puede conectarse a [!DNL Intacct], debe autorizarlo.

En su cuenta de Instacct, vaya a la **[!UICONTROL Empresa]** pestaña .

1. Haga clic en **Información de la empresa**.
1. Vaya a la **Seguridad** pestaña .
1. Haga clic en [!UICONTROL Editar] en la esquina superior derecha
1. Seleccione Autorizaciones de servicios web.
1. Haga clic en el icono más
1. Introduzca AzuquaMPP como sender_id.
1. (Opcional) Introduzca una descripción para la conexión

### Configuración de una conexión en [!DNL Workfront Fusion] {#set-up-a-connection-in-workfront-fusion}

Puede crear una conexión con su [!DNL Intacct] cuenta directamente desde dentro de un [!DNL Intacct] módulo.

1. En cualquier módulo de Intacct, haga clic en **[!UICONTROL Agregar]** junto al campo Connection .
1. Introduzca las credenciales de Intacct

   * Identificador de compañía
   * Identificador del usuario
   * Contraseña

1. Haga clic en **[!UICONTROL Continuar]** para crear la conexión y volver al módulo .

## Módulos Intacct y sus campos

Al configurar [!DNL Intacct] módulos, [!DNL Workfront Fusion] muestra los campos que se enumeran a continuación. Junto con estos, podrían mostrarse campos de interacción adicionales, según factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón de asignación encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Realizar una llamada API personalizada]](#make-a-custom-api-call)
* [[!UICONTROL Registros de búsqueda]](#search-records)

### [!UICONTROL Realizar una llamada API personalizada] {#make-a-custom-api-call}

Este módulo de acción le permite realizar una llamada autenticada personalizada al [!DNL Intacct] API. De este modo, puede crear una automatización del flujo de datos que no se pueda lograr con la otra [!DNL Intacct] módulos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Conexión</p> </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de Intacct a [!DNL Workfront Fusion] 2.0, consulte <a href="#set-up-a-connection-in-workfront-fusion" class="MCXref xref">Configuración de una conexión en Workfront Fusion</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Código XML</td> 
   <td> <p>Incluir solo el XML dentro del cuerpo. La solicitud incluye automáticamente los encabezados de autenticación.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Registros de búsqueda]

Este módulo de búsqueda recupera una lista de registros que coinciden con criterios de búsqueda específicos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Conexión</p> </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de Intacct a [!DNL Workfront Fusion] 2.0, consulte <a href="#set-up-a-connection-in-workfront-fusion" class="MCXref xref">Configuración de una conexión en Workfront Fusion</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione el tipo de registro que desea buscar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Criterios de búsqueda</p> </td> 
   <td> 
    <ul> 
     <li> <p>Seleccione el campo en el que desea buscar</p> </li> 
     <li> <p>Seleccione el operador que desee utilizar para la búsqueda</p> </li> 
     <li> <p>Introduzca el valor que desea buscar</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Conjunto de resultados</td> 
   <td>Seleccione si desea devolver todos los registros coincidentes o solo el primer registro coincidente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Límite</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ordenar por</td> 
   <td>Seleccione el campo por el que desea ordenar los resultados. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ordenar</td> 
   <td>Seleccione si desea ordenar ascendente o descendente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Salidas</td> 
   <td> <p>Seleccione la información que desee incluir en el paquete de salida para este módulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Distinción entre mayúsculas y minúsculas</td> 
   <td>Active esta opción para que la consulta distinga entre mayúsculas y minúsculas.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Consultar en entidades privadas</td> 
   <td>Active esta opción para permitir que el módulo busque entidades privadas.</td> 
  </tr> 
 </tbody> 
</table>
