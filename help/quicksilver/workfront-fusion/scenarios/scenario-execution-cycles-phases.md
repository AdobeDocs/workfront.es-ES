---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Ejecución de escenarios, ciclos y fases en  [!DNL Adobe Workfront Fusion]
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 5403f476-226d-4268-affc-8e06b1117684
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 87%

---

# Ejecución de escenarios, ciclos y fases en [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Ejecución de escenarios, ciclos y fases](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/scenarios/scenario-execution-cycles-phases.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

[!DNL Adobe Workfront Fusion] es un sistema transaccional, similar a las bases de datos relacionales. Cada ejecución de escenario comienza con la fase de inicialización, continúa con al menos un ciclo compuesto por las fases de operación y compromiso/reversión, y finaliza con la fase de finalización:

>[!INFO]
>
>**Ejemplo**
>
>Inicialización
>
>Ciclo núm. 1
>
>Operación (lectura o escritura)
>
>Confirmar o revertir
>
>Ciclo núm. 2
>
>Operación (lectura o escritura)
>
>Confirmar o revertir
>
>...
>
>Ciclo núm. N
>
>Operación (lectura o escritura)
>
>Confirmar o revertir
>
>Finalización

## Requisitos de acceso

Para utilizar la funcionalidad de este artículo debe tener el siguiente acceso:

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
   <td role="rowheader">Licencia** de [!UICONTROL Adobe Workfront Fusion]</td> 
  <td>
   <p>Requisito de licencia actual: no se requiere la licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Producto</td> 
   <td>
   <p>Requisito de producto actual: si tiene el plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] su organización debe adquirir [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en el plan [!DNL Workfront] de [!UICONTROL Ultimate].</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] y [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Inicialización

Durante la fase de inicialización, se crean todas las conexiones necesarias (conexión a una base de datos, servicio de correo electrónico, etc.). También se comprueban si cada módulo es capaz de realizar las operaciones previstas.

## Ciclos

Cada ciclo representa una unidad de trabajo indivisible compuesta por una serie de operaciones. Es posible establecer el número máximo de ciclos en el panel [!UICONTROL Configuración del escenario]. El número predeterminado es 1.

Para obtener más información, consulte [El panel de configuración del escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Operación

Durante la fase de operación se realiza la operación de lectura y/o escritura:

* La operación de lectura consiste en obtener datos de un servicio que luego procesan otros módulos de acuerdo con un escenario predefinido. Por ejemplo, el módulo [!UICONTROL Dropbox] >[!UICONTROL Ver archivos] devuelve nuevos paquetes (archivos) creados desde la última ejecución del escenario.
* La operación de escritura consiste en enviar datos a un servicio determinado para un procesamiento posterior. Por ejemplo, el módulo [!DNL Dropbox] >[!UICONTROL Subir un archivo] sube un archivo a una carpeta de [!DNL Dropbox].

## Confirmar

Si la fase de operación es correcta para todos los módulos, comienza la fase de confirmación durante la cual se confirman todas las operaciones realizadas por los módulos. Esto significa que [!DNL Workfront Fusion] envía información a todos los servicios involucrados en la fase de operación sobre su éxito.

## Reversión

Si se produce un error durante la fase de operación o confirmación en cualquier módulo, la fase se anula y se inicia la fase de reversión, lo que anula todas las operaciones durante el ciclo determinado. Algunos módulos no admiten la reversión y las operaciones realizadas por estos módulos no se pueden recuperar. Para obtener más información, consulte la sección [Módulos ACID](#acid-modules).

## Finalización

Durante la fase de finalización, las conexiones abiertas (por ejemplo, conexiones FTP, conexiones de base de datos, etc.) se cierran y se completa el escenario.

## Módulos ACID

Todos los módulos de [!DNL Workfront Fusion] que admiten la reversión (también conocida como transaccionalidad) están marcados con la etiqueta ACID.

![](assets/acid-modules-350x189.png)

Los módulos no marcados con esta etiqueta no se pueden revertir a su estado inicial cuando se producen errores en otros módulos. Un ejemplo típico de un módulo que no es ACID es la acción [!UICONTROL Email] >[!UICONTROL Send an Email]. Una vez enviado el correo electrónico, no se puede deshacer el envío.
