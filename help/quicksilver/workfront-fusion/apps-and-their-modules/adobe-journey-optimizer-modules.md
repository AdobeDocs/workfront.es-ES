---
filename: adobe-journey-optimizer-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Módulos de Adobe Journey Optimizer
description: En un  [!DNL Adobe Workfront Fusion] escenario, puede automatizar los flujos de trabajo que usan [!DNL Adobe Journey Optimizer], así como conectarlo a varias aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion
exl-id: 2c1aea46-edbf-42a3-a6e9-f8aea042a48d
source-git-commit: f6b00b98d3375e5660d684f1fad682fa721517aa
workflow-type: tm+mt
source-wordcount: '3692'
ht-degree: 0%

---

# [!DNL Adobe Journey Optimizer] módulos

En un escenario de [!DNL Adobe Workfront Fusion], puede automatizar los flujos de trabajo que utilizan [!DNL Adobe Journey Optimizer], así como conectarlo a varias aplicaciones y servicios de terceros. Los módulos [!DNL Adobe Journey Optimizer] le permiten crear, leer, actualizar o eliminar registros, o realizar una llamada de API personalizada a la API [!DNL Adobe Journey Optimizer].


Si necesita instrucciones para crear un escenario, consulte [Crear un escenario](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obtener información acerca de los módulos, vea [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
      <td>
        <p>[!UICONTROL Pro] o superior</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] licencia*</td>
      <td>
        <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p>
      </td>
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

+++

## Requisitos previos

Antes de poder usar el conector [!DNL Adobe Journey Optimizer], debe asegurarse de que se cumplen los siguientes requisitos previos:

* Debe tener una cuenta de [!DNL Adobe Journey Optimizer] activa.

## Información de API de Adobe Journey Optimizer

El conector de Adobe Journey Optimizer utiliza lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL básica</td> 
   <td>{{connection.url}}</td> 
  </tr>
  <tr> 
   <td role="rowheader">Etiqueta de API</td> 
   <td>Versión 1.7.11</td> 
  </tr>
 </tbody> 
 </table>

## Creación de una conexión con Adobe Journey Optimizer

Puede crear una conexión en cualquier módulo de Adobe Journey Optimizer.

1. Haga clic en **[!UICONTROL Agregar]** junto al cuadro Conexión.

1. Rellene los campos siguientes:

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
        <td role="rowheader">[!UICONTROL Nombre de conexión]</td>
        <td>
          <p>Escriba un nombre para esta conexión.</p>
        </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Entorno]</td>
        <td>Seleccione si desea conectarse a un entorno de producción o de no producción.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Tipo]</td>
        <td>Seleccione si desea conectarse a una cuenta de servicio o a una cuenta personal.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL ID de cliente]</td>
        <td>Introduzca el [!UICONTROL Adobe] [!UICONTROL ID de cliente]. Esto se puede encontrar en la sección de detalles de [!UICONTROL Credentials] de [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Secreto de cliente]</td>
        <td>Escriba su [!UICONTROL Secreto de cliente] [!DNL Adobe]. Esto se puede encontrar en la sección de detalles de [!UICONTROL Credentials] de [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL ID de organización]</td>
        <td>Escriba su [!UICONTROL Organization ID] de [!DNL Adobe]. Esto se puede encontrar en la sección de detalles de [!UICONTROL Credentials] de [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Nombre de zona protegida]</td>
        <td>Introduzca el nombre de la zona protegida que utilizará esta conexión.</td>
        </tr>
      </tbody>
    </table>


## [!DNL Adobe Journey Optimizer] módulos y sus campos

