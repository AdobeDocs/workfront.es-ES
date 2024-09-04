---
product-area: resource-management
navigation-topic: resource-planning
title: Revisar la disponibilidad y asignación de recursos mediante el Planificador de recursos de Adobe Workfront
description: Puede consultar la disponibilidad de los recursos y la cantidad de trabajo planificado o presupuestado de los proyectos en el Planificador de recursos. Estos valores se muestran en horas, ETC (equivalente a tiempo completo) o importes de coste y se organizan en columnas.
author: Lisa
feature: Resource Management
exl-id: 5b3e52a6-af9b-4e68-8d6e-43a5151a2a2c
source-git-commit: a5317e3126939d4c648977635af2dbc6add02780
workflow-type: tm+mt
source-wordcount: '1237'
ht-degree: 4%

---

# Revisar la disponibilidad y asignación de recursos mediante el Planificador de recursos de Adobe Workfront

Puede consultar la disponibilidad de los recursos y la cantidad de trabajo planificado o presupuestado de los proyectos en el Planificador de recursos. Estos valores se muestran en horas, ETC (equivalente a tiempo completo) o importes de coste y se organizan en columnas.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td><p>Nuevo: Cualquiera</p>
       <p>o</p>
       <p>Actual: Pro o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Nuevo: claro o superior</p>
       <p>o</p>
       <p>Actual: revisar o superior</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Vea o acceda a lo siguiente:</p> 
    <ul> 
     <li> <p>Administración de recursos</p> </li> 
     <li> <p>Datos financieros</p> </li> 
     <li> <p>Usuarios</p> </li> 
     <li> <p>Proyectos</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver los permisos superiores a los proyectos que desea ver en el Planificador de recursos</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Debe cumplir todos los requisitos previos necesarios para trabajar con el Planificador de recursos. Para obtener más información, consulte [Resumen del Planificador de recursos](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

>[!IMPORTANT]
>
>Si falta alguno de los requisitos previos necesarios para la correcta funcionalidad del Planificador de recursos, algunos de los números pueden ser cero o las horas presupuestadas pueden estar atenuadas.

## Disponibilidad y asignación de recursos

Las columnas que muestran la disponibilidad y la asignación de los recursos cambian según la vista que aplique al Planificador de recursos. Para obtener información sobre cómo mostrar la información en el Planificador de recursos por proyecto, rol o usuario, consulte [Resumen de navegación del Planificador de recursos](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

Tenga en cuenta lo siguiente al cambiar la vista al Planificador de recursos:

* Cuando aplique las vistas **Vista por proyecto** o **Vista por rol**, verá las siguientes columnas:

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: Alina: (some of the information in this area is also covered in Calculating Costs in the RP - https://workfront.zendesk.com/hc/en-us/articles/115004186433 - update this article also, when changes here occur)
  </MadCap:conditionalText>
  -->



   * Horas, ETC o costos disponibles
   * Horas planificadas, ETC o costo
   * Horas, ETC o Coste presupuestados
   * Desviación de horas, ETC o costo
   * Horas netas, ETC o Coste

* Al aplicar la vista **Vista por usuario**, puede ver las siguientes columnas:

   * Horas disponibles o ETC
   * Horas planificadas o ETC
   * Diferencia de hora o ETC
   * Porcentaje de asignación de horas planificadas

>[!TIP]
>
>La información no está disponible como Costo al aplicar la vista **Ver por usuario** al Planificador de recursos.
>
>Para obtener más información sobre lo que muestra cada columna, pase el ratón sobre el nombre de la columna en la que se muestra el número.\
>![Net_hours_res_planner_mouse_over.png](assets/net-hours-res-planner-mouse-over-350x95.png)
>
>Para obtener más información sobre los datos mostrados en cada columna, consulte los siguientes artículos:
>
>* [Información general sobre horas, ETC e información de costos en las vistas Proyecto y Rol del Planificador de recursos](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)
>* [Ver horas disponibles, planificadas y reales o FTE en el Planificador de recursos al usar la vista de usuario](../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md)
>

## Ver información por hora, ETC o costo

1. Vaya al Planificador de recursos.

   De forma predeterminada, la información se muestra por horas en el Planificador de recursos.

1. Expanda el menú desplegable.\
   ![Horas_después_o_costo_desplegable.png](assets/hours-fte-or-cost-dropdown.png)

1. Seleccione entre las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Horas</td> 
      <td>Muestra la información de disponibilidad y asignación en horas.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">ETC</td> 
      <td> <p>Muestra información de disponibilidad y asignación en FTE.</p> <p>Para obtener más información acerca de cómo se calcula el valor de FTE en el Planificador de recursos, vea <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Información general sobre el cálculo de horas y de FTE para usuarios y roles en el Planificador de recursos</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Costo</td> 
      <td> <p>Muestra la información de disponibilidad y asignación por costo, si está viendo el Planificador de recursos en las vistas Proyecto o Rol. La información muestra los valores en la moneda del sistema. El administrador de Workfront define la divisa del sistema. Para obtener más información sobre cómo configurar la divisa del sistema en Workfront, consulte <a href="../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Configurar tasas de cambio</a>.</p> <p><b>NOTA</b>

   Debe asociar usuarios y roles con tasas de costo por hora para mostrar la información de costo en el Planificador de recursos.<br style="font-style: italic;">Para obtener más información sobre cómo asociar las tarifas de costo por hora con los roles de trabajo, consulte <a href="../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Crear y administrar roles</a>.<br style="font-style: italic;">Para obtener más información sobre cómo asociar tarifas de costo por hora con usuarios, consulte <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Editar el perfil de un usuario</a>.<br style="font-style: italic;">Para obtener más información acerca de cómo se calcula el costo en el Planificador de recursos, vea <a href="../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md" class="MCXref xref">Calcular costos en el Planificador de recursos </a>.</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Personalizar</td> 
      <td>Crea una vista personalizada de las columnas que se muestran en el Planificador de recursos. Seleccione las opciones que desea mostrar en el Planificador de recursos, tal como se describe en los pasos siguientes. </td> 
     </tr> 
    </tbody> 
   </table>

1. (Condicional) Si seleccionó **Personalizar**, indique las opciones en el cuadro **Personalizar las métricas mostradas** para configurar la vista personalizada.

   ![](assets/planner-customize-view-box-350x114.png)

1. En la columna **Tipo de vista** de la izquierda, seleccione una de las siguientes vistas:

   * Proyecto
   * Función
   * Usuario

1. En la sección **Mostrar elementos seleccionados**, seleccione el tipo de información que desea mostrar en las columnas de la vista seleccionada. La tabla siguiente muestra qué opciones están disponibles en cada vista:

   | **Opción** | Vista de usuario | Vista de proyectos | Vista de rol |
   |---|---|---|---|
   | Disponible | ✔ | ✔ | ✔ |
   | Planificados | ✔ | ✔ | ✔ |
   | Presupuestado |   | ✔ | ✔ |
   | Desviación |   | ✔ | ✔ |
   | Neto |   | ✔ | ✔ |
   | Real | ✔ |   |   |
   | Diferencia | ✔ |   |   |
   | Porcentaje | ✔ |   |   |

1. Seleccione **Usar valores planificados (PLN) en los cálculos de red** para usar la información planificada en lugar de la presupuestada al calcular los valores netos en las vistas Proyecto y Rol.

   Al seleccionar esta opción, Workfront calcula los valores netos mediante la siguiente fórmula:

   `Net = Available - Planned`

   >[!TIP]
   >
   >**Esta opción se aplica solamente cuando selecciona al menos una opción para personalizar la vista en la sección Mostrar los elementos seleccionados.**

1. Haga clic en **Guardar**.

   Se muestra la vista personalizada que incluye las columnas seleccionadas.

   El Planificador de recursos enumera la vista personalizada como Personalizada en el menú desplegable Horas.

   >[!NOTE]
   >
   >Solo puede tener una vista personalizada.

   ![](assets/planner-hours-drop-down-with-custom-and-customize-option-183x281.png)

## Ver el gráfico de asignación de usuarios

Puede mostrar en un gráfico la asignación planificada de los usuarios en relación con su disponibilidad.

Para mostrar la asignación de usuarios en un gráfico:

1. Vaya al Planificador de recursos.

   Para obtener más información sobre cómo obtener acceso al Planificador de recursos, consulte la sección [Localizar el Planificador de recursos](../../resource-mgmt/resource-planning/get-started-resource-planner.md#accessing-the-resource-planner) en el artículo [Información general del Planificador de recursos](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

1. Seleccione **Ver por usuario**.

   >[!TIP]
   >
   >Solo puede ver el gráfico de asignación de usuarios en la vista de usuario.

1. Haga clic en el icono **Gráfico de asignación de usuarios** ![RP_user_allocation_chart.png](assets/rp-user-allocation-chart.png) para mostrar la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">% de disponibilidad sin asignación excesiva para todos los usuarios</td> 
      <td>Es la cantidad de tiempo que todos los usuarios están disponibles para trabajar en un período de tiempo, que se muestra como porcentaje del tiempo total disponible. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">% de asignación excesiva para todos los usuarios </td> 
      <td> <p>Es la cantidad de tiempo que los usuarios están sobreasignados en un período de tiempo, que se muestra como porcentaje del tiempo total disponible.</p> <p><b>NOTA</b>

   Una sobreasignación se produce cuando las horas planificadas son superiores a las horas disponibles. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">% de infrautilización para todos los usuarios</td> 
      <td> <p>Es la cantidad de tiempo que los usuarios están infrautilizados en un período de tiempo, que se muestra como porcentaje del tiempo total disponible.</p> <p><b>NOTA</b>

   La infrautilización se produce cuando las horas planificadas son inferiores a las horas disponibles. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Al menos un usuario tiene una asignación excesiva durante este período de tiempo</td> 
      <td>Esto indica que hay una sobreasignación para al menos un usuario en un período de tiempo, aunque la cantidad total de tiempo de todos los usuarios no está sobreasignada para el período de tiempo.<br>Debe desplazarse por la lista de usuarios y las horas del usuario sobreasignado aparecerán resaltadas en rojo.</td> 
     </tr> 
    </tbody> 
   </table>

   ![RP__user_allocation_chart_Dec._7__2017.png](assets/rp--user-allocation-chart-dec.-7--2017-350x148.png)

1. (Opcional) Haga clic en el área **Sobreasignación % para todos los usuarios** del gráfico.\
   Todos los usuarios sobreasignados aparecen resaltados en rojo.
1. (Opcional) Haga clic en el área **Porcentaje de infrautilización para todos los usuarios** del gráfico.\
   Todos los usuarios infrautilizados aparecen resaltados en azul.

1. (Opcional) Haga clic en el icono del indicador ![one_user_overallocation_marker.png](assets/one-user-overallocation-marker.png) que muestra dónde tiene al menos un usuario sobreasignado.\
   Los usuarios sobreasignados se resaltan en rojo.

1. (Opcional) Actualice la página para contraer el gráfico.
