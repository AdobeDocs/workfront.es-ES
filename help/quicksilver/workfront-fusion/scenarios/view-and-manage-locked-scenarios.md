---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Administrar escenarios bloqueados en  [!DNL Adobe Workfront Fusion]
description: Administrar escenarios bloqueados en  [!DNL Adobe Workfront Fusion]
author: Becky
feature: Workfront Fusion
exl-id: 5fccf336-d904-43fe-ad4a-c3ce76dbcad0
source-git-commit: abb021a6857f8016d4f8b6bcf99fe818e47faea6
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---

# Administrar escenarios bloqueados en [!DNL Adobe Workfront Fusion]

En algunos casos, un escenario podría estar bloqueado temporalmente en [!DNL Workfront Fusion]. Las ejecuciones bloqueadas se desbloquearán automáticamente en un plazo de 2 a 4 horas. También puede desbloquear escenarios manualmente.

>[!IMPORTANT]
>
>Desbloquear manualmente un escenario puede provocar errores en las ejecuciones de un escenario.

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
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p><p>[!UICONTROL [!DNL Workfront Fusion] para automatización de trabajo] </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para usar la funcionalidad descrita en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Explicación de los escenarios bloqueados

Los escenarios pueden estar bloqueados por varios motivos.

Workfront Fusion no admite el procesamiento paralelo de escenarios programados. Estos escenarios se bloquean al principio de la ejecución del escenario y se desbloquean cuando se completa. Si se interrumpe la ejecución, es posible que el escenario no se desbloquee. Esto puede ocurrir cuando un usuario detiene manualmente el escenario o cuando hay un problema con el sistema.

Además, el equipo de ingeniería de Workfront Fusion puede bloquear un escenario porque está causando problemas de rendimiento u otros problemas.

Independientemente de la causa de un escenario bloqueado, este se desbloqueará automáticamente entre 2 y 4 horas después de bloquearlo.

## Desbloquear un escenario bloqueado

Los escenarios bloqueados se desbloquearán de 2 a 4 horas desde el momento en que se bloquearon. Puede desbloquear un escenario manualmente antes de programarlo para que se desbloquee automáticamente.

Desbloquear manualmente un escenario puede provocar errores en las ejecuciones de un escenario. Se recomienda desbloquear escenarios manualmente solo cuando un escenario esté bloqueado debido a la ejecución y detención de ejecuciones como parte del diseño del escenario. En otras circunstancias, se recomienda esperar a que el escenario se desbloquee automáticamente.

>[!IMPORTANT]
>
>Desbloquear manualmente un escenario puede provocar errores en las ejecuciones de un escenario.

1. Vaya a la página de detalles del escenario del escenario bloqueado.
1. Haga clic en **[!UICONTROL Opciones]** en la esquina superior derecha de la pantalla.
1. Seleccione **[!UICONTROL Desbloquear ejecución]**.
1. Haga clic en **[!UICONTROL Desbloquear]**.
