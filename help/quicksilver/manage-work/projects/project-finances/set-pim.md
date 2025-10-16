---
product-area: projects
navigation-topic: financials
title: Establecer el método de índice de rendimiento (PIM)
description: El método de índice de rendimiento (PIM) del proyecto controla el método que utiliza Adobe Workfront para calcular las métricas de rendimiento del proyecto como el Índice de rendimiento de costes (CPI), el Índice de rendimiento de programación de costes (CSI), el Índice de rendimiento de la programación (SPI) y la Estimación al finalizar (EAC).
author: Lisa
feature: Work Management
exl-id: de628881-c016-4521-bc33-3bcfba19a88f
source-git-commit: 23a4d055871c9138818e70fa1cd936581dbd7552
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 99%

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
   <td>paquete de Adobe Workfront</td> 
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
   <td>Permisos de administración para el proyecto con permisos para administrar finanzas</td> 
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