Al configurar [!DNL Adobe Journey Optimizer] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL Adobe Journey Optimizer] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, vea [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Administración de configuración](#configuration-management)
* [Administración de paquetes](#package-management)
* [Administración de registros](#record-management)
* [Administración de mensajes](#message-management)
* [Comprobaciones de estado](#status-checks)
* [Búsquedas](#searches)
* [Otro](#other)




### Administración de configuración

* [Crear una configuración](#create-a-configuration)
* [Implementar una configuración](#deploy-a-configuration)
* [Actualizar una configuración](#update-a-configuration)
* [Anular la implementación de una configuración](#undeploy-a-configuration)
* [Comprobar si la configuración se puede implementar](#check-if-configuration-can-be-deployed)
* [Eliminar una configuración](#delete-a-configuration)
* [Obtener una configuración](#get-a-configuration)

#### Crear una configuración

Este módulo de acción crea un extremo de límite o una configuración de restricción.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Journey Optimizer], vea <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Crear una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seleccionar tipo de configuración]</td> 
   <td>Seleccione si va a crear una configuración de límite o una configuración de restricción.<ul><li><p><b>Límite</b></p>Continúe con <a href="#capping-fields" class="MCXref xref" >Campos de límite</a>.</li><li><p><b>Aceleración</b></p>Continuar a <a href="#throttling-fields" class="MCXref xref" >Campos de restricción</a>.</li></ul></td> 
  </tr> 
   </tbody> 
</table>

##### Campos de límite

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Introduzca o asigne la dirección URL del punto de conexión que desea configurar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL IMS Org ID]</td> 
   <td>Introduzca o asigne el ID de IMS de Adobe de la organización.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Métodos]</td> 
   <td>Seleccione los métodos que desea utilizar en esta configuración.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Service]</td> 
   <td>Seleccione si está utilizando una acción o una fuente de datos para esta configuración.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Máximo de conexiones HTTP]</td> 
   <td>Introduzca o asigne el número máximo de conexiones simultáneas a este punto final.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Llamadas máximas]</td> 
   <td>Introduzca o asigne el número máximo de llamadas que se realizarán en el periodo especificado en el campo Periodo de tiempo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Periodo de tiempo (milisegundos)]</td> 
   <td>Introduzca o asigne el número de milisegundos relacionados con el campo Máximo de llamadas.</td> 
  </tr> 
 </tbody> 
</table>

##### Campos de restricción

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> <tr> 
   <td role="rowheader">[!UICONTROL Nombre]</td> 
   <td>Escriba o asigne un nombre para esta configuración.</td> 
<tr> 
   <td role="rowheader">[!UICONTROL Descripción]</td> 
   <td>Escriba o asigne una descripción para esta configuración.</td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL patrón de URL]</td> 
   <td>Introduzca o asigne la dirección URL del punto de conexión al que desee acelerar.</td> 
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Métodos]</td> 
   <td>Seleccione los métodos que desea utilizar en esta configuración.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Rendimiento máximo]</td> 
   <td>Seleccione si está utilizando una acción o una fuente de datos para esta configuración.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Máximo de conexiones HTTP]</td> 
   <td>Introduzca o asigne el número máximo de conexiones simultáneas a este punto final.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Llamadas máximas]</td> 
   <td>Especifique o asigne el rendimiento máximo que desea para este punto de conexión. Este valor debe estar entre 200 y 5000.</td> 
  </tr> 
 </tbody> 
</table>

#### Implementar una configuración

Este módulo de acción implementa la configuración de límite o regulación especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Journey Optimizer], vea <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Crear una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seleccionar tipo de configuración]</td> 
   <td>Seleccione si va a implementar una configuración de límite o de restricción.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de configuración]</td> 
   <td>Introduzca o asigne el ID de la configuración que desea implementar.</td> 
  </tr> 
 </tbody> 
</table>

#### Actualizar una configuración

Este módulo de acción actualiza la configuración de límite o regulación especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Journey Optimizer], vea <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Crear una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seleccionar tipo de configuración]</td> 
   <td>Seleccione si va a actualizar una configuración de límite o de restricción.<ul><li><p><b>Límite</b></p>Para ver los campos, consulte <a href="#capping-fields" class="MCXref xref" >Campos de límite</a> en la sección Crear una configuración de este artículo.</li><li><p><b>Aceleración</b></p>Para ver los campos, consulte <a href="#throttling-fields" class="MCXref xref" >Campos de restricción</a> en la sección Crear una configuración de este artículo.</li></ul></td> 
  </tr> 
  </tbody> 
</table>

#### Anular la implementación de una configuración

Este módulo de acción anula la implementación de una configuración de límite o restricción. El estado de configuración vuelve a cambiarse al estado anterior a la implementación (`created` o `updated`).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Journey Optimizer], vea <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Crear una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seleccionar tipo de configuración]</td> 
   <td>Seleccione si va a anular la implementación de una configuración de límite o de restricción.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de configuración]</td> 
   <td>Introduzca o asigne el ID de la configuración que desea anular la implementación.</td> 
  </tr> 
 </tbody> 
</table>

#### Comprobar si la configuración se puede implementar

Este módulo de acción verifica si se puede implementar una configuración de restricción o límite.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Journey Optimizer], vea <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Crear una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seleccionar tipo de configuración]</td> 
   <td>Seleccione si está comprobando una configuración de límite o de restricción.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de configuración]</td> 
   <td>Introduzca o asigne el ID de la configuración que desea comprobar.</td> 
  </tr> 
 </tbody> 
</table>

#### Eliminar una configuración

