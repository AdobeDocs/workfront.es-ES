---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Módulos de almacén de datos
description: Un almacén de datos  [!DNL Adobe Workfront Fusion] similar a una base de datos o tabla simple, puede almacenar datos de escenarios, lo que permite transferir datos entre escenarios individuales o ejecuciones de escenarios. Puede utilizar un almacén de datos para almacenar nuevos datos de varios sistemas durante la sincronización.
author: Becky
feature: Workfront Fusion
exl-id: 1dc9cb88-d1b9-4a67-91fb-be980cc1ccd1
source-git-commit: c51169c18bef8ac8126a04c08deb88d830517b0b
workflow-type: tm+mt
source-wordcount: '1164'
ht-degree: 0%

---

# [!UICONTROL Módulos del almacén de datos]

Un almacén de datos [!DNL Adobe Workfront Fusion], similar a una base de datos o tabla simple, puede almacenar datos de escenarios, lo que permite transferir datos entre escenarios individuales o ejecuciones de escenarios. Puede utilizar un almacén de datos para almacenar nuevos datos de varios sistemas durante la sincronización.

Los módulos del almacén de datos permiten agregar, reemplazar, actualizar, recuperar, eliminar, buscar o contar registros en el almacén de datos de [!DNL Adobe Workfront Fusion].

Para obtener información sobre cómo crear, editar y solucionar problemas de almacenes de datos, consulte [Almacenes de datos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

Para ver un vídeo introductorio a los almacenes de datos de Workfront Fusion, consulte:

* [Almacenes de datos](https://video.tv.adobe.com/v/3427029/){target=_blank}

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
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo], [!UICONTROL [!DNL Workfront Fusion] para automatización de trabajo]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
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

Para usar módulos de [!UICONTROL Almacén de datos], primero debe crear un almacén de datos.

Para obtener información sobre la creación de almacenes de datos, consulte [Almacenes de datos en [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

## [!UICONTROL Almacén de datos] módulos y sus campos

Al configurar los módulos del almacén de datos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto a estos, pueden mostrarse campos de almacén de datos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, vea [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

Todos los módulos de [!UICONTROL Almacén de datos] son módulos de tipo acción.

* [Agregar o reemplazar un registro](#addreplace-a-record)
* [Actualizar un registro](#update-a-record)
* [Obtener un registro](#get-a-record)
* [Comprobar la existencia de un registro](#check-the-existence-of-a-record)
* [Eliminar un registro](#delete-a-record)
* [Eliminar todos los registros](#delete-all-records)
* [Buscar registros](#search-records)
* [Contar registros](#count-records)

### [!UICONTROL Agregar o reemplazar un registro]

Este módulo de acción agrega o reemplaza un registro.

Especifique el almacén de datos y la clave del registro.

El módulo devuelve el ID del registro y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

>[!NOTE]
>
>El módulo genera un error cuando intenta agregar el registro que ya está en el almacén de datos con el mismo nombre y la opción [!UICONTROL Sobrescribir un registro existente] está deshabilitada.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Almacén de datos]</td> 
   <td> <p> Seleccione o agregue el almacén de datos en el que desea crear un registro. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>Introduzca la clave única del registro que desea que el módulo agregue o reemplace. La clave se puede utilizar más adelante para recuperar el registro. Si deja este campo en blanco, se genera una clave automáticamente.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sobrescribir un registro existente] </td> 
   <td> <p>Active esta opción para sobrescribir el registro. El registro que desea sobrescribir debe especificarse en el campo Clave anterior.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Registro] </td> 
   <td> <p>Introduzca los valores deseados en los campos del registro.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Actualizar un registro]

Este módulo de acción actualiza un registro.

Especifique el almacén de datos y la clave del registro.

El módulo devuelve el ID del registro y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Almacén de datos]</td> 
   <td> <p> Seleccione o agregue el almacén de datos en el que desea crear un registro. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>Introduzca la clave única del registro que desea que actualice el módulo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Insertar registro que falta] </td> 
   <td> <p>Active esta opción para crear un nuevo registro si el registro con la clave especificada no existe todavía.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Registro]</td> 
   <td> <p> Introduzca los valores deseados en los campos del registro que desee actualizar.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Obtener un registro]

Este módulo de acción recupera un registro.

Especifique el almacén de datos y la clave del registro.

El módulo devuelve el ID del registro y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Almacén de datos]</td> 
   <td> <p> Seleccione el almacén de datos desde el que desea recuperar un registro</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>Introduzca la clave única del registro que desea que recupere el módulo.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Comprobar la existencia de un registro]

Este módulo de acción especifica si existe un registro en particular.

Especifique el almacén de datos y la clave del registro.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Almacén de datos] </td> 
   <td> <p>Seleccione el almacén de datos en el que desea comprobar la existencia del registro.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>Introduzca la clave única del registro que desea que el módulo compruebe si existe.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Eliminar un registro]

Este módulo de acción elimina un registro.

Especifique el almacén de datos y la clave del registro.

El módulo devuelve el ID del registro y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Almacén de datos] </td> 
   <td> <p>Seleccione el almacén de datos en el que desea comprobar la existencia del registro.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>Introduzca la clave única del registro que desea que elimine el módulo.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Eliminar todos los registros]

Este módulo de acción elimina todos los registros de un almacén de datos concreto.

Usted especifica el almacén de datos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Almacén de datos] </td> 
   <td> <p>Seleccione el almacén de datos del que desea eliminar todos los registros.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Registros de búsqueda]

Este módulo de búsqueda busca registros en un objeto del almacén de datos que coincidan con la consulta de búsqueda especificada.

Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Almacén de datos]</td> 
   <td> <p> Seleccione el almacén de datos que desea buscar.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Filtro]</p> </td> 
   <td> <p>Establezca el filtro para la búsqueda.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Ordenar]</p> </td> 
   <td> <p style="font-weight: normal;">Para cada campo por el que desee ordenar, rellene los campos siguientes:</p> <p style="font-weight: bold;">[!UICONTROL Key]</p> <p>Seleccione el nombre de columna por el que desea ordenar los resultados.</p> <p style="font-weight: bold;">[!UICONTROL Pedido]</p> <p>Seleccione si desea ordenar los resultados en orden ascendente o descendente.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Límite]</td> 
   <td> <p> Establezca el número máximo de resultados de búsqueda que devuelve [!DNL Workfront Fusion] durante un ciclo de ejecución.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Continuar la ejecución de la ruta aunque el módulo no devuelva resultados]</td> 
   <td> <p> Si está habilitado, la ruta de la que forma parte este módulo continúa procesándose aunque no devuelva resultados.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Contar registros]

Este módulo de acción numera los registros de un almacén de datos.

Usted especifica el almacén de datos.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Almacén de datos] </td> 
   <td> <p>Seleccione el almacén de datos que contiene los registros que desea contar.</p> </td> 
  </tr> 
 </tbody> 
</table>
