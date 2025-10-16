---
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Vista: Calcular costo de horas extra en una vista de hoja de horas'
description: Las horas extra no se calculan de forma predeterminada en Adobe Workfront, pero puede crear un informe de hoja de horas que calcule las horas extra.
author: Nolan
feature: Reports and Dashboards
exl-id: ad6205cd-7534-49e5-b142-09f90bf672ce
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 18%

---

# Ver: calcular el coste de horas extra en una vista de hoja de horas

<!--Audited: 11/2024-->

Las horas extra no se calculan de forma predeterminada en Adobe Workfront, pero puede crear un informe de hoja de horas que calcule las horas extra.

Si el usuario está asociado con una tarifa de coste por hora en su perfil, también puede calcular la cantidad de coste por las horas extra de ese usuario.\
Para obtener información acerca de cómo asociar usuarios con tasas de costo por hora, vea el artículo [Configurar mis opciones](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

>[!NOTE]
>
>El campo Horas extra que se puede agregar a una vista Hoja de horas de una lista o un informe muestra la información que se encuentra en el campo Horas extra de la hoja de horas. La información la actualiza manualmente un usuario con acceso para modificar la plantilla de horas. Para obtener más información sobre el campo Horas extra en una hoja de horas, consulte el artículo [Información general sobre el diseño de la hoja de horas](../../../timesheets/timesheets/timesheet-layout.md).

![informe_parte_de_horas_extra_calculadas_costo_en_parte_de_horas.png](assets/calculated-overtime-cost-in-timesheet-report-350x92.png)

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
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

## Calcular costo de horas extra en una vista de hoja de horas

Para agregar una columna de horas extra calculadas a una vista de hoja de horas:

1. Ir a una lista de plantillas de horas.

1. Haga clic en el menú desplegable **Vista** y luego haga clic en **Nueva vista**.

1. Haga clic en **Añadir columna**.
1. Haga clic en **Cambiar al modo de texto** y luego haga clic en **Editar modo de texto**.
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

1. Haga clic en **Listo**, asigne un nombre a la nueva vista y haga clic en **Guardar vista** en una lista de hojas de horas.

   El costo de las horas extra de cada usuario se muestra en la columna **Costo calculado de horas extra**.


