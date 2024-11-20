---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Crear informes de datos financieros con tasas de cambio únicas
description: Si se han configurado varios tipos de cambio en Adobe Workfront, puede definir valores financieros en informes y listas para que se muestren en una moneda distinta a la predeterminada.
author: Nolan
feature: Reports and Dashboards
exl-id: a0837c70-8330-4c38-98dc-8cf2e7e2e4bd
source-git-commit: 2322415c173919a1fecffabb4b561645d33eea8d
workflow-type: tm+mt
source-wordcount: '978'
ht-degree: 0%

---

# Crear informes de datos financieros con tasas de cambio únicas

<!-- Audited: 11/2024 -->

Si se han configurado varios tipos de cambio en Adobe Workfront, puede definir valores financieros en informes y listas para que se muestren en una moneda distinta a la predeterminada.

>[!IMPORTANT]
>
>Si selecciona una moneda distinta a la predeterminada en una vista, ya no verá los vínculos **Agregar más tareas** y **Agregar más problemas** al final de la lista de proyectos.

Para obtener información acerca de cómo cambiar la moneda predeterminada de un proyecto determinado, vea [Cambiar la moneda del proyecto](../../../manage-work/projects/project-finances/change-project-currency.md).

Si hay proyectos con una sola moneda en el informe, las sumas de las agrupaciones también se muestran en la moneda predeterminada del sistema.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Editar acceso a filtros, vistas y agrupaciones</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto*</td> 
   <td> <p>Administración de permisos de un informe</p></td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Para poder ver las divisas alternativas como se describe en esta sección, el administrador de Workfront debe activar y configurar primero varias divisas en el área de configuración de Workfront. Para obtener más información, consulte [Configurar tasas de cambio](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

## Aplicación de valores financieros a un informe {#apply-financial-values-to-a-report}

Para convertir valores financieros entre divisas al trabajar con informes:

1. Vaya al informe en el que desea convertir los valores financieros a una moneda diferente.
1. Haga clic en la lista desplegable **Ver**, haga clic en **Cambiar moneda** y, a continuación, seleccione una de las siguientes monedas en las que desee mostrar los valores financieros:

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

   Para obtener más información acerca del registro del tiempo, vea [Registrar tiempo](../../../timesheets/create-and-manage-timesheets/log-time.md).

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) y luego haga clic en **Informes**.
1. Haga clic en **Nuevo informe** y luego en **Informe del proyecto**.
1. En la ficha **Columnas (Ver)**, agregue una columna **Costo real** y revísela por **Suma**.

   Para obtener información sobre cómo crear una columna, consulte [Información general sobre vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. En la ficha **Agrupaciones**, aplique una agrupación de **Fecha planificada de finalización**.

   Para obtener información sobre cómo crear una agrupación, consulte [Información general sobre agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. En la ficha **Filtros**, agregue un filtro para **Nombre de proyecto** y seleccione los dos proyectos con monedas diferentes.

   Para obtener información sobre cómo crear un filtro, consulte [Resumen de filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Haga clic en **Guardar + Cerrar**.

   El total de **Costo real** se muestra en la agrupación usando la moneda predeterminada del sistema, independientemente de la moneda de los proyectos del informe.

   Si los dos proyectos tienen monedas diferentes, la moneda predeterminada del sistema también se muestra en la sección Agrupación del informe.

## Mostrar la divisa del proyecto en un informe en el nivel de proyecto

Si se aplica una agrupación en una lista de tareas u horas dentro de un proyecto, las sumas de la agrupación se muestran en la moneda del proyecto.

1. Cree un proyecto con una moneda personalizada que no sea la moneda predeterminada del sistema.
1. Vaya al proyecto y asegúrese de que incluye horas que se han registrado para tareas.

   Para obtener más información acerca del registro del tiempo, vea [Registrar tiempo](../../../timesheets/create-and-manage-timesheets/log-time.md).

   >[!NOTE]
   >
   >Las tareas deben asignarse a usuarios o roles con tasas de coste por hora.

1. Haga clic en **Tareas**.
1. Expanda el menú desplegable **Vista** y seleccione **Nueva vista**.
1. Agregue **Costo real** a la nueva vista como una columna nueva y resuma el valor por **Suma**.
1. Haz clic en **Listo** y luego haz clic en **Guardar vista**.
1. Expanda el menú desplegable **Agrupación** y seleccione **Nueva agrupación**.
1. Agregue **Fecha real de finalización** a la nueva agrupación como un nuevo campo y luego haga clic en **Guardar agrupación**.

   La columna **Costo real** se resume en la nueva agrupación y muestra el total en la moneda del proyecto.

## Editar informes con monedas únicas

Los campos financieros de un informe no se pueden editar hasta que cambie la configuración del informe para mostrar la moneda original de los proyectos.

Para editar en línea un campo financiero en un informe:

1. Vaya a un informe.

   >[!NOTE]
   >
   >Si la moneda predeterminada no se muestra para una lista en ninguna otra área, puede editar la Vista para mostrar la moneda predeterminada.\
   >Para obtener información sobre cómo cambiar la moneda en una vista, consulte la sección de este artículo [Aplicar valores financieros a un informe](#apply-financial-values-to-a-report).

1. Haga clic en **Acciones de informe** y, a continuación, seleccione **Editar**.
1. Haga clic en **Configuración del informe**.
1. Haga clic en el menú desplegable **Moneda predeterminada** y, a continuación, seleccione **Moneda original del proyecto**.

   ![](assets/qs-report-settings-default-currency-350x370.png)

1. Haga clic en **Listo**.