Este módulo de acción elimina un extremo de límite o una configuración de restricción.

Si la configuración se ha implementado, debe anular su implementación para poder eliminarla.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Journey Optimizer], vea <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Crear una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seleccionar tipo de configuración]</td> 
   <td>Seleccione si desea eliminar una configuración de límite o de restricción.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de configuración]</td> 
   <td>Introduzca o asigne el ID de la configuración que desea eliminar.</td> 
  </tr> 
 </tbody> 
</table>

#### Obtener una configuración

Este módulo de acción devuelve la configuración de límite o limitación identificada por el ID especificado. Se devuelve la definición más reciente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Journey Optimizer], vea <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Crear una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seleccionar tipo de configuración]</td> 
   <td>Seleccione si va a recuperar una configuración de límite o de restricción.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de configuración]</td> 
   <td>Introduzca o asigne el ID de la configuración que desea recuperar.</td> 
  </tr> 
 </tbody> 
</table>




### Administración de paquetes

* [Creación de un paquete](#create-a-package)
* [Actualización de un paquete](#update-a-package)
* [Eliminación de un paquete](#delete-a-package)
* [Búsqueda de un paquete](#look-up-a-package)
* [Importar un paquete](#import-a-package)
* [Publish un paquete](#publish-a-package)
* [Envío de una importación](#submit-an-import)



#### Creación de un paquete

Este módulo de acción crea un paquete de varios artefactos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Journey Optimizer], vea <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Crear una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre]</td> 
   <td>Introduzca o asigne un nombre para el paquete.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descripción]</td> 
   <td>Introduzca o asigne una descripción del paquete.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fecha de caducidad]</td> 
   <td>Introduzca o asigne la marca de tiempo que define la fecha de caducidad del paquete. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de paquete]</td> 
   <td>Seleccione el tipo de paquete que desea crear.<ul><li><p><b>Completo</b></p>El paquete incluirá todos los artefactos</p></li><li><p><b>Parcial</b></p><p>El paquete solo incluirá los artefactos que agregue. </p></li><ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Artefactos]</td> 
   <td>Si va a crear un paquete parcial, para cada artefacto que desee agregar, haga clic en <b>Agregar artefacto</b> y especifique el identificador, el tipo y el título del artefacto. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Entorno aislado de [!UICONTROL Source]</td> 
   <td>Introduzca o asigne el nombre y el ID de organización de IMS de la zona protegida que contiene los elementos que desea que contenga el paquete.</td> 
  </tr> 
 </tbody> 
</table>

#### Actualización de un paquete

Este módulo de acción añade o elimina artefactos de un paquete, o actualiza los metadatos del paquete.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Journey Optimizer], vea <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Crear una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seleccionar acción]</td> 
   <td>Seleccione la acción que desee realizar.<ul><li><p><b>Agregar artefacto</b></p><p>Para cada artefacto que desee agregar, haga clic en <b>Agregar artefacto</b>, especifique el identificador, el tipo y el título del artefacto y, a continuación, escriba o asigne la fecha de caducidad del paquete. </p></li><li><p><b>Eliminar artefacto</b></p><p>Para cada artefacto que desee eliminar, haga clic en <b>Agregar artefacto</b> y especifique el identificador, el tipo y el título del artefacto. </p></li><li><p><b>Actualización de metadatos</b></p><p>Introduzca nuevos valores para el nombre, la descripción o el nombre de la zona protegida de origen o el ID de organización de IMS.</p></li></ul></td> 
  </tr> 
 </tbody> 
</table>

#### Eliminación de un paquete

Este módulo de acción elimina un paquete de varios artefactos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Journey Optimizer], vea <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Crear una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de paquete]</td> 
   <td>Introduzca o asigne el ID del paquete que desea eliminar.</td> 
  </tr> 
 </tbody> 
</table>

#### Búsqueda de un paquete

Este módulo de acción recupera los detalles del paquete especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Journey Optimizer], vea <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Crear una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de paquete]</td> 
   <td>Introduzca o asigne el ID del paquete cuyos detalles desea devolver.</td> 
  </tr> 
 </tbody> 
</table>

#### Importar un paquete

Este módulo de acción recupera los objetos en conflicto de la zona protegida de destino especificada. Los objetos en conflicto representan objetos similares que ya están presentes en la zona protegida de destino.

Debe publicar un paquete para poder importarlo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Journey Optimizer], vea <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Crear una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de paquete]</td> 
   <td>Introduzca o asigne el ID del paquete que desea importar.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL Entorno de pruebas de destino]</td> 
   <td>Introduzca o asigne el nombre de la zona protegida en la que desea importar el paquete.</td> 
  </tr> 
 </tbody> 
