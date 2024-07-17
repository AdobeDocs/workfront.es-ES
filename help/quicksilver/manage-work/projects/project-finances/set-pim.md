---
product-area: projects
navigation-topic: financials
title: Establecer el método de índice de rendimiento (PIM)
description: El método de índice de rendimiento (PIM) del proyecto controla el método que utiliza Adobe Workfront para calcular métricas de rendimiento del proyecto como el índice de rendimiento de costos (CPI), el índice de rendimiento del horario de costos (CSI), el índice de rendimiento del horario (SPI) y la estimación al finalizar (EAC).
author: Alina
feature: Work Management
exl-id: de628881-c016-4521-bc33-3bcfba19a88f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 1%

---

# Establecer el método de índice de rendimiento (PIM)

El método de índice de rendimiento (PIM) del proyecto controla el método que utiliza Adobe Workfront para calcular métricas de rendimiento del proyecto como el índice de rendimiento de costos (CPI), el índice de rendimiento del horario de costos (CSI), el índice de rendimiento del horario (SPI) y la estimación al finalizar (EAC).

Workfront calcula estos valores de la siguiente manera:

* Horas
* Costo

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos y datos financieros</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para el proyecto con permisos para Administrar finanzas</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Consideraciones sobre PIM en Workfront

* El administrador de Workfront o un administrador de grupo configuran de forma predeterminada si el Método de índice de rendimiento (PIM) debe basarse en horas o en costes. Los cálculos de las métricas de rendimiento cambian según la configuración de este valor predeterminado. Para obtener más información sobre cómo cambiar el valor predeterminado para calcular el PIM, consulte [Configurar las preferencias de proyecto en todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Los jefes de proyecto también pueden cambiar la configuración del PIM, en el nivel de proyecto, para proyectos individuales en la subpestaña Finance del proyecto. Debe tener permisos de administración en el proyecto para editar la subpestaña Finanzas del proyecto.

## Establecer el método de índice de rendimiento (PIM) para un proyecto

1. Vaya a un proyecto del que sea propietario.

   >[!IMPORTANT]
   >
   >Necesita permisos de administración en el proyecto para realizar los siguientes pasos. También recomendamos que solo el Propietario del proyecto realice cambios en el área de Finanzas del proyecto.

1. Haga clic en **Detalles del proyecto** en el panel izquierdo y, a continuación, vaya al área de **Finanzas**.
1. Haga doble clic en el valor del campo **Método de índice de rendimiento** para editarlo.
1. Seleccione entre las siguientes opciones del campo **Método de índice de rendimiento**:

   | Basado en horas | Workfront utiliza las horas planificadas para calcular el IPC y el EAC del proyecto, y el EAC del proyecto se muestra como un número, en horas. |
   |---|---|
   | Basado en costos | Workfront utiliza el coste laboral planificado para calcular el IPC y el EAC del proyecto, y el EAC se muestra como un valor de moneda. Al seleccionar esta opción, asegúrese de que las personas asignadas a la tarea (funciones del puesto o usuarios) estén asociadas a las tasas de coste. |

   {style="table-layout:auto"}

1. Haga clic en **Guardar** **Cambios**.
