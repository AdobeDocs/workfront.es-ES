---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Variables matemáticas en  [!DNL Adobe Workfront Fusion]
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 2fb561d2-0780-4fd6-87b3-5360a02df177
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 62%

---

# Variables matemáticas en [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Variables matemáticas](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/mapping-panel/functions/math-variables.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

<!--Audited: 4/2024-->

## Requisitos de acceso

Para utilizar la funcionalidad de este artículo debe tener el siguiente acceso:

<table style="table-layout:auto"> 
 <col>  
 <col>  
 <tbody>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront] plan</td>  
   <td> <p>Cualquiera</p> </td>  
  </tr>  
  <tr data-mc-conditions="">  
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td>  
   <td> <p>Nuevo: [!UICONTROL Standard]</p><p>O</p><p>Actual: [!UICONTROL Work] o superior</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td>  
   <td> 
   <p>Actual: no se requiere licencia para [!DNL Workfront Fusion].</p> 
   <p>O</p> 
   <p>Heredado: cualquiera </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">Producto</td>  
   <td> 
   <p>Nuevo:</p> <ul><li>Plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Workfront]: su organización debe comprar [!DNL Adobe Workfront Fusion].</li><li>Plan [!UICONTROL Ultimate] [!DNL Workfront]: [!DNL Workfront Fusion] está incluido.</li></ul> 
   <p>O</p> 
   <p>Actual: su organización debe comprar [!DNL Adobe Workfront Fusion].</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Para obtener información sobre las licencias de [!DNL Adobe Workfront Fusion], consulte Licencias de [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## pi

Representa el símbolo matemático $\pi$.

## [!UICONTROL random]

Devuelve un número pseudoaleatorio de coma flotante en el rango [`0`,`1`] (que incluye `0`, pero no `1`).

Utilice la siguiente fórmula para generar un número pseudoaleatorio entero en el rango [`min`,`max`] (que incluye `min` y `max`):

![](assets/math-variable-random-350x61.png)

```
floor(random * (1.max - 1.min + 1)) + 1.min
```