</table>

#### Publish un paquete

Debe publicar un paquete para poder importarlo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Journey Optimizer], vea <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Crear una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de paquete]</td> 
   <td>Introduzca o asigne el ID del paquete que desea publicar.</td> 
  </tr> 
 </tbody> 
</table>

#### Envío de una importación

Este módulo de acción envía una importación para un paquete después de haber revisado los conflictos y proporcionado las sustituciones. El resultado se proporciona como carga útil, que inicia el trabajo de importación para la zona protegida de destino según se especifica en la carga útil.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Journey Optimizer], vea <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Crear una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de paquete]</td> 
   <td>Introduzca o asigne el ID del paquete que desea publicar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre]</td> 
   <td>Introduzca o asigne un nombre para el trabajo de importación.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descripción]</td> 
   <td>Introduzca o asigne una descripción del trabajo de importación</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL (Nombre de zona protegida de destino)]</td> 
   <td>Introduzca o asigne el nombre de la zona protegida a la que está enviando la importación.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL (zona protegida de destino) ID de organización de IMS]</td> 
   <td>Introduzca o asigne el ID de organización de Adobe IMS para la zona protegida a la que envía la importación.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID de [!UICONTROL (zona protegida de Source)]</td> 
   <td>Introduzca o asigne el ID de la zona protegida que contiene el paquete que desea publicar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tipo de [!UICONTROL (zona protegida de Source)]</td> 
   <td></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Vínculo de [!UICONTROL (zona protegida de Source)]</td> 
   <td>Introduzca o asigne el vínculo del paquete que desea publicar.</td> 
  </tr> 
 </tbody> 
</table>


<!--

### Artifact management

* [Copy artifacts synchronously](#copy-artifacts-synchronously)
* [Export artifacts asynchronously](#export-artifacts-asynchronously)
* [Import artifacts asynchronously](#import-artifacts-asynchronously)

#### Copy artifacts synchronously

This action module copies artifacts from a source sandbox into a destination sandbox.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Enter or map a name for the new file</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>Enter or map a description for the new file</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Visibility]</td> 
   <td></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destination sandbox]</td> 
   <td></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Artifacts]</td> 
   <td>For each artifact you want to copy, click <b>Add artifact</b> and continue to <a href="#artifact-fields" class="MCXref xref" >Artifact fields</a>.</td> 
  </tr> 
 </tbody> 
</table>

##### Artifact fields

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Enter or map the ID of the artifact.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td>Enter or map the artifact type, such as <code>REGISTRY_SCHEMA<code> or <code>JOURNEY</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Version]</td> 
   <td>Enter or map the visibility of the artifact. This applies only to Registry objects.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Visibility]</td> 
   <td>Enter or map the visibility (tenant or global). This applies only to Registry objects.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Found]</td> 
   <td>Select <b>Yes</b> if this item was found using a GET operation.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tasks]</td> 
   <td>For each task you want to add, click <b>Add task</b> and fill in the following:
   <ul>
   <li><p><b>Method</b></p></li>
   <li><p><b>Action</b></p></li>
   <li><p><b>Using</b></p></li>
   <li><p><b>With</b></p></li>
   </ul>
   </td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Messages]</td> 
   <td>For each task you want to add, click <b>Add message</b> and fill in the following:
   <ul>
   <li><p><b>Status</b></p><p>Enter or map the status that this message represents, such as <code>ERROR</code>.</li>
   <li><p><b>Attempt</b></p><p>Enter or map the attempt number related to this message. This may be useful if different attempts produce different messages.</p></li>
   <li><p><b>Message</b></p><p>Enter or map the text of the message.</li>
   <li><p><b>Object</b></p></li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>

#### Export Artifacts asynchronously

This action module exports artifacts from the specified sandbox.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Enter or map a name for the export file</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>Enter or map a description for the export file</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Visibility]</td> 
   <td></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Artifacts]</td> 
   <td>For each artifact you want to export, click <b>Add artifact</b> and continue to <a href="#artifact-fields" class="MCXref xref" >Artifact fields</a>.</td> 
  </tr> 
 </tbody> 
</table>

