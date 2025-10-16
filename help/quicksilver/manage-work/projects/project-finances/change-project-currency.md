---
product-area: projects
navigation-topic: financials
title: Cambiar la divisa del proyecto
description: Como administrador de proyectos, puede configurar un proyecto para que utilice una moneda distinta a la predeterminada para el sistema de Adobe Workfront. Esto le permite mostrar información financiera del proyecto en la moneda deseada al calcular los costes laborales y los ingresos.
author: Lisa
feature: Work Management
exl-id: c496fe92-5c17-41a5-972b-1c063643bde3
source-git-commit: 23a4d055871c9138818e70fa1cd936581dbd7552
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 98%

---

# Cambiar la moneda del proyecto

Como administrador de proyectos, puede configurar un proyecto para que utilice una moneda distinta a la predeterminada para el sistema de Adobe Workfront. Esto le permite mostrar información financiera del proyecto en la moneda deseada al calcular los costes laborales y los ingresos.

Antes de poder usar divisas alternativas, como se describe en esta sección, el administrador de Workfront debe habilitar y configurar primero varias divisas, tal como se describe en el artículo [Configuración de tipos de cambio](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

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
   <td>Acceso de edición a proyectos</td> 
  </tr> 
  <tr> 
   <td>Permisos de objeto</td> 
   <td>Administrar permisos del proyecto</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones a la hora de cambiar la divisa de un proyecto en Workfront

* No se puede cambiar la moneda de un proyecto cuando ya contiene información financiera
* Las tasas se utilizan para los costes laborales; los cálculos de ingresos y se utilizan en el futuro para fines de creación de informes.
* Si no especifica una moneda diferente para un proyecto, Workfront supone que la del proyecto es la predeterminada del sistema. Para obtener información sobre la moneda predeterminada a nivel de sistema, consulte [Configuración de tipos de cambio](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).
* De forma predeterminada, todos los usuarios con licencia completa tienen acceso para ver las monedas y los tipos de cambio. El administrador de Workfront debe conceder acceso administrativo adicional para los **tipos de cambio**, a fin de permitir que los usuarios establezcan tipos específicas en los proyectos.
* Los tipos de cambio en Workfront no son dinámicos. El valor lo establece un administrador y debe actualizarse cuando se produzcan cambios en los tipos de cambio.
* Cuando se crea un informe para reflejar la moneda de un proyecto, todos los informes se agrupan por la divisa predeterminada del proyecto. Si crea un informe con varios proyectos que tienen tipos de cambio diferentes, cualquier agrupación aplicada al proyecto refleja el tipo de cambio predeterminado en el nivel del sistema. Para obtener más información, consulte el artículo [Crear informes de datos financieros con tipos de cambio únicos](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

## Configuración de la moneda de un proyecto

1. Vaya al proyecto en el que desea cambiar la moneda predeterminada.

   >[!TIP]
   >
   >Asegúrese de que el proyecto no incluya ya información financiera. Por ejemplo, asegúrese de que no haya costes planificados o reales asociados con el proyecto.

1. Haga clic en **Detalles del proyecto** en el panel izquierdo y, a continuación, vaya al área de **Finanzas**.
1. Haga clic en **Añadir** en el campo **moneda** y seleccione la que desee usar como moneda predeterminada para el proyecto. Se muestran todas las monedas que el administrador de Workfront ha definido para la instancia de Workfront.

   ![Moneda en el proyecto](assets/currency-on-project-expanded-nwe.png)

1. (Condicional) Si selecciona una moneda distinta de la predeterminada establecida para el sistema de Workfront, especifique la tarifa de la moneda seleccionada, en relación con la establecida como base en el sistema.
1. Haga clic en **Guardar cambios**.
