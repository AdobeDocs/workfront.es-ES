---
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Ver: calcular el coste de horas extra en una vista de parte de horas'
description: Las horas extra no se calculan de forma predeterminada en Adobe Workfront, pero puede crear un informe de parte de horas que calcule las horas extra.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: ad6205cd-7534-49e5-b142-09f90bf672ce
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# Ver: calcular el coste de horas extra en una vista de hoja de horas

Las horas extra no se calculan de forma predeterminada en Adobe Workfront, pero puede crear un informe de parte de horas que calcule las horas extra.

Si el usuario está asociado con una tasa de costo por hora en su perfil, también puede calcular la cantidad de costo de las horas extra de ese usuario.\
Para obtener información sobre cómo asociar usuarios con las tasas de costo por hora, consulte el artículo [Configurar mis ajustes](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

>[!NOTE]
>
>El campo Horas extra que se puede agregar a una vista de parte de horas en una lista o un informe muestra la información que se encuentra en el campo Horas extra del parte de horas. Esta información la actualiza manualmente un usuario con acceso para modificar el parte de horas. Para obtener más información sobre el campo Tiempo extra de un parte de horas, consulte el artículo [Comprender el diseño de la hoja de horas](../../../timesheets/timesheets/timesheet-layout.md).

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
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Editar acceso a filtros, vistas y grupos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en un informe</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Calcular el costo de las horas extra en una vista de parte de horas

Para agregar una columna de tiempo extra calculada a una vista de parte de horas:

1. Vaya a una lista de partes de horas o cree un informe de parte de horas.

   Para obtener información sobre la creación de informes, consulte el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Haga clic en **Personalizar vista** en una lista de partes de horas.

   O

   Seleccione el **Columnas (Vista)** en un informe de hoja de horas.

1. Haga clic en **Agregar columna**.
1. Haga clic en **Cambiar al modo de texto**.
1. En el **Mostrar en esta columna** área, haga clic en **Haga clic para editar texto**.
1. Copie y pegue el siguiente código de modo de texto en el **Modo de texto** para abrir el Navegador.
   <pre>displayName=Calculated Overtime Cost<br>linkedname=direct<br>namekey=totalHours<br>querysort=totalHours <br>textmode=true<br>value=IF({totalHours}&gt;40,({totalHours}-40)*{user}.{costPerHour},{totalHours}*{user}.{costPerHour})<br>valueFormat=currencyStringCurrencyRound</pre>

   >[!NOTE]
   >
   >Este cálculo supone que el usuario suele trabajar una semana de 40 horas.

1. Haga clic en **Guardar**, asigne un nombre a la nueva vista y haga clic en **Guardar vista** en una lista de partes de horas.

   O

   Haga clic en **Guardar + Cerrar** en un informe de parte de horas.

1. (Opcional y condicional) si está creando un informe de parte de horas, especifique un nombre para el informe y haga clic en **Guardar informe**.

   El coste de las horas extra de cada usuario se muestra en la **Costo de horas extra calculado** para abrir el Navegador.

   ![calculated_overtime_cost_in_timesheet_report.png](assets/calculated-overtime-cost-in-timesheet-report-350x92.png)
