---
product-area: projects
navigation-topic: financials
title: Definir el método del índice de rendimiento (PIM)
description: El método de índice de rendimiento (PIM) del proyecto controla el método que utiliza Adobe Workfront para calcular las métricas de rendimiento del proyecto, como Índice de rendimiento de costes (CPI), Índice de rendimiento del programa de costes (CSI), Índice de rendimiento del programa (SPI) y Estimación al finalizar (EAC).
author: Alina
feature: Work Management
exl-id: de628881-c016-4521-bc33-3bcfba19a88f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 1%

---

# Definir el método del índice de rendimiento (PIM)

El método de índice de rendimiento (PIM) del proyecto controla el método que utiliza Adobe Workfront para calcular las métricas de rendimiento del proyecto, como Índice de rendimiento de costes (CPI), Índice de rendimiento del programa de costes (CSI), Índice de rendimiento del programa (SPI) y Estimación al finalizar (EAC).

Workfront calcula estos valores mediante lo siguiente:

* Horas
* Costo

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos y Datos Financieros</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administre permisos para el proyecto con permisos para Administrar finanzas</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Consideraciones sobre PIM en Workfront

* El administrador de Workfront o un administrador de grupo configuran el valor predeterminado para si el método de índice de rendimiento (PIM) debe basarse en horas o en costes. Los cálculos de las métricas de rendimiento cambian según la configuración predeterminada. Para obtener más información sobre cómo cambiar el valor predeterminado para calcular el PIM, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Los administradores de proyectos también pueden cambiar la configuración del PIM, a nivel de proyecto, para proyectos individuales en la subpestaña Finanzas del proyecto. Debe tener permisos de administración para editar la subficha Finanzas del proyecto.

## Definir el método de índice de rendimiento (PIM) para un proyecto

1. Vaya a un proyecto del que sea propietario.

   >[!IMPORTANT]
   >
   >Para realizar los siguientes pasos, debe administrar los permisos del proyecto. También recomendamos que solo el propietario del proyecto realice cambios en el área de finanzas del proyecto.

1. Haga clic en **Detalles del proyecto** en el panel izquierdo y, a continuación, vaya a la **Finanzas** .
1. Haga doble clic en el valor de la variable **Método de índice de rendimiento** para editarlo.
1. Seleccione entre las siguientes opciones en la sección **Método de índice de rendimiento** campo:

   | Basado en horas | Workfront utiliza las horas planificadas para calcular el CPI y la CAO del proyecto, y el CAO del proyecto se muestra como un número, en horas. |
   |---|---|
   | Basado en costos | Workfront utiliza el Costo de trabajo planificado para calcular el IPC y la CAO del proyecto, y el EAC se muestra como un valor de moneda. Cuando seleccione esta opción, asegúrese de que los asignadores de tareas (funciones de trabajo o usuarios) estén asociados a tasas de coste. |

   {style=&quot;table-layout:auto&quot;}

1. Haga clic en **Guardar** **Cambios**.