##### Artifact fields

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Enter or map the ID of the artifact.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td>Enter or map the artifact type, such as <code>REGISTRY_SCHEMA<code> or <code>JOURNEY</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Version]</td> 
   <td>Enter or map the visibility of the artifact. This applies only to Registry objects.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Visibility]</td> 
   <td>Enter or map the visibility (tenant or global). This applies only to Registry objects.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Found]</td> 
   <td>Select <b>Yes</b> if this item was found using a GET operation.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tasks]</td> 
   <td>For each task you want to add, click <b>Add task</b> and fill in the following:
   <ul>
   <li><p><b>Method</b></p></li>
   <li><p><b>Action</b></p></li>
   <li><p><b>Using</b></p></li>
   <li><p><b>With</b></p></li>
   </ul>
   </td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Messages]</td> 
   <td>For each task you want to add, click <b>Add message</b> and fill in the following:
   <ul>
   <li><p><b>Status</b></p><p>Enter or map the status that this message represents, such as <code>ERROR</code>.</li>
   <li><p><b>Attempt</b></p><p>Enter or map the attempt number related to this message. This may be useful if different attempts produce different messages.</p></li>
   <li><p><b>Message</b></p><p>Enter or map the text of the message.</li>
   <li><p><b>Object</b></p></li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>



#### Import Artifacts asynchronously

This action module imports a snapshot containing artifacts.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Snapshot ID]</td> 
   <td>Enter or map the ID of the snapshot you want to import.</td> 
  </tr> 
 </tbody> 
</table>

-->

### Administración de registros

* [Creación de un registro](#create-a-record)
* [Actualización de un registro](#update-a-record)
* [Eliminación de un registro](#delete-a-record)
* [Revisión de un registro](#patch-a-record)
* [Obtener un registro](#get-a-record)

#### Creación de un registro

Este módulo de acción crea una nueva plantilla de contenido o fragmento de contenido.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Journey Optimizer], vea <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Crear una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seleccionar tipo de contenido]</td> 
   <td>Seleccione si va a crear una plantilla de contenido o un fragmento de contenido.<ul><li><p><b>Plantilla de contenido</b></p>Continuar a <a href="#template-fields" class="MCXref xref" >Campos de plantilla</a>.</li><li><p><b>Fragmento de contenido</b></p>Continuar a <a href="#fragment-fields" class="MCXref xref" >Campos de fragmento</a>.</li></ul></td> 
  </tr> 
  </tbody> 
</table>

##### Campos de plantilla

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> <tr> 
   <td role="rowheader">[!UICONTROL Nombre]</td> 
   <td>Escriba o asigne un nombre para esta plantilla de contenido.</td> 
<tr> 
   <td role="rowheader">[!UICONTROL Descripción]</td> 
   <td>Escriba o asigne una descripción para esta plantilla de contenido.</td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL Tipo]</td> 
   <td>Seleccione el tipo de plantilla que desea crear.</td> 
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Canales]</td> 
   <td>Seleccione los canales incluidos en esta plantilla.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Origen de plantilla de contenido]</td> 
   <td>Seleccione el origen de esta plantilla.</td>  
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadatos]</td> 
   <td>Para incluir propiedades personalizadas en la nueva plantilla, seleccione "Añadir metadatos" e introduzca o asigne la clave y el valor de los metadatos. Repita el proceso para cada campo personalizado que desee incluir.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL HTML de correo electrónico]</td> 
   <td>Introduzca o asigne el HTML del correo electrónico incluido en esta plantilla.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Editor context]</td> 
   <td>Para incluir propiedades personalizadas en el correo electrónico, seleccione Añadir contexto del editor e introduzca o asigne la clave y el valor del contexto. Repita el proceso para cada campo personalizado que desee incluir.</td> 
  </tr> 
 </tbody> 
</table>

##### Campos de fragmento

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> <tr> 
   <td role="rowheader">[!UICONTROL Nombre]</td> 
   <td>Introduzca o asigne un nombre para este fragmento de contenido.</td> 
<tr> 
   <td role="rowheader">[!UICONTROL Descripción]</td> 
   <td>Escriba o asigne una descripción para este fragmento de contenido.</td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL Tipo]</td> 
   <td>Seleccione el tipo de plantilla que desea crear.</td> 
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Canales]</td> 
   <td>Seleccione los canales incluidos en esta plantilla.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Origen de fragmento de contenido]</td> 
   <td>Seleccione el origen de este fragmento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadatos]</td> 
   <td>Para incluir propiedades personalizadas en la nueva plantilla, seleccione "Añadir metadatos" e introduzca o asigne la clave y el valor de los metadatos. Repita el proceso para cada campo personalizado que desee incluir.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contenido]</td> 
   <td>Introduzca o asigne el contenido del fragmento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Editor context]</td> 
   <td>Para incluir propiedades personalizadas en el correo electrónico, seleccione Añadir contexto del editor e introduzca o asigne la clave y el valor del contexto. Repita el proceso para cada campo personalizado que desee incluir.</td> 
  </tr> 
 </tbody> 
