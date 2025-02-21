---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Cree informes de datos financieros con tipos de cambio únicos
description: Si se configuraron varios tipos de cambio en Adobe Workfront, es posible establecer valores financieros en informes y listas para que se muestren en una moneda distinta de la predeterminada.
author: Nolan
feature: Reports and Dashboards
exl-id: a0837c70-8330-4c38-98dc-8cf2e7e2e4bd
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '984'
ht-degree: 98%

---

# Cree informes de datos financieros con tipos de cambio únicos

<!-- Audited: 11/2024 -->

Si se configuraron varios tipos de cambio en Adobe Workfront, es posible establecer valores financieros en informes y listas para que se muestren en una moneda distinta de la predeterminada.

>[!IMPORTANT]
>
>Al seleccionar una moneda distinta de la predeterminada en una vista, ya no se verán los vínculos **Añadir más tareas** y **Añadir más problemas** al final de las listas de proyectos.

Para obtener información acerca de cómo cambiar la moneda predeterminada de un proyecto determinado, consulte [Cambiar la moneda del proyecto](../../../manage-work/projects/project-finances/change-project-currency.md).

Si hubiera proyectos con una sola moneda en el informe, las sumas de las agrupaciones también se mostrarán en la moneda predeterminada del sistema.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> 
      <p>Nuevo:</p>
         <ul>
         <li><p>Estándar</p></li>
         </ul>
      <p>Actual:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso de edición a informes, paneles y calendarios</p> <p>Acceso de edición a filtros, vistas y agrupaciones</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto*</td> 
   <td> <p>Permisos de administración para un informe</p></td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Para poder ver monedas alternativas como se describe en esta sección, el administrador de Workfront deberá activar y configurar primero varias monedas en el área de configuración de Workfront. Para obtener más información, consulte [Configuración de tipos de cambio](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

## Aplicar valores financieros a un informe {#apply-financial-values-to-a-report}

Para convertir valores financieros entre monedas al trabajar con informes:

1. Vaya al informe en el que quiera convertir los valores financieros a una moneda diferente.
1. Haga clic en la lista desplegable **Ver**, haga clic en **Cambiar moneda** y, a continuación, seleccione una de las siguientes monedas en la que desee que se muestren los valores financieros:

   * Moneda original del proyecto
   * Cualquiera de las otras monedas

     >[!TIP]
     >
     >Solo es posible seleccionar monedas previamente seleccionadas en Configuración.

   El uso de esta opción permite convertir rápidamente los valores financieros de un informe entre valores de tipos.

   ![Cambiar moneda](assets/qs-change-currency-2022-350x257.png)

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

Al personalizar la moneda en el proyecto y mostrar información de todos los proyectos en el mismo informe, se dan los siguientes escenarios:

* Al crear informes que obtengan información financiera de dos o más proyectos a los que se hayan aplicado distintas divisas, el resumen de agrupación reflejará de forma predeterminada la moneda predeterminada del sistema, según la haya seleccionado el administrador de Workfront.
* Al crear informes para dos o más proyectos que tengan la misma moneda, pero difieran de la moneda predeterminada del sistema, las sumas de las agrupaciones se mostrarán con la moneda predeterminada del sistema.
* Al crear informes para dos o más proyectos que tengan asignaciones de funciones asociadas a un cambio de moneda, Workfront convertirá la información financiera de los tipos de cambio de moneda cambiados de la función a la moneda del proyecto (al seleccionar Moneda original del proyecto en la vista) o a cualquier moneda diferente que se seleccione al consultar el informe. Para obtener información sobre cómo cambiar la moneda de una función, consulte [Crear y administrar funciones](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

Para mostrar dos proyectos con monedas personalizadas en un informe:

1. Crear dos proyectos con diferentes monedas aplicadas.

    ![Divisa](assets/qs-currency-350x217.png)

1. Registro de horas en ambos proyectos.

   Para obtener más información acerca del registro del tiempo, consulte [Registrar tiempo](../../../timesheets/create-and-manage-timesheets/log-time.md).

1. Haga clic en el icono **Menú principal** ![Icono del menú principal](assets/main-menu-icon.png) y luego haga clic en **Informes**.
1. Haga clic en **Nuevo informe** y luego en **Informe del proyecto**.
1. En la pestaña **Columnas (Vista)**, añada una columna **Coste real** y revísela por **Suma**.

   Para obtener información sobre cómo crear columnas, consulte [Información general sobre vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. En la pestaña **Agrupaciones**, aplique una agrupación a **Fecha planificada de finalización**.

   Para obtener información sobre cómo crear agrupaciones, consulte [Información general sobre agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. En la pestaña **Filtros**, añada un filtro para **Nombre de proyecto** y seleccione los dos proyectos con monedas diferentes.

   Para obtener información sobre cómo crear un filtro, consulte [Información general sobre filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Haga clic en **Guardar + Cerrar**.

   El total del **Coste real** se muestra en la agrupación usando la moneda predeterminada del sistema, independientemente de la moneda de los proyectos del informe.

   Si los dos proyectos tienen monedas diferentes, la moneda predeterminada del sistema también se muestra en la sección Agrupación del informe.

## Visualización de la divisa del proyecto en un informe a nivel de proyecto

Si se aplica una agrupación en una lista de tareas u horas dentro de un proyecto, las sumas de la agrupación se muestran en la moneda del proyecto.

1. Cree un proyecto con una moneda personalizada que no sea la moneda predeterminada del sistema.
1. Vaya al proyecto y asegúrese de que incluye horas que se han registrado para tareas.

   Para obtener más información sobre el registro del tiempo, consulte [Registrar el tiempo](../../../timesheets/create-and-manage-timesheets/log-time.md).

   >[!NOTE]
   >
   >Las tareas deben asignarse a usuarios o funciones de trabajo con tarifas de coste Tarifas por hora.

1. Haga clic en **Tareas**.
1. Expanda el menú desplegable **Vista** y seleccione **Nueva vista**.
1. Añada **Coste real** en la nueva vista como una columna nueva y resúmala como **Suma**.
1. Haga clic en **Listo** y luego haga clic en **Guardar vista**.
1. Expanda el menú desplegable **Agrupación** y seleccione **Nueva agrupación**.
1. Añada **Fecha real de finalización** a la nueva agrupación como un nuevo campo y luego haga clic en **Guardar agrupación**.

   La columna **Coste real** se resume en la nueva agrupación y muestra el total en la moneda del proyecto.

## Edición de informes con monedas únicas

Los campos financieros de un informe no se pueden editar hasta que cambie la configuración del informe para mostrar la moneda original de los proyectos.

Para editar en línea un campo financiero en un informe:

1. Vaya a un informe.

   >[!NOTE]
   >
   >Si la moneda predeterminada no se muestra para una lista en ninguna otra área, puede editar la vista para mostrar la moneda predeterminada.\
   >Para obtener información sobre cómo cambiar la moneda en una vista, consulte la sección de este artículo [Aplicar valores financieros a un informe](#apply-financial-values-to-a-report).

1. Haga clic en **Acciones de informe** y seleccione **Editar**. 
1. Haga clic en **Configuración del informe**.
1. Haga clic en el menú desplegable **Moneda predeterminada** y, a continuación, seleccione **Moneda original del proyecto**.

   ![Moneda predeterminada](assets/qs-report-settings-default-currency-350x370.png)

1. Haga clic en **Listo**.
