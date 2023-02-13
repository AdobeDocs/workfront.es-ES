---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Módulos de almacenamiento de datos
description: Un [!DNL Adobe Workfront Fusion] el almacén de datos, similar a una base de datos o a una tabla sencilla, puede almacenar datos de escenarios, lo que permite transferir datos entre escenarios o ejecuciones de escenarios individuales. Puede utilizar un almacén de datos para almacenar nuevos datos de varios sistemas durante la sincronización.
author: Becky
feature: Workfront Fusion
exl-id: 1dc9cb88-d1b9-4a67-91fb-be980cc1ccd1
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1103'
ht-degree: 0%

---

# [!UICONTROL Almacén de datos] módulos

Un [!DNL Adobe Workfront Fusion] el almacén de datos, similar a una base de datos o a una tabla sencilla, puede almacenar datos de escenarios, lo que permite transferir datos entre escenarios o ejecuciones de escenarios individuales. Puede utilizar un almacén de datos para almacenar nuevos datos de varios sistemas durante la sincronización.

Los módulos del almacén de datos le permiten agregar, reemplazar, actualizar, recuperar, eliminar, buscar o contar registros en su [!DNL Adobe Workfront Fusion] almacén de datos.

Para obtener información sobre la creación, edición y solución de problemas de almacenes de datos, consulte [Almacenes de datos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p>  <p>[!UICONTROL [!DNL Workfront Fusion] para la automatización del trabajo]</p></td> 
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

Para usar [!UICONTROL Almacén de datos] , primero debe crear un almacén de datos.

Para obtener información sobre la creación de almacenes de datos, consulte [Almacenes de datos en [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

## [!UICONTROL Almacén de datos] módulos y sus campos

Al configurar los módulos del almacén de datos, [!DNL Workfront Fusion] muestra los campos que se enumeran a continuación. Junto con estos, podrían mostrarse campos adicionales del almacén de datos, según factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón de asignación encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

Todo [!UICONTROL Almacén de datos] son módulos de tipo Action .

* [Agregar o reemplazar un registro](#addreplace-a-record)
* [Actualizar un registro](#update-a-record)
* [Obtener un registro](#get-a-record)
* [Comprobar la existencia de un registro](#check-the-existence-of-a-record)
* [Eliminar un registro](#delete-a-record)
* [Eliminar todos los registros](#delete-all-records)
* [Registros de búsqueda](#search-records)
* [Recuento de registros](#count-records)

### [!UICONTROL Agregar o reemplazar un registro]

Este módulo de acción agrega o reemplaza un registro.

Se especifica el almacén de datos y la clave del registro.

El módulo devuelve el ID del registro y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

>[!NOTE]
>
>El módulo genera un error al intentar añadir el registro que ya se encuentra en el almacén de datos con el mismo nombre y la variable [!UICONTROL Sobrescribir un registro existente] está desactivada.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store]</td> 
   <td> <p> Seleccione o agregue el almacén de datos donde desea crear un registro. </p> </td> 
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
   <td>[!UICONTROL Record] </td> 
   <td> <p>Introduzca los valores deseados en los campos del registro.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Actualizar un registro]

Este módulo de acción actualiza un registro.

Se especifica el almacén de datos y la clave del registro.

El módulo devuelve el ID del registro y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store]</td> 
   <td> <p> Seleccione o agregue el almacén de datos donde desea crear un registro. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>Introduzca la clave única del registro que desea que actualice el módulo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Insertar registro que falta] </td> 
   <td> <p>Active esta opción para crear un nuevo registro si el registro con la clave especificada no existe.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record]</td> 
   <td> <p> Introduzca los valores deseados en los campos del registro que desea actualizar.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Obtener un registro]

Este módulo de acción recupera un registro.

Se especifica el almacén de datos y la clave del registro.

El módulo devuelve el ID del registro y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store]</td> 
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

Se especifica el almacén de datos y la clave del registro.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store] </td> 
   <td> <p>Seleccione el almacén de datos que desea comprobar para comprobar la existencia del registro.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>Introduzca la clave única del registro que desea que el módulo compruebe si existe.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Eliminar un registro]

Este módulo de acción elimina un registro.

Se especifica el almacén de datos y la clave del registro.

El módulo devuelve el ID del registro y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store] </td> 
   <td> <p>Seleccione el almacén de datos que desea comprobar para comprobar la existencia del registro.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>Introduzca la clave única del registro que desea que elimine el módulo.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Eliminar todos los registros]

Este módulo de acción elimina todos los registros de un almacén de datos en particular.

El almacén de datos se especifica.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store] </td> 
   <td> <p>Seleccione el almacén de datos desde el que desea eliminar todos los registros.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Registros de búsqueda]

Este módulo de búsqueda busca registros en un objeto del almacén de datos que coincidan con la consulta de búsqueda especificada.

Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store]</td> 
   <td> <p> Seleccione el almacén de datos que desea buscar.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Filtro]</p> </td> 
   <td> <p>Establezca el filtro para la búsqueda.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Sort]</p> </td> 
   <td> <p style="font-weight: normal;">Para cada campo por el que desee ordenar, rellene los siguientes campos:</p> <p style="font-weight: bold;">[!UICONTROL Key]</p> <p>Seleccione el nombre de columna por el que desea ordenar los resultados.</p> <p style="font-weight: bold;">[!UICONTROL Order]</p> <p>Seleccione si desea ordenar los resultados en orden ascendente o descendente.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Límite]</td> 
   <td> <p> Configurar el número máximo de resultados de búsqueda [!DNL Workfront Fusion] vuelve durante un ciclo de ejecución.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Continúe con la ejecución de la ruta aunque el módulo no devuelva ningún resultado]</td> 
   <td> <p> Si está habilitado, la ruta de la que forma parte este módulo continúa procesándose aunque este módulo no devuelva ningún resultado.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Recuento de registros]

Este módulo de acción enumera los registros de un almacén de datos.

El almacén de datos se especifica.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store] </td> 
   <td> <p>Seleccione el almacén de datos que contiene los registros que desea contar.</p> </td> 
  </tr> 
 </tbody> 
</table>