</table>

#### Actualización de un registro

Este módulo de acción actualiza una plantilla de contenido o un fragmento.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Journey Optimizer], vea <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Crear una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seleccionar tipo de contenido]</td> 
   <td>Seleccione si va a actualizar una configuración de límite o de restricción.<ul><li><p><b>Plantilla</b></p>Para ver los campos, consulte <a href="#template-fields" class="MCXref xref" >Campos de plantilla</a> en la sección Crear un registro de este artículo.</li><li><p><b>Fragmento</b></p>Para ver los campos, consulte <a href="#fragment-fields" class="MCXref xref" >Campos de fragmento</a> en la sección Crear un registro de este artículo.</li></ul></td> 
  </tr> 
  </tbody> 
  </table>

#### Eliminación de un registro

Este módulo de acción elimina una plantilla o un fragmento de contenido.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Journey Optimizer], vea <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Crear una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seleccionar tipo de contenido]</td> 
   <td>Seleccione si desea eliminar una plantilla de contenido o un fragmento de contenido.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Plantilla/ID de fragmento]</td> 
   <td>Introduzca o asigne el ID de la plantilla o el fragmento que desea eliminar.</td> 
  </tr> 
 </tbody> 
</table>

#### Revisión de un registro

Este módulo de acción actualiza un registro con un PATCH con formato de puntero JSON

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Journey Optimizer], vea <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Crear una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seleccionar tipo de contenido]</td> 
   <td>Seleccione si va a aplicar parches a una plantilla de contenido o a un fragmento de contenido.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Plantilla/ID de fragmento]</td> 
   <td>Introduzca o asigne el ID de la plantilla o el fragmento al que desee aplicar el parche.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Datos de carga]</td> 
   <td>Para añadir un registro a la carga útil de este parche: <ol><li>Haga clic en <b>Agregar un registro</b>.</li><li>Seleccione la operación: Agregar, Quitar o Reemplazar.</li><li>En el campo Ruta, seleccione si desea aplicar un parche al nombre o a la descripción.</li><li> En el campo Desde, introduzca o asigne una cadena que contenga un valor de puntero JSON.</li><li>En el campo Value, introduzca el valor que desea utilizar en la operación.</li></ol></td> 
  </tr> 
 </tbody> 
</table>

#### Obtener un registro

Este módulo de acción devuelve la plantilla de contenido o el fragmento de contenido identificado por el ID especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Journey Optimizer], vea <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Crear una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seleccionar tipo de contenido]</td> 
   <td>Seleccione si va a recuperar una plantilla de contenido o un fragmento de contenido.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Plantilla/ID de fragmento]</td> 
   <td>Introduzca o asigne el ID de la plantilla o el fragmento que desea recuperar.</td> 
  </tr> 
 </tbody> 
</table>


### Administración de mensajes

* [Déclencheur de la ejecución de un mensaje unitario](#trigger-a-unitary-message-execution)
* [Déclencheur de un mensaje basado en audiencias](#trigger-an-audience-based-message)
* [Comprobar el estado de un mensaje basado en audiencias](#check-the-status-for-audience-based-message)



#### Déclencheur de la ejecución de un mensaje unitario

Déclencheur Este módulo de acción envía un mensaje unitario a los destinatarios especificados.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Journey Optimizer], vea <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Crear una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de solicitud]</td> 
   <td>Introduzca o asigne el ID de la solicitud asociada a este mensaje.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de campaña]</td> 
   <td>Introduzca o asigne el ID de la campaña asociada con este mensaje.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destinatarios]</td> 
   <td>Para cada destinatario que desee recibir este mensaje, haga clic en <b>Agregar destinatario</b> e introduzca lo siguiente:
   <ul>
   <li><p><b>Tipo</b></p>Seleccione <code>aep</code>.</li>
   <li><p><b>ID de usuario</b></p>Introduzca o asigne el identificador de perfil de Adobe Experience Platform del destinatario.</li>
   <li><p><b>Área de nombres</b></p>Introduzca o asigne el área de nombres del perfil de Adobe Experience Platform del destinatario.</li>
   <li><p><b>Dirección de correo electrónico</b></p></li>
   <li><p><b>Número de teléfono móvil</b></p></li>
   <li><p><b>Nombre</b></p></li>
   <li><p><b>Apellidos</b></p></li>
   <li><p><b>Producto</b></p>Introduzca o asigne el producto asociado a este mensaje. Se utiliza para la sustitución dinámica de variables en el contenido del mensaje.</li>
   </ul></td> 
  </tr> 
 </tbody> 
