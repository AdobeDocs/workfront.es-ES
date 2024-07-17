---
product-area: projects
navigation-topic: financials
title: Cambiar la divisa del proyecto
description: Como administrador de proyectos, puede configurar un proyecto para que utilice una moneda distinta a la predeterminada para el sistema de Adobe Workfront. Esto le permite mostrar información financiera del proyecto en la moneda deseada al calcular los costes laborales y los ingresos.
author: Alina
feature: Work Management
exl-id: c496fe92-5c17-41a5-972b-1c063643bde3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---

# Cambiar la divisa del proyecto

Como administrador de proyectos, puede configurar un proyecto para que utilice una moneda distinta a la predeterminada para el sistema de Adobe Workfront. Esto le permite mostrar información financiera del proyecto en la moneda deseada al calcular los costes laborales y los ingresos.

Antes de poder usar monedas alternativas como se describe en esta sección, el administrador de Workfront debe habilitar y configurar primero varias monedas, tal como se describe en el artículo [Configurar tasas de cambio](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

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
   <td> <p>Editar acceso a Proyectos</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos en un proyecto</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Consideraciones al cambiar la moneda de un proyecto en Workfront

* No puede cambiar la moneda de un proyecto si contiene información financiera.
* Las tasas se utilizan para los costes laborales; los cálculos de ingresos y se utilizan en el futuro para fines de creación de informes.
* Si no especifica una divisa diferente para un proyecto, Workfront supone que la divisa del proyecto es la divisa predeterminada del sistema. Para obtener información sobre la moneda predeterminada en el nivel del sistema, consulte [Configurar tasas de cambio](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).
* De forma predeterminada, todos los usuarios con licencia completa tienen acceso para ver las monedas y los tipos de cambio. El administrador de Workfront debe conceder acceso administrativo adicional para **tasas de cambio** a fin de permitir que los usuarios establezcan tasas específicas en los proyectos.
* Las tasas de cambio en Workfront no son dinámicas. El valor lo establece un administrador y debe actualizarse cuando se produzcan cambios en los tipos de cambio.
* Cuando se crea un informe para reflejar la moneda de un proyecto, de forma predeterminada todos los informes se agrupan por la moneda predeterminada del proyecto. Si crea un informe con varios proyectos que tienen tasas de cambio diferentes, cualquier agrupación aplicada al proyecto reflejará la tasa de cambio predeterminada en el nivel del sistema. Para obtener más información, consulte el artículo [Crear informes de datos financieros con tasas de cambio únicas](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

## Configuración de la moneda de un proyecto

1. Vaya al proyecto en el que desea cambiar la moneda predeterminada.

   >[!TIP]
   >
   >Asegúrese de que el proyecto no tenga ya información financiera. Por ejemplo, asegúrese de que no hay costos planificados o reales asociados con el proyecto.

1. Haga clic en **Detalles del proyecto** en el panel izquierdo y, a continuación, vaya al área de **Finanzas**.
1. Haga clic en **Agregar** en el campo **Moneda** y seleccione la moneda que desee usar como moneda predeterminada para el proyecto. Se muestran todas las divisas que el administrador de Workfront ha definido para la instancia de Workfront.

   ![](assets/currency-on-project-expanded-nwe.png)

1. (Condicional) Si selecciona una divisa distinta de la predeterminada establecida para el sistema de Workfront, especifique la tarifa de la divisa seleccionada, en relación con la divisa establecida como divisa base en el sistema.
1. Haga clic en **Guardar cambios**.
