---
product-area: projects
navigation-topic: financials
title: Establecer el método de índice de rendimiento (PIM)
description: El método de índice de rendimiento (PIM) del proyecto controla el método que utiliza Adobe Workfront para calcular las métricas de rendimiento del proyecto como el Índice de rendimiento de costes (CPI), el Índice de rendimiento de programación de costes (CSI), el Índice de rendimiento de la programación (SPI) y la Estimación al finalizar (EAC).
author: Lisa
feature: Work Management
exl-id: de628881-c016-4521-bc33-3bcfba19a88f
TQID: https://experienceleague.adobe.com/g4FYe8k1psS9xuL6Z40teAyJ-SV4UD6ThnWvnvl8au4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 418
ht-degree: 97%

---

# Establecer el método de índice de rendimiento (PIM)

El método de índice de rendimiento (PIM) del proyecto controla el método que utiliza Adobe Workfront para calcular las métricas de rendimiento del proyecto como el Índice de rendimiento de costes (CPI), el Índice de rendimiento de programación de costes (CSI), el Índice de rendimiento de la programación (SPI) y la Estimación al finalizar (EAC).

Workfront calcula estos valores mediante:

* Horas
* Coste

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Paquete de Adobe Workfront</td> 
   <td>Cualquiera </td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td>
   <p>Estándar</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>Acceso de edición a proyectos y datos financieros</td> 
  </tr> 
  <tr> 
   <td>Permisos de objeto</td> 
   <td>Administrar permisos del proyecto con permisos para Editar finanzas generales</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones sobre PIM en Workfront

* El administrador de Workfront o de grupos configuran el ajuste predeterminado si el método de índice de rendimiento (PIM) debe basarse en horas o en costes. Los cálculos de las métricas de rendimiento cambian según la configuración de este ajuste predeterminado. Para obtener más información sobre cómo cambiar el ajuste predeterminado para calcular el PIM, consulte [Configurar las preferencias de proyecto en todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Los administradores de proyecto también pueden cambiar la configuración del PIM, en el nivel de proyecto, para proyectos individuales en la subpestaña Finanzas del proyecto. Debe tener permisos de administración en el proyecto para editar la subpestaña Finanzas del proyecto.

## Establecer el método de índice de rendimiento (PIM) para un proyecto

1. Vaya a un proyecto del que sea propietario.

   >[!IMPORTANT]
   >
   >Necesita permisos de administración en el proyecto para realizar los siguientes pasos. También recomendamos que el propietario del proyecto sea el único que realice cambios en el área de Finanzas del proyecto.

1. Haga clic en **Detalles del proyecto** en el panel izquierdo y, a continuación, vaya al área de **Finanzas**.
1. Haga doble clic en el valor del campo **Método de índice de rendimiento** para editarlo.
1. Seleccione entre las siguientes opciones del campo **Método de índice de rendimiento**:

   | Basado en horas | Workfront utiliza las horas planificadas para calcular el CPI y el EAC del proyecto, y el EAC del proyecto se muestra como un número, en horas. |
   |---|---|
   | Basado en costes | Workfront utiliza el coste planificado de mano de obra para calcular el CPI y el EAC del proyecto, y el EAC se muestra como un valor de moneda. Al seleccionar esta opción, asegúrese de que los destinatarios de la tarea (funciones o usuarios) estén asociados con las tasas de coste. |

   {style="table-layout:auto"}

1. Haga clic en **Guardar** **cambios**.
