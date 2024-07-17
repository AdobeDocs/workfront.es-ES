---
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
title: "Vista: calcular el coste de horas extra en una vista de plantilla de horas"
description: Las horas extra no se calculan de forma predeterminada en Adobe Workfront, pero puede crear un informe de hoja de horas que calcule las horas extra.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: ad6205cd-7534-49e5-b142-09f90bf672ce
source-git-commit: c49b545938a78716084296ef1b4e7c0fc075ef95
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 1%

---

# Ver: calcular el coste de horas extra en una vista de hoja de horas

Las horas extra no se calculan de forma predeterminada en Adobe Workfront, pero puede crear un informe de hoja de horas que calcule las horas extra.

Si el usuario está asociado con una tarifa de coste por hora en su perfil, también puede calcular la cantidad de coste por las horas extra de ese usuario.\
Para obtener información acerca de cómo asociar usuarios con tasas de costo por hora, vea el artículo [Configurar mis opciones](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

>[!NOTE]
>
>El campo Horas extra que se puede agregar a una vista Hoja de horas de una lista o un informe muestra la información que se encuentra en el campo Horas extra de la hoja de horas. La información la actualiza manualmente un usuario con acceso para modificar la plantilla de horas. Para obtener más información sobre el campo Horas extra en una hoja de horas, consulte el artículo [Información general sobre el diseño de la hoja de horas](../../../timesheets/timesheets/timesheet-layout.md).

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
   <td> <p>Solicitud para modificar una vista </p>
   <p>Plan para modificar un informe</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar el acceso a Informes, Tableros y Calendarios para modificar un informe</p> <p>Editar el acceso a filtros, vistas y agrupaciones para modificar una vista</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Calcular costo de horas extra en una vista de hoja de horas

Para agregar una columna de horas extra calculadas a una vista de hoja de horas:

1. Vaya a una lista de plantillas de horas o cree un informe de plantilla de horas.

   Para obtener información sobre cómo crear informes, consulte el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Haga clic en **Personalizar vista** en una lista de hojas de horas.

   O

   Seleccione la ficha **Columnas (Ver)** en un informe de hoja de horas.

1. Haga clic en **Añadir columna**.
1. Haga clic en **Cambiar al modo de texto**.
1. En el área **Mostrar en esta columna**, haga clic en **Haga clic para editar el texto**.
1. Copie y pegue el siguiente código de modo de texto en el cuadro de diálogo **Modo de texto**.
   <pre>displayname=Costo calculado de horas extra<br>linkedname=direct<br>namekey=totalHours<br>querysort=totalHours <br>textmode=true<br>valueexpression=IF({totalHours}&gt;40,({totalHours}-40)*{user}.{costPerHour},{totalHours}*{user}.{costPerHour})<br>valueformat=currencyStringCurrencyRounded</pre>

   >[!NOTE]
   >
   >Este cálculo supone que el usuario suele trabajar una semana de 40 horas.

1. Haga clic en **Guardar**, asigne un nombre a la nueva vista y haga clic en **Guardar vista** en una lista de hojas de horas.

   O

   Haga clic en **Guardar + Cerrar** en un informe de hoja de horas.

1. (Opcional y condicional) Si está generando un informe de hoja de horas, especifique un nombre para el informe y haga clic en **Guardar informe**.

   El costo de las horas extra de cada usuario se muestra en la columna **Costo calculado de horas extra**.

   ![informe_parte_de_horas_extra_calculadas_costo_en_parte_de_horas.png](assets/calculated-overtime-cost-in-timesheet-report-350x92.png)
