---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Añadir un filtro a un escenario en [!DNL Adobe] Workfront Fusion
description: En algunos casos, solo debe trabajar con paquetes que cumplan criterios específicos. Los filtros le permiten seleccionar esos paquetes.
author: Becky
feature: Workfront Fusion
exl-id: 114ab37f-71e0-494e-9f3d-93ff5a9d13ba
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 0%

---

# Añadir un filtro a un escenario en [!DNL Adobe Workfront Fusion]

En algunos casos, solo debe trabajar con paquetes que cumplan criterios específicos. Los filtros le permiten seleccionar esos paquetes.

<!--

For example, you could create a scenario with the [!UICONTROL Watch records] trigger for [!DNL Salesforce] to capture only records containing a specific word written by a specific author.

-->

Puede añadir un filtro entre dos módulos y comprobar si los paquetes recibidos de los módulos anteriores cumplen determinadas condiciones de filtro:

* Si lo hacen, los paquetes pasan al siguiente módulo en el escenario.
* Si no lo hacen, termina el procesamiento de los paquetes.

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
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p><p>[!UICONTROL [!DNL Workfront Fusion] para la automatización del trabajo] </p>  </td>    </tr> 
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

Debe añadir ambos módulos a un escenario para poder agregar un filtro entre ellos.

## Añadir un filtro entre dos módulos:

1. Haga clic en **[!UICONTROL Situaciones]** ![](assets/scenarios-icon.png) en el panel izquierdo, seleccione el escenario para abrirlo.
1. En la esquina superior derecha de la ventana, haga clic en **[!UICONTROL Editar]**.
1. Haga clic en la línea de conexión entre los módulos.
1. En el cuadro que aparece, escriba un **[!UICONTROL Etiqueta]** para el filtro .
1. Definir un filtro **[!UICONTROL Condición]**.

   Puede introducir uno o dos operandos en los dos cuadros. Si introduce operandos en ambos cuadros, puede seleccionar un operador en el menú desplegable entre ellos para especificar la relación entre ellos.

   >[!TIP]
   >
   >En los campos del operando, puede introducir valores del mismo modo que lo haría para asignarlos, tal como se describe en [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

   Por ejemplo, si desea que el filtro busque archivos en [!DNL Adobe Workfront] terminar con XML y pasarlos a [!DNL Dropbox], debe introducir **[!UICONTROL Nombre del archivo]** en el primer cuadro y .**[!UICONTROL xml]** en la segunda casilla. En el menú desplegable entre ellos, debe seleccionar **[!UICONTROL Finaliza con (sin distinción de mayúsculas y minúsculas)]**. Este filtro se aplicaría a los paquetes entrantes del primer módulo (Workfront). Solo los paquetes que contienen archivos XML se pasarían al siguiente módulo ([!DNL Dropbox]).

   ![](assets/set-up-filter-box-350x368.jpg)

1. Haga clic **[!DNL OK]**.

## Copiar un filtro

Actualmente, el editor de escenarios no incluye una función para copiar un filtro.

>[!NOTE]
>
>Si copia los módulos en cualquier lado del filtro, también se copia el filtro.
>
>Para obtener más información sobre cómo copiar módulos, consulte [Copiar módulos o escenarios en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md)

Para copiar un filtro sin copiar módulos, puede utilizar [!DNL Google] Chrome para la siguiente solución:

1. Instale el [!UICONTROL [!DNL Adobe Workfront Fusion] DevTool Chrome] extensión.
1. En [!DNL Workfront Fusion], abra el escenario.
1. Haga clic en el menú de tres puntos de Chrome y, a continuación, haga clic en **[!UICONTROL Más herramientas*]* > **[!UICONTROL Herramientas para desarrolladores]**.

1. En el [!UICONTROL Herramientas para desarrolladores] que se muestra, en la barra de menús de la parte superior, haga clic en el [!UICONTROL Workfront Fusion] pestaña .

   ![](assets/copy-a-filter-350x174.png)

1. Haga clic en el **[!UICONTROL Herramientas]** icono ![](assets/devtools-tools-icon.png) en la barra izquierda.

1. Haga clic en **[!UICONTROL Copiar filtro]** y, a continuación, configure la variable **[!UICONTROL Copiar filtro]** herramienta en el panel lateral derecho:

   1. Configure las variables **[!UICONTROL Módulo de origen]** como módulo justo después del filtro que desea copiar.
   1. Configure las variables **[!UICONTROL Módulo de Target]** como módulo justo antes del filtro que desea copiar.

1. Haga clic en **[!UICONTROL Ejecutar]**.
