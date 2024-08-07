---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Ejecución de escenarios, ciclos y fases en  [!DNL Adobe Workfront Fusion]
description: Este artículo describe los eventos que se producen mientras se ejecuta un  [!DNL Adobe Workfront Fusion] escenario, como la inicialización, las operaciones, las confirmaciones y las reversiones.
author: Becky
feature: Workfront Fusion
exl-id: 5403f476-226d-4268-affc-8e06b1117684
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 0%

---

# Ejecución de escenarios, ciclos y fases en [!DNL Adobe Workfront Fusion]

[!DNL Adobe Workfront Fusion] es un sistema transaccional, similar a las bases de datos relacionales. Cada ejecución de escenario comienza con la fase de inicialización, continúa con al menos un ciclo compuesto por las fases de operación y compromiso/reversión, y finaliza con la fase de finalización:

>[!INFO]
>
>**Ejemplo**
>
>Inicialización
>
>#1 de ciclo
>
>Funcionamiento (lectura o escritura)
>
>Confirmar o revertir
>
>#2 de ciclo
>
>Funcionamiento (lectura o escritura)
>
>Confirmar o revertir
>
>...
>
>#N de ciclo
>
>Funcionamiento (lectura o escritura)
>
>Confirmar o revertir
>
>Finalización

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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de [!UICONTROL Adobe Workfront Fusion]**</td> 
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

## Inicialización

Durante la fase de inicialización, se crean todas las conexiones necesarias (conexión a una base de datos, servicio de correo electrónico, etc.). También se comprueba si cada módulo es capaz de realizar las operaciones previstas.

## Ciclos

Cada ciclo representa una unidad de trabajo indivisible compuesta por una serie de operaciones. Es posible establecer el número máximo de ciclos en el panel [!UICONTROL configuración de escenario]. El número predeterminado es 1.

Para obtener más información, consulte [El panel de configuración de escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Operación

Durante la fase de operación se realiza la operación de lectura y/o escritura:

* La operación de lectura consiste en obtener datos de un servicio que luego procesan otros módulos de acuerdo con un escenario predefinido. Por ejemplo, el módulo [!UICONTROL Dropbox] >[!UICONTROL Observar archivos] devuelve nuevos paquetes (archivos) creados desde la última ejecución del escenario.
* La operación de escritura consiste en enviar datos a un servicio determinado para un procesamiento posterior. Por ejemplo, el módulo [!DNL Dropbox] >[!UICONTROL Cargar un archivo] carga un archivo en una carpeta [!DNL Dropbox].

## Confirmar

Si la fase de operación es correcta para todos los módulos, comienza la fase de confirmación durante la cual se confirman todas las operaciones realizadas por los módulos. Esto significa que [!DNL Workfront Fusion] envía información a todos los servicios involucrados en la fase de operación sobre su éxito.

## Reversión

Si se produce un error durante la fase de operación o confirmación en cualquier módulo, la fase se anula y se inicia la fase de reversión, lo que anula todas las operaciones durante el ciclo determinado. Algunos módulos no admiten la reversión y las operaciones realizadas por estos módulos no se pueden recuperar. Para obtener más información, consulte la sección [Módulos ACID](#acid-modules).

## Finalización

Durante la fase de finalización, las conexiones abiertas (por ejemplo, conexiones FTP, conexiones de base de datos, etc.) se cierran y se completa el escenario.

## módulos ÁCIDOS

Todos los módulos de [!DNL Workfront Fusion] que admiten la reversión (también conocida como transaccionalidad) están marcados con la etiqueta ACID.

![](assets/acid-modules-350x189.png)

Los módulos no marcados con esta etiqueta no se pueden volver a su estado inicial cuando se producen errores en otros módulos. Un ejemplo típico de un módulo que no es ACID es la acción [!UICONTROL Correo electrónico] >[!UICONTROL Enviar un correo electrónico]. Una vez enviado el correo electrónico, no se puede deshacer el envío.
