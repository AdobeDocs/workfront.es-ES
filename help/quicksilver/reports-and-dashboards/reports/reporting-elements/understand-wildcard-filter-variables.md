---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: Variables de filtro comodín
description: Mediante el uso de comodines en los filtros, puede hacer referencia a un usuario o una fecha genéricos en lugar de a un usuario o fecha específicos. De este modo, los elementos que genera son dinámicos y los resultados cambian según el contexto en el que se utilicen.
author: Nolan
feature: Reports and Dashboards
exl-id: f99cd99e-c4c1-471d-8428-c680f0e73336
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '1447'
ht-degree: 1%

---

# Variables de filtro comodín

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: This article is linked to the training self-serve promted articles for user-based and date-based widlcards (how-to articles). This serves as the "overview/ reference" article for those articles. Consider renaming this when that is allowed.) </p>
<p>(NOTE: Alina: ***&gt;&gt;Linked in other articles - do not move/ delete.</p>
<p>&gt;&gt;This was included but it is not supported???:</p>
<p>The $$USER.roleIDs variable refers to all the job roles that are associated with the logged-in user. Using this variable, you can&nbsp; items assigned to all of the job roles associated with the logged-in user.</p>
<p>For example, if you want to display tasks assigned to any of the job roles associated with the logged-in user, you can use the following filter rule in a task filter:</p>
<p>AssignedToID Equals $$USER.roleIDs.)</p>
</div>
-->

Adobe Workfront admite variables de filtro o caracteres comodín al crear los siguientes elementos:

