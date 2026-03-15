---
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ver: Calcular el coste de horas extra en una vista de parte de horas'
description: Las horas extra no se calculan de forma predeterminada en Adobe Workfront, pero puede crear un informe de parte de horas que calcule las horas extra.
author: Courtney
feature: Reports and Dashboards
exl-id: ad6205cd-7534-49e5-b142-09f90bf672ce
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 22%

---

# Vista: calcular el coste de horas extra en una vista de plantilla de horas

<!--Audited: 11/2024-->

Las horas extra no se calculan de forma predeterminada en Adobe Workfront, pero puede crear un informe de parte de horas que calcule las horas extra.

Si el usuario está asociado a una tasa de coste por hora en su perfil, también puede calcular el importe del coste de las horas extra de ese usuario.\
Para obtener información sobre la asociación de usuarios con tarifas de costo por hora, consulte el artículo [Configurar mi configuración](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

>[!NOTE]
>
>El campo Horas extra que puede agregar a una vista Hoja de horas de una lista o un informe muestra la información encontrada en el campo Horas extra del parte de horas. Esta información la actualiza manualmente un usuario con acceso para modificar el parte de horas. Para obtener más información sobre el campo Horas extra de un parte de horas, consulte el artículo [Introducción al diseño del parte de horas](../../../timesheets/timesheets/timesheet-layout.md).

![calculated_overtime_cost_in_timesheet_report.png](assets/calculated-overtime-cost-in-timesheet-report-350x92.png)

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
   <p>Colaborador o solicitud para modificar un filtro </p>
   <p>Estándar o Plan para modificar un informe</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Informes, Paneles de control y Calendarios para modificar un informe</p> <p>Acceso de edición a filtros, vistas y agrupaciones para modificar un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración para un informe</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Calcular el costo de horas extra en una vista Parte de horas

Para agregar una columna de horas extra calculada a una vista de parte de horas:

1. Vaya a una lista de partes de horas.

1. Haga clic en el menú desplegable **Ver** y, a continuación, en **Nueva vista**.

1. Haga clic en **Añadir columna**.
1. Haga clic en **Cambiar al modo de texto** y, a continuación, haga clic en **Editar modo de texto**.
1. En el cuadro **Editar modo de texto**, quite el texto del cuadro y, a continuación, copie y pegue el siguiente código de modo de texto:

   ```
   displayname=Calculated Overtime Cost
   linkedname=direct
   namekey=totalHours
   querysort=totalHours 
   textmode=true
   valueexpression=IF({totalHours}>40,({totalHours}-40)*{user}.{costPerHour},{totalHours}*{user}.{costPerHour})
   valueformat=currencyStringCurrencyRounded
   ```

   >[!NOTE]
   >
   >Este cálculo supone que el usuario suele trabajar una semana de 40 horas.

1. Haga clic en **Hecho**, asigne un nombre a la nueva vista y haga clic en **Guardar vista** en una lista de partes de horas.

   El costo de las horas extra de cada usuario se muestra en la columna **Costo calculado de horas extra**.


