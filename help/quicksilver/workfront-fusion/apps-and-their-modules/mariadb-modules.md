---
title: Módulos MariaDB
description: En un  [!DNL Adobe Workfront Fusion] escenario, puede automatizar los flujos de trabajo que usan [!DNL MariaDB], así como conectarlo a varias aplicaciones y servicios de terceros.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 45d4d7fe-a70c-4906-adb4-f913a870fe47
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 0%

---

# [!DNL MariaDB] módulos

En un escenario de [!DNL Adobe Workfront Fusion], puede automatizar los flujos de trabajo que utilizan [!DNL MariaDB], así como conectarlo a varias aplicaciones y servicios de terceros.

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

Para usar módulos de [!DNL MariaDB], debe tener una cuenta de [!DNL MariaDB].

## Conectar [!DNL MariaDB] a [!DNL Workfront Fusion]

Puede crear una conexión con su cuenta de [!DNL MariaDB] directamente desde un módulo de [!DNL MariaDB].

1. En cualquier módulo de [!DNL MariaDB], haga clic en **[!UICONTROL Agregar]** junto al campo [!UICONTROL Conexión].
1. Configure los campos siguientes:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Nombre de conexión]</p> </td> 
      <td> <p>Introduzca un nombre para la nueva conexión.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Host]</td> 
      <td> <p>Introduzca la dirección IP o el nombre de host de la instancia de base de datos. Se debe poder acceder a este host desde fuera de la red.</p> <p>Ejemplo: <code>[!DNL mariadb.hwoh2j5h.us-east-1.rds.amazon.com]</code></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Puerto]</td> 
      <td>El puerto predeterminado es 3306. Si utiliza un puerto no estándar, establezca este número en el puerto. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nombre de base de datos]</td> 
      <td>Introduzca el nombre de la base de datos con la que desea interactuar.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nombre de usuario]</td> 
      <td>Escriba su nombre de usuario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Contraseña]</td> 
      <td>Introduzca su contraseña.</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Continuar]** para crear la conexión y volver al módulo.

## [!DNL MariaDB] módulos y sus campos

Al configurar [!DNL MariaDB] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL MariaDB] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, vea [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Ejecución de una consulta (avanzada)

Este módulo de acción recupera información de la base de datos, en función de la consulta proporcionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL MariaDB] a [!DNL Workfront Fusion], vea <a href="#connect-mariadb-to-workfront-fusion" class="MCXref xref">Conectar [!DNL MariaDB] a [!DNL Workfront Fusion]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Consulta]</td> 
   <td> <p>Introduzca la consulta SQL que desea que utilice el módulo para recuperar datos.</p> <p>Importante: Las variables utilizadas en la consulta no se sanean. Asegúrese de sanear las variables correctamente para evitar la inyección de SQL.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Seleccionar filas de una tabla (avanzado)]

Este módulo lee registros de la base de datos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL MariaDB] a [!DNL Workfront Fusion], vea <a href="#connect-mariadb-to-workfront-fusion" class="MCXref xref">Conectar [!DNL MariaDB] a [!DNL Workfront Fusion]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tabla]</td> 
   <td> <p>Seleccione la tabla que contiene los registros que desea leer.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td> <p>Configure el filtro mediante el cual desea seleccionar filas</p> 
    <ul> 
     <li> <p>Seleccione el campo por el que desea buscar</p> </li> 
     <li> <p>Seleccione el operador que desee utilizar para la búsqueda</p> </li> 
     <li> <p>Introduzca o asigne el valor que desea buscar.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordenar] </td> 
   <td> <p>Para cada nivel por el que desee ordenar los resultados, haga clic en <strong>[!UICONTROL Agregar elemento]</strong> y, a continuación, seleccione el campo por el que desea ordenar los resultados y si desea ordenar de forma ascendente o descendente</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>