* Filtros de listas, informes y el planificador de recursos

   Para obtener información sobre los filtros de Workfront, consulte el artículo [Información general sobre filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* Búsquedas avanzadas

   Para obtener información sobre las búsquedas avanzadas, consulte la sección [Usar la búsqueda avanzada](../../../workfront-basics/navigate-workfront/search/search-workfront.md#using-advanced-search) en el artículo [Buscar en Adobe Workfront](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

* Columnas calculadas en vistas
* Formato condicional en vistas

   Para obtener información sobre el formato condicional, consulte el artículo [Utilizar el formato condicional en las vistas](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

* Campos personalizados calculados

   >[!NOTE]
   >
   >Las variables de filtro comodín no son compatibles cuando se hace referencia a colecciones anidadas en una columna calculada.

   Para obtener información sobre los campos y columnas personalizados calculados, consulte el artículo [Campos personalizados calculados vs. columnas calculadas](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

Con los comodines puede hacer referencia a un usuario o fecha genéricos en lugar de a un usuario o fecha específicos. De este modo, los elementos que genera son dinámicos y los resultados cambian según el contexto en el que se utilicen.

Por ejemplo, al filtrar por $$USER.homeGroupID en un informe de proyecto, se recuperan solo los proyectos asociados al grupo de inicio del usuario que ha iniciado sesión.

Puede utilizar variables de filtro basadas en datos o en usuarios en Workfront.

## Variables de filtro comodín basadas en fechas

Las opciones de comodín basadas en datos de Workfront se pueden usar en combinación con cualquier atributo de filtro de fecha.

Para obtener información sobre cómo agregar un comodín basado en datos a un informe, consulte el artículo [Utilice caracteres comodín basados en datos para generalizar informes](../../../reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

>[!NOTE]
>
>Si crea un cálculo de fecha y hora que no incluye una parte de tiempo, o que utiliza los comodines de fecha $$TODAY o $$Now, el sistema utiliza la fecha según la zona de Hora Universal Coordinada (UTC), no según la zona horaria local. Esto puede provocar un resultado de fecha inesperado.

Elija entre los siguientes comodines basados en datos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$HOY</strong> </p> </td> 
   <td> <p>Se recomienda crear filtros que distingan fechas utilizando este comodín para evitar crear el filtro de nuevo mañana, la semana siguiente o el mes siguiente.</p> <p>Por ejemplo, si desea mostrar todas las tareas que vencen antes de hoy, puede utilizar la siguiente regla en un filtro de tareas: <em>Fecha de inicio planeada inferior a $$TODAY</em>.</p> <p>$$TODAY es siempre igual a medianoche para el día actual.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$AHORA</strong> </p> </td> 
   <td> <p>Esto es similar al comodín $$TODAY , pero incluye la fecha y la hora actuales. $$AHORA es igual a la fecha y hora actuales.</p> <p>Por ejemplo, si desea mostrar todas las entradas de hora proporcionadas hasta la hora actual, puede hacerlo utilizando la siguiente regla en un filtro de hora: <em>Fecha de inicio planeada inferior a $$AHORA</em>.</p> <p>Nota: Este comodín no se admite en el planificador de recursos.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para indicar varios períodos de tiempo y distintos puntos en el tiempo (futuro o pasado), se pueden combinar caracteres comodín con los siguientes:

| Atributos |   |
|---|---|
| **q** | trimestre del calendario |
| **h** | hora |
| **d** | día |
| **w** | semana |
| **m** | mes |
| **y** | año |

{style="table-layout:auto"}

| **Cualificadores** |  |
|---|---|
| **b** | inicio de la semana (domingo) |
| **e** | final de semana (sábado) |

{style="table-layout:auto"}

| **Operadores** |  |
|---|---|
| **+** | añadir valor al valor comodín |
| **-** | restar valor del valor comodín |

{style="table-layout:auto"}

Por ejemplo, el comodín `$$TODAYb+2w` hace referencia a &quot;2 semanas desde el comienzo de esta semana&quot;. El comodín *`$$NOW+2h` hace referencia a &quot;2 horas a partir de ahora&quot;.

## Variables de filtro comodín basadas en el usuario

>[!IMPORTANT]
>
>Si un filtro o informe contiene una variable de filtro comodín basada en el usuario, los resultados siempre muestran información filtrada por el usuario que actualmente ha iniciado sesión. Cuando comparte este filtro o informe con otro usuario, el comodín recupera información para el usuario que ve el informe. Los dos usuarios ven resultados diferentes.

Para obtener información sobre cómo agregar un comodín basado en el usuario a un informe, consulte el artículo [Utilice caracteres comodín basados en el usuario para generalizar informes](../../../reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md).

Workfront proporciona las siguientes variables basadas en usuarios:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="200" role="rowheader"> <p><strong>$$USER.ID</strong> </p> </td> 
   <td> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : should these be formatted with code?!) </p>
    --> <p>La variable basada en usuarios más común es $$USER.ID. Esto siempre devuelve el ID del usuario que ha iniciado sesión. Este es el ID utilizado para identificar qué usuario creó cada objeto y sus asignaciones de trabajo.</p> <p>Cuando se utiliza en los informes, este comodín reduce el número de informes que debe crear en el sistema. Puede crear un informe y compartirlo con varios usuarios, y los resultados cambiarán según el usuario que haya iniciado sesión y observe el informe.</p> <p>Por ejemplo, para crear un informe de todos los problemas asignados al usuario que ha iniciado sesión, puede utilizar la siguiente regla en un filtro de problemas: <em>Asignado a ID igual a $$USER.ID</em>.</p> <p>Workfront utiliza esta variable en los siguientes filtros integrados:</p> 
    <ul> 
     <li>Mis informes</li> 
     <li>Mis proyectos</li> 
     <li>Mis tareas</li> 
     <li>Mis problemas</li> 
     <li>Mis horas</li> 
    </ul> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="200" role="rowheader"> <p><strong>$$USER.categoryID</strong> </p> </td> 
   <td> <p>La variable $$USER.categoryID hace referencia a un formulario personalizado específico asociado al usuario que ha iniciado sesión.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.accessLevelID</strong> </p> </td> 
   <td> <p>La variable $$USER.accessLevelID hace referencia al ID del nivel de acceso asociado al usuario que ha iniciado sesión.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.accessLevelRank</strong> </p> </td> 
   <td> <p>La variable $$USER.accessLevelRank hace referencia a la clasificación de nivel de acceso asociada al usuario que ha iniciado sesión.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.companyID</strong> </p> </td> 
   <td> <p>La variable $$USER.companyID hace referencia a la empresa asociada al usuario que ha iniciado sesión.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.customerID</strong> </p> </td> 
   <td> <p>La variable $$USER.customerID hace referencia al ID de la cuenta de cliente asociada a su entorno. Para su entorno, solo hay un valor posible para esta variable y normalmente se utiliza solo al crear integraciones a través de la API.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.firstName</strong> </p> </td> 
   <td> <p>La variable $$USER.firstName hace referencia al nombre del usuario que ha iniciado sesión.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.lastName</strong> </p> </td> 
   <td> <p>La variable $$USER.lastName hace referencia al apellido del usuario que ha iniciado sesión.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.name</strong> </p> </td> 
   <td> <p>La variable $$USER.name hace referencia al nombre completo del usuario que ha iniciado sesión.</p> <p>Nota:   <p>Esta variable comodín solo funciona al modificar un filtro en modo de texto. No puede utilizar este comodín en filtros que no admiten el modo de texto. Por ejemplo, no se puede usar este comodín en los filtros de las siguientes áreas:</p> 
     <ul> 
      <li> <p>Planificador de recursos</p> </li> 
      <li> <p>Distribuidor de cargas de trabajo</p> </li> 
      <li> <p>Análisis</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeGroupID</strong> </p> </td> 
   <td> <p>La variable $$USER.homeGroupID hace referencia al ID del grupo de inicio del usuario que ha iniciado sesión. Como administrador de grupos, puede usar esta variable para filtrar solo los elementos que pertenezcan a los usuarios de su grupo de inicio.</p> <p>Por ejemplo, para ver todas las tareas incompletas de los proyectos del grupo de finanzas, utilice las siguientes reglas de filtro en un filtro de tareas:<br><em>Proyecto: ID de grupo igual a $$USER.homeGroupID </em><br><em>Porcentaje completado inferior a 100</em></p> <p>Para ver todas las tareas incompletas asignadas a personas de un grupo específico que es el grupo principal del usuario que ha iniciado sesión, utilice las siguientes reglas de filtro en un filtro de tareas:</p> <p><em>Asignado a: ID de grupo igual a $$USER.homeGroupID<br>Porcentaje completado inferior a 100</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.otherGroupIDs</strong> </p> </td> 
   <td> <p>La variable $$USER.otherGroupIDs hace referencia a todos los grupos (incluido el grupo principal) asociados al perfil del usuario que ha iniciado sesión.</p> <p>La funcionalidad de esta variable es similar a la de la variable $$USER.homeGroupID , excepto que los resultados muestran información sobre los usuarios que pertenecen a cualquiera de los grupos asociados con el usuario que ha iniciado sesión.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeTeamID</strong> </p> </td> 
   <td> <p>La variable $$USER.homeTeamID hace referencia al ID del equipo principal del usuario que ha iniciado sesión. Como administrador de equipos, puede usar esta variable para filtrar solo los elementos que pertenezcan a los usuarios de su equipo de inicio.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.teamIDs</strong> </p> </td> 
   <td> <p>La variable $$USER.teamIDs devuelve una lista de todos los equipos asociados con el usuario que ha iniciado sesión.</p> <p>La funcionalidad de esta variable es similar a la de la variable $$USER.homeTeamID , excepto que los resultados muestran información sobre el usuario que pertenece a cualquiera de los equipos identificados en el filtro.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.roleID</strong> </p> </td> 
   <td> <p>La variable $$USER.roleID hace referencia a la función principal del usuario que ha iniciado sesión. Con esta variable, puede crear informes sobre tareas o problemas asignados a una función de trabajo específica.</p> <p>Por ejemplo, para ver todas las tareas asignadas a la función principal del usuario que ha iniciado sesión, puede utilizar la siguiente regla de filtro en un filtro de tareas:</p> <p><em>Tarea: Id. de función es igual a $$USER.roleID.</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader">$$USER.roleIDs</td> 
   <td> <p>La variable $$USER.roleIDs hace referencia a todas las funciones de trabajo asociadas con el usuario que ha iniciado sesión. Con esta variable, puede crear informes sobre las tareas o los problemas asignados a cualquiera de las funciones de trabajo asociadas con el usuario que ha iniciado sesión. </p> <p>Por ejemplo, para ver todas las tareas asignadas a cualquiera de las funciones asociadas con el usuario que ha iniciado sesión, puede utilizar la siguiente regla de filtro en un filtro de tareas:</p> <p><i>Tarea: ID de función igual a $$USERID.roleIDs<br></i> </p> <p>Sugerencia: La variable <i>Tarea: ID de función igual a $$USERID.roleIDs</i> la regla de filtro existe en los filtros integrados Tareas no asignadas en Mi rol y Problemas no asignados en mi rol. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Variables de filtro de comodín basadas en objetos

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><b>$$OBJCODE</b> </td> 
   <td> 
    <div> 
     <p>La variable $$OBJCODE hace referencia al tipo de objeto. </p> 
     <p>En un formulario personalizado, cuando los tipos de objeto seleccionados del formulario son incompatibles con un campo al que se hace referencia en un campo personalizado calculado, se puede utilizar este comodín para evitar la solución de crear formularios duplicados para esos tipos de objeto.</p> 
     <p>En el campo personalizado calculado, puede hacerlo incluyendo el comodín en una expresión IF para que el cálculo pueda generar valores diferentes para cada uno de los tipos de objeto del formulario. </p> 
     <p>Para obtener más información y ver un ejemplo, consulte la sección <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#calculat" class="MCXref xref">Campos personalizados calculados en formularios personalizados con varios objetos</a> en el artículo <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">Agregar datos calculados a un formulario personalizado</a>.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>
