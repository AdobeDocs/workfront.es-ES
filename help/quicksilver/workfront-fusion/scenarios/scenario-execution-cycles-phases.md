---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Ejecución del escenario, ciclos y fases en [!DNL Adobe Workfront Fusion]
description: Este artículo describe los eventos que se producen durante la [!DNL Adobe Workfront Fusion] se está ejecutando, como inicialización, operaciones, confirmaciones y devoluciones.
author: Becky
feature: Workfront Fusion
exl-id: 5403f476-226d-4268-affc-8e06b1117684
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---

# Ejecución del escenario, ciclos y fases en [!DNL Adobe Workfront Fusion]

[!DNL Adobe Workfront Fusion] es un sistema transaccional, similar a las bases de datos relacionales. Cada ejecución de escenario comienza con la fase de inicialización, continúa con al menos un ciclo compuesto por las fases de operación y confirmación/reversión, y finaliza con la fase de finalización:

>[!INFO]
>
>**Ejemplo**
>
>Inicialización
>
>Ciclo 1
>
>Funcionamiento (lectura o escritura)
>
>Confirmar o revertir
>
>Ciclo 2
>
>Funcionamiento (lectura o escritura)
>
>Confirmar o revertir
>
>...
>
>Ciclo N
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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de [!UICONTROL Adobe Workfront Fusion**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p><p>[!UICONTROL [!DNL Workfront Fusion] para la automatización del trabajo] </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Inicialización

Durante la fase de inicialización, se crean todas las conexiones necesarias (conexión a una base de datos, servicio de correo electrónico, etc.). También se verifican si cada módulo es capaz de realizar las operaciones deseadas.

## Ciclos

Cada ciclo representa una unidad de trabajo indivisible compuesta por una serie de operaciones. Es posible establecer el número máximo de ciclos en la variable [!UICONTROL configuración de escenario] panel. El número predeterminado es 1.

Para obtener más información, consulte [El panel de configuración de escenario de [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Operación

Durante la fase de operación se realiza la lectura y/o escritura:

* La operación de lectura consiste en obtener datos de un servicio que luego otros módulos procesan según un escenario predefinido. Por ejemplo, la variable [!UICONTROL Dropbox] >[!UICONTROL Archivos de Watch] devuelve nuevos paquetes (archivos) creados desde la última ejecución del escenario.
* La operación de escritura consiste en enviar datos a un servicio determinado para un procesamiento posterior. Por ejemplo, la variable [!DNL Dropbox] >[!UICONTROL Cargar un archivo] el módulo carga un archivo en un [!DNL Dropbox] carpeta.

## Confirmar

Si la fase de operación es correcta para todos los módulos, la fase de confirmación comienza durante la cual se confirman todas las operaciones realizadas por los módulos. Esto significa que [!DNL Workfront Fusion] envía información a todos los servicios implicados en la fase de operación sobre su éxito.

## Reversión

Si se produce un error durante la fase de operación o confirmación en cualquier módulo, la fase se anula y se inicia la fase de reversión, lo que anula todas las operaciones durante el ciclo dado. Algunos módulos no admiten la reversión y las operaciones realizadas por estos módulos no se pueden recuperar. Para obtener más información, consulte [Módulos ACID](#acid-modules) para obtener más información.

## Finalización

Durante la fase de finalización, las conexiones abiertas (por ejemplo, conexiones FTP, conexiones de base de datos, etc.) se cierran y se completa el escenario.

## Módulos ACID

Todo [!DNL Workfront Fusion] los módulos compatibles con la reversión (también conocidos como transaccionalidad) se marcan con la etiqueta ACID .

![](assets/acid-modules-350x189.png)

Los módulos que no están marcados con esta etiqueta no se pueden volver a su estado inicial cuando se producen errores en otros módulos. Un ejemplo típico de un módulo que no es ACID es el [!UICONTROL Correo electrónico] >[!UICONTROL Enviar un correo electrónico] acción. Una vez enviado el correo electrónico, no se puede deshacer el envío.
