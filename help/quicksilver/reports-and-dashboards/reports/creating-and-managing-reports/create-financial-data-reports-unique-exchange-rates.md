---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Crear informes de datos financieros con tasas de cambio únicas
description: Si se han configurado varios tipos de cambio en Adobe Workfront, puede definir valores financieros en informes y listas para que se muestren en una moneda distinta a la predeterminada.
author: Nolan
feature: Reports and Dashboards
exl-id: a0837c70-8330-4c38-98dc-8cf2e7e2e4bd
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '1025'
ht-degree: 0%

---

# Crear informes de datos financieros con tasas de cambio únicas

Si se han configurado varios tipos de cambio en Adobe Workfront, puede definir valores financieros en informes y listas para que se muestren en una moneda distinta a la predeterminada.

>[!IMPORTANT]
>
>Si selecciona una moneda distinta a la predeterminada en una vista, ya no verá los vínculos **Agregar más tareas** y **Agregar más problemas** en la parte inferior de una lista de proyectos.

Para obtener información sobre cómo cambiar la moneda predeterminada de un proyecto determinado, consulte [Cambiar la divisa del proyecto](../../../manage-work/projects/project-finances/change-project-currency.md).

Si hay proyectos con una sola moneda en el informe, las sumas de las agrupaciones también se muestran en la moneda predeterminada del sistema.

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
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Editar acceso a filtros, vistas y agrupaciones</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Requisitos previos

Para poder ver las divisas alternativas como se describe en esta sección, el administrador de Workfront debe activar y configurar primero varias divisas en el área de configuración de Workfront. Para obtener más información, consulte [Configurar tasas de cambio](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

## Aplicación de valores financieros a un informe {#apply-financial-values-to-a-report}

Para convertir valores financieros entre divisas al trabajar con informes:

1. Vaya al informe en el que desea convertir los valores financieros a una moneda diferente.
1. Haga clic en **Ver** , haga clic en **Cambiar divisa**, luego seleccione una de las siguientes monedas en la que desee mostrar los valores financieros:

   * Divisa original del proyecto
   * Cualquiera de las otras monedas

     >[!TIP]
     >
     >Sólo puede seleccionar divisas previamente seleccionadas en Configuración.

   El uso de esta opción le permite convertir rápidamente los valores financieros de un informe entre valores de tasa.

   ![Cambiar divisa](assets/qs-change-currency-2022-350x257.png)

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: drafted this tip because I think this is confusing; this is in the step above.)</p>
   -->

   <!--
   <note type="tip">
   You can also select the Change Currency option to convert financial values in other lists.
   <br>
   <img src="assets/nwe-change-currency-new-lists-350x219.png" style="width: 350;height: 219;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   <br>
   <br>
   </note>
   -->

## Mostrar la moneda predeterminada en varios proyectos con distintas monedas

Cuando personaliza la moneda en el nivel de proyecto y desea mostrar información de todos los proyectos del mismo informe, existen los siguientes escenarios:

* Si crea un informe que obtiene información financiera de dos o más proyectos a los que se han aplicado distintas divisas, el resumen de agrupación refleja de forma predeterminada la divisa predeterminada del sistema, según la haya seleccionado el administrador de Workfront.
* Si crea un informe para dos o más proyectos que tienen la misma moneda, pero difieren de la moneda predeterminada del sistema, las sumas de las agrupaciones se muestran con la moneda predeterminada del sistema.
* Si crea un informe para dos o más proyectos que tienen asignaciones de funciones asociadas a una sustitución de divisa, Workfront convierte la información financiera de las tasas de cambio de divisa sustituidas de la función a la divisa del proyecto (al seleccionar Divisa Original del Proyecto en la vista) o a cualquier divisa diferente que seleccione al consultar el informe. Para obtener información sobre cómo anular la moneda de un rol, consulte [Crear y administrar roles](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

Para mostrar dos proyectos con monedas personalizadas en un informe:

1. Cree dos proyectos con diferentes monedas aplicadas.

   ![](assets/qs-currency-350x217.png)

1. Registrar horas en ambos proyectos.

   Para obtener más información sobre el registro del tiempo, consulte [Registrar tiempo](../../../timesheets/create-and-manage-timesheets/log-time.md).

1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png), luego haga clic en **Informes**.
1. Clic **Nuevo informe**, entonces **Informe de proyecto**.
1. En el **Columnas (vista)** pestaña, añadir una **Costo real** y lo resume por **Sum**.

   Para obtener información sobre cómo crear una columna, consulte [Información general sobre vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. En el **Agrupaciones** pestaña, aplique una **Fecha planificada de finalización** agrupación.

   Para obtener información sobre cómo crear una agrupación, consulte [Información general sobre agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. En el **Filtros** pestaña, añadir un filtro para **Nombre de proyecto** y seleccione los dos proyectos con las distintas monedas.

   Para obtener información sobre cómo crear un filtro, consulte [Resumen de filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Haga clic en **Guardar + Cerrar**.

   El total de la **Costo real** se muestra en la variable Grouping using the system default currency, independientemente de la moneda de los proyectos del informe.

   ![Moneda mostrada en la agrupación](assets/qs-currency-displayed-in-groupings-2022-350x292.png)

   Si los dos proyectos tienen monedas diferentes, la moneda predeterminada del sistema también se muestra en la sección Agrupación del informe.

## Mostrar la divisa del proyecto en un informe en el nivel de proyecto

Si se aplica una agrupación en una lista de tareas u horas dentro de un proyecto, las sumas de la agrupación se muestran en la moneda del proyecto.

1. Cree un proyecto con una moneda personalizada que no sea la moneda predeterminada del sistema.
1. Vaya al proyecto y asegúrese de que incluye horas que se han registrado para tareas.

   Para obtener más información sobre el registro del tiempo, consulte [Registrar tiempo](../../../timesheets/create-and-manage-timesheets/log-time.md).

   >[!NOTE]
   >
   >Las tareas deben asignarse a usuarios o roles con tasas de coste por hora.

1. Clic **Tareas**.
1. Expanda el **Ver** menú desplegable y seleccione **Nueva vista**.
1. Añadir **Costo real** en la nueva vista como una columna nueva y resuma el valor por **Sum**.
1. Clic **Listo**, luego haga clic en **Guardar vista**.
1. Expanda el **Agrupación** menú desplegable y seleccione **Nueva agrupación**.
1. Añadir **Fecha real de finalización** en la nueva agrupación como un nuevo campo, haga clic en **Guardar agrupación**.

   El **Costo real** La columna resume la nueva agrupación y muestra el total en la moneda del proyecto.

## Editar informes con monedas únicas

Los campos financieros de un informe no se pueden editar hasta que cambie la configuración del informe para mostrar la moneda original de los proyectos.

Para editar en línea un campo financiero en un informe:

1. Vaya a un informe.

   >[!NOTE]
   >
   >Si la moneda predeterminada no se muestra para una lista en ninguna otra área, puede editar la Vista para mostrar la moneda predeterminada.\
   >Para obtener información sobre cómo cambiar la moneda en una vista, consulte la sección de este artículo [Aplicación de valores financieros a un informe](#apply-financial-values-to-a-report).

1. Clic **Acciones de informe**, luego seleccione **Editar**.
1. Clic **Configuración de informes**.
1. Haga clic en **Moneda predeterminada** , luego seleccione. **Divisa original del proyecto**.

   ![](assets/qs-report-settings-default-currency-350x370.png)

1. Clic **Listo**.