</table>

#### Déclencheur de un mensaje basado en audiencias

Este módulo de acción déclencheur la ejecución de un mensaje basado en audiencias, según la solicitud y la campaña que especifique.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Journey Optimizer], vea <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Crear una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de solicitud]</td> 
   <td>Introduzca o asigne el ID de la solicitud asociada a este mensaje.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de campaña]</td> 
   <td>Introduzca o asigne el ID de la campaña asociada con este mensaje.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Product]</td> 
   <td>Introduzca o asigne el producto asociado a este mensaje. Se utiliza para la sustitución dinámica de variables en el contenido del mensaje.</td> 
  </tr> 
 </tbody> 
</table>

#### Comprobar el estado de los mensajes basados en audiencias

Este módulo de acción comprueba el estado de un mensaje por lotes basado en audiencias.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Journey Optimizer], vea <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Crear una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de ejecución de mensaje]</td> 
   <td>Introduzca o asigne el ID de la ejecución del mensaje que desea comprobar.</td> 
  </tr> 
 </tbody> 
</table>

### Comprobaciones de estado

<!--* [Check service health](#check-service-health)-->
* [Compruebe las dependencias de importación](#check-the-import-dependencies)
* [Comprobación del estado de un trabajo de importación](#check-the-status-of-an-import-job)

<!--

#### Check service health

This action module checks that the service represented by the connection is running.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td> 
  </tr> 
 </tbody> 
</table>

-->

#### Compruebe las dependencias de importación

Este módulo de acción comprueba las dependencias de los artefactos del paquete. Esto le permite comprobar si tiene permisos para importar artefactos del paquete.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Journey Optimizer], vea <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Crear una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de paquete]</td> 
   <td>Introduzca o asigne el ID del paquete para el que desea comprobar los permisos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entorno de pruebas de destino]</td> 
   <td>Introduzca o asigne el nombre de la zona protegida en la que desea importar el paquete.</td> 
  </tr> 
 </tbody> 
</table>

#### Comprobación del estado de un trabajo de importación

Este módulo de acción comprueba si un trabajo de importación se ha realizado correctamente o no.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Journey Optimizer], vea <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Crear una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de trabajo]</td> 
   <td>Introduzca o asigne el ID del trabajo para el que desea recuperar datos.</td> 
  </tr> 
 </tbody> 
</table>

### Búsquedas

* [Mostrar todos los objetos dependientes](#list-all-dependent-objects)
* [Enumerar configuraciones](#list-configurations)
* [Enumeración de trabajos de exportación e importación](#list-export-and-import-jobs)
* [Enumeración de paquetes](#list-packages)
* [Enumeración de registros](#list-records)

#### Mostrar todos los objetos dependientes

Este módulo de búsqueda enumera todos los objetos dependientes de los objetos del paquete especificado

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Journey Optimizer], vea <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Crear una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Objetos de paquete]</td> 
   <td>Para cada objeto del paquete para el que desee devolver un objeto dependiente, haga clic en <b>Agregar objeto</b> e introduzca el nombre y el tipo del objeto.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de paquete]</td> 
   <td>Introduzca o asigne el ID del paquete para el que desea enumerar los objetos dependientes.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL Entorno de pruebas de destino]</td> 
   <td>Introduzca o asigne el nombre de la zona protegida que contiene el paquete para el que desea enumerar los objetos dependientes.</td> 
  </tr> 
 </tbody> 
</table>

#### Enumerar configuraciones

Este módulo de acción enumera todas las configuraciones de límite o restricción.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Journey Optimizer], vea <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Crear una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seleccionar tipo de configuración]</td> 
   <td>Seleccione si desea enumerar las configuraciones de límite o de restricción.</td> 
  </tr> 
 </tbody> 
</table>

#### Enumeración de trabajos de exportación e importación

Este módulo de búsqueda enumera los trabajos actuales de exportación e importación. Puede utilizar parámetros de consulta para filtrar la lista.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Journey Optimizer], vea <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Crear una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Iniciar]</td> 
   <td></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de resultados devueltos]</td> 
      <td>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordenar por]</td> 
      <td>Seleccione si desea ordenar los resultados por fecha de creación o de modificación.</td>
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL Parámetro de consulta]</td> 
   <td>Para cada parámetro de consulta por el que desee filtrar, haga clic en <b>Agregar parámetro de consulta</b>, seleccione el campo y el operador e introduzca el valor de campo para el filtro.</td> 
  </tr> 
 </tbody> 
</table>



#### Enumeración de paquetes

Este módulo de búsqueda enumera todos los paquetes de la organización. Puede utilizar parámetros de consulta para filtrar la lista.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Journey Optimizer], vea <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Crear una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Iniciar]</td> 
   <td></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de resultados devueltos]</td> 
      <td>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordenar por]</td> 
      <td>Seleccione si desea ordenar los resultados por fecha de creación o de modificación.</td>
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL Parámetro de consulta]</td> 
   <td>Para cada parámetro de consulta por el que desee filtrar, haga clic en <b>Agregar parámetro de consulta</b>, seleccione el campo y el operador e introduzca el valor de campo para el filtro.</td> 
  </tr> 
 </tbody> 
</table>

#### Enumeración de registros

Este módulo de búsqueda enumera todas las configuraciones de límite o restricción.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Journey Optimizer], vea <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Crear una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seleccionar tipo de contenido]</td> 
   <td>Seleccione si va a recuperar una plantilla de contenido o un fragmento de contenido.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordenar por]</td> 
   <td>Introduzca o asigne el nombre del parámetro por el que desea ordenar esta lista. Agregue <code>-</code> o <code>+</code> para ordenar de forma descendente o ascendente. Si no se especifica ningún signo, la lista se ordena en sentido de bajada.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Iniciar]</td> 
   <td>Este campo se utiliza para la paginación. Introduzca o asigne los criterios de la página siguiente con respecto a la propiedad especificada en el campo Ordenar por.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordenar por]</td> 
   <td>Introduzca o asigne el nombre del parámetro por el que desea ordenar esta lista. Agregue <code>-</code> o <code>+</code> para ordenar de forma descendente o ascendente. Si no se especifica ningún signo, la lista se ordena en sentido de bajada.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtrar por propiedad]</td> 
   <td>Para cada filtro de propiedad que desee agregar, haga clic en <b>Agregar elemento</b> e introduzca la clave y el valor de la propiedad. Los registros que incluyen el valor especificado para la propiedad se incluyen en la lista.</td> 
  </tr> 
 </tbody> 
</table>


### Otro


#### Realizar una llamada de API personalizada

Este módulo de acción realiza una llamada de API personalizada a la API de Adobe Journey Optimizer.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Journey Optimizer], vea <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Crear una conexión con [!DNL Adobe Journey Optimizer]</a> en este artículo.</td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Introduzca una ruta relativa a la dirección URL base.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Método]</p>
      </td>
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada de API. Para obtener más información, vea <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Encabezados]</td>
      <td>
        <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p>
        <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] agrega automáticamente encabezados authorization, <code>x-api-key</code> y <code>x-gw-ims-org-id</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Cadena de consulta]  </td>
      <td>
        <p>Introduzca la cadena de consulta de solicitud.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Cuerpo]</td>
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Cuando utilice afirmaciones condicionales como <code>if</code> en su JSON, coloque las comillas fuera de la afirmación condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>







<!--

* [Check if configuration can be deployed](#check-if-configuration-can-be-deployed)
* [Check service health](#check-service-health)
* [Check the import dependencies](#check-the-import-dependencies)
* [Check the status for audience-based message](#status-for-audience-based-message)
* [Copy artifacts synchronously](#copy-artifacts-synchronously)
* [Create a configuration](#create-a-configuration)
* [Create a package](#create-a-package)
* [Create a record](#create-a-record)
* [Delete a configuration](#delete-a-configuration)
* [Delete a package](#delete-a-package)
* [Delete a record](#delete-a-record)
* [Deploy a configuration](#deploy-a-configuration)
* [Export artifacts asynchronously](#export-artifacts-asynchronously)
* [Get a configuration](#get-a-configuration)
* [Get a record](#get-a-record)
* [Import a package](#import-a-package)
* [Import artifacts asynchronously](#import-artifacts-asynchronously)
* [List all dependent objects](#list-all-dependent-objects)
* [List export and import jobs](#list-import-and-export-jobs)
* [Look up a package](#look-up-a-package)
* [Make a custom API call](#make-a-custom-api-call)
* [Patch a record](#patch-a-record)
* [Publish a package](#publish-a-package)
* [Submit an import](#submit-an-import)
* [Trigger a unitary message execution](#trigger-a-unitary-message-execution)
* [Trigger an audience-based message](#trigger-an-audience-based-message)
* [Undeploy a configuration](#undeploy-a-configuration)
* [Update a configuration](#update-a-configuration)
* [Update a package](#update-a-package)
* [Update a record](#update-a-record)
* [List configurations](#list-configurations)
* [List packages](#list-packages)
* [List records](#list-records)

-->
