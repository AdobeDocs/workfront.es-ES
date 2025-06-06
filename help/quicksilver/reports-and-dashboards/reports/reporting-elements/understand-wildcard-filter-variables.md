---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: Variables de filtro comodín
description: Mediante el uso de comodines en los filtros, se puede hacer referencia a un usuario o fecha genéricos en lugar de a un usuario o fecha específica. De este modo, los elementos que cree serán dinámicos y los resultados cambiarán según el contexto en el que se utilicen.
author: Nolan
feature: Reports and Dashboards
exl-id: f99cd99e-c4c1-471d-8428-c680f0e73336
source-git-commit: 577761ff5d1fb59db104df5995af953a0b5e6c0c
workflow-type: tm+mt
source-wordcount: '1439'
ht-degree: 100%

---

# Información general sobre las variables de filtro comodín

<!-- Audited: 11/2024 -->

<!--(NOTE: This article is linked to the training self-serve promoted articles for user-based and date-based wildcards (how-to articles). This serves as the "overview/ reference" article for those articles. Consider renaming this when that is allowed.)
(NOTE: Alina: ***&gt;&gt;Linked in other articles - do not move/ delete.
This was included but it is not supported???:
The $$USER.roleIDs variable refers to all the job roles that are associated with the logged-in user. Using this variable, you can&nbsp; items assigned to all of the job roles associated with the logged-in user.
For example, if you want to display tasks assigned to any of the job roles associated with the logged-in user, you can use the following filter rule in a task filter:
AssignedToID Equals $$USER.roleIDs.)-->

Con los comodines, se puede hacer referencia a un usuario o fecha genéricos en lugar de a un usuario o fecha específica. De este modo, los elementos que se generan son dinámicos; los resultados cambian en función del contexto en el que se utilizan.

Por ejemplo, si se filtra $$USER.homeGroupID en un informe de proyecto, se recuperan únicamente los proyectos asociados al grupo de inicio del usuario que ha iniciado sesión.

Puede utilizar variables de filtro (también conocidas como comodines) al crear los siguientes elementos:

<table>
    <tr>
        <td>Filtros en listas, informes y el Planificador de recursos</td>
        <td>Para obtener más información sobre los filtros de Workfront, consulte el artículo <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md">Información general sobre los filtros</a>.
</td>
    </tr>
    <tr>
        <td>Búsquedas avanzadas</td>
        <td>Para obtener información acerca de las búsquedas avanzadas, consulte la sección <a href="../../../workfront-basics/navigate-workfront/search/search-workfront.md#using-advanced-search">Utilizar la búsqueda avanzada</a> en el artículo <a href="../../../workfront-basics/navigate-workfront/search/search-workfront.md">Buscar en Adobe Workfront</a>.
    </tr>
    <tr>
        <td>Columnas calculadas en vistas</td>
        <td></td>
    </tr>
    <tr>
        <td>Formato condicional en vistas</td>
        <td>Para obtener información acerca del formato condicional, consulte el artículo <a href="../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md">Usar formato condicional en vistas</a>.
    </tr>
    <tr>
        <td>Campos personalizados calculados</td>
        <td>No se admiten variables de filtro comodín cuando se hace referencia a colecciones anidadas en una columna calculada.

Para obtener información sobre los campos y columnas personalizados calculados, consulte el artículo <a hreft="../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md">Campos personalizados calculados frente a columnas calculadas</a>.
</td>
    </tr>
</table>

## Variables de filtro comodín basadas en fechas

Las opciones de carácter comodín basadas en fechas se pueden utilizar en combinación con cualquier atributo de filtro de fecha. Para obtener información acerca de cómo añadir un comodín basado en fecha a un informe, consulte el artículo [Usar comodines basados en fecha para generalizar informes](../../../reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

>[!NOTE]
>
>Si crea un cálculo de fecha y hora que no incluye una parte de hora o que utiliza los caracteres comodín de fecha $$TODAY o $$NOW, el sistema utilizará la fecha según la zona horaria universal coordinada (UTC), no según la zona horaria local. Esto puede provocar un resultado de fecha inesperado.

Puede elegir entre los siguientes comodines basados en fechas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$TODAY</strong> </p> </td> 
   <td> <p>Le recomendamos que genere filtros con distinción de fechas utilizando este comodín para evitar volver a generar el filtro mañana, la semana que viene o el mes que viene.</p> <p>Por ejemplo, si desea mostrar todas las tareas que vencen antes de hoy, puede usar la siguiente regla en un filtro de tareas: <em>Fecha planificada de inicio menor que $$TODAY</em>.</p> <p>$$TODAY siempre equivale a la medianoche del día actual.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$NOW</strong> </p> </td> 
   <td> <p>Es similar al comodín $$TODAY, pero incluye la fecha y la hora actuales. $$NOW es igual a la fecha y hora actuales.</p> <p>Por ejemplo, si desea mostrar todas las entradas de horas proporcionadas hasta la hora actual, puede hacerlo usando la siguiente regla en un filtro de horas: <em>Fecha planificada de inicio inferior a $$NOW</em>.</p> <p>Nota: Este comodín no es compatible con el Planificador de recursos.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para indicar varios periodos de tiempo y varios puntos en el tiempo (futuros o pasados), puede combinar los caracteres comodín anteriores con lo siguiente:

| Atributos |   |
|---|---|
| **q** | trimestre natural |
| **h** | hora |
| **d** | día |
| **w** | semana |
| **m** | mes |
| **y** | año |

{style="table-layout:auto"}

| **Calificadores** | |
|---|---|
| **b** | inicio del período (sin un atributo especificado, el valor predeterminado es el inicio de la semana: domingo) |
| **e** | final del período (sin un atributo especificado, el valor predeterminado es el fin de semana: sábado) |

{style="table-layout:auto"}

| **Operadores** | |
|---|---|
| **+** | añadir valor al valor comodín |
| **-** | restar valor de valor comodín |

{style="table-layout:auto"}

Por ejemplo, el comodín `$$TODAYb+2w` hace referencia a “2 semanas a partir del inicio de esta semana”. El comodín *`$$NOW+2h` hace referencia a “2 horas a partir de ahora”.

## Variables de filtro comodín basadas en el usuario

>[!IMPORTANT]
>
>Si un filtro o informe contiene una variable de filtro comodín basada en el usuario, los resultados siempre muestran información filtrada por el usuario que ha iniciado sesión en ese momento. Cuando comparte un filtro o informe de este tipo con otro usuario, el comodín recupera información para el usuario que consulta el informe. Los dos usuarios ven resultados diferentes.
>
>Para obtener información acerca de cómo añadir un comodín basado en el usuario a un informe, consulte el artículo [Usar comodines basados en el usuario para generalizar informes](../../../reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md).

Puede elegir entre las siguientes variables basadas en el usuario:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="200" role="rowheader"> <p><strong>$$USER.ID</strong> </p> </td> 
   <td> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : should these be formatted with code?!) </p>
    --> <p>La variable basada en el usuario más común es $$USER.ID. Esto siempre devuelve el ID del usuario que ha iniciado sesión. Identificador que se utiliza para identificar qué usuario creó cada objeto y sus asignaciones de trabajo.</p> <p>Cuando se utiliza en los informes, este comodín reduce el número de informes que debe crear en el sistema. Puede crear un informe y compartirlo con varios usuarios, y los resultados cambian según el usuario que ha iniciado sesión y está viendo el informe.</p> <p>Por ejemplo, para generar un informe con todos los problemas asignados al usuario que ha iniciado sesión, puede usar la siguiente regla en un filtro de problemas: <em>Asignado a ID es igual a $$USER.ID</em>.</p> <p>Workfront utiliza esta variable en los siguientes filtros integrados:</p> 
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
   <td> <p>La variable $$USER.companyID hace referencia a la compañía asociada al usuario que ha iniciado sesión.</p> </td> 
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
   <td> <p>La variable $$USER.name hace referencia al nombre completo del usuario que ha iniciado sesión.</p> <p>Nota:   <p>Esta variable comodín solo funciona cuando se modifica un filtro en modo de texto. No puede utilizar este comodín en filtros que no admiten el modo de texto. Por ejemplo, no puede utilizar este comodín en los filtros de las siguientes áreas:</p> 
     <ul> 
      <li> <p>Planificador de recursos</p> </li> 
      <li> <p>Distribuidor de cargas de trabajo</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeGroupID</strong> </p> </td> 
   <td> <p>La variable $$USER.homeGroupID hace referencia al ID del grupo de inicio del usuario que ha iniciado sesión. Como administrador de grupos, puede utilizar esta variable para filtrar únicamente los elementos que pertenezcan a los usuarios del grupo de inicio.</p> <p>Por ejemplo, para ver todas las tareas incompletas de los proyectos del grupo de finanzas, use las siguientes reglas de filtro en un filtro de tareas:<br><em>Proyecto: el ID de grupo es igual a $$USER.homeGroupID </em><br><em>Porcentaje completado menor que 100</em></p> <p>Para ver todas las tareas incompletas asignadas a personas de un grupo específico, que es el grupo de inicio del usuario que ha iniciado sesión, utilice las siguientes reglas de filtro en el filtro de tareas:</p> <p><em>Asignado a: ID de grupo es igual a $$USER.homeGroupID<br>Porcentaje completado menor que 100</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.otherGroupIDs</strong> </p> </td> 
   <td> <p>La variable $$USER.otherGroupIDs hace referencia a todos los grupos (incluido el grupo de inicio) asociados al perfil del usuario que ha iniciado sesión.</p> <p>La funcionalidad de esta variable es similar a la de la variable $$USER.homeGroupID, excepto que los resultados muestran información sobre los usuarios que pertenecen a cualquiera de los grupos asociados con el usuario que ha iniciado sesión.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeTeamID</strong> </p> </td> 
   <td> <p>La variable $$USER.homeTeamID hace referencia al ID del equipo de inicio del usuario que ha iniciado sesión. Como administrador de equipo, puede utilizar esta variable para filtrar solo los elementos que pertenezcan a los usuarios de su equipo de inicio.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.teamIDs</strong> </p> </td> 
   <td> <p>La variable $$USER.teamIDs devuelve una lista de todos los equipos asociados con el usuario que ha iniciado sesión.</p> <p>La funcionalidad de esta variable es similar a la de la variable $$USER.homeTeamID, excepto que los resultados muestran información sobre el usuario que pertenece a cualquiera de los equipos identificados en el filtro.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.roleID</strong> </p> </td> 
   <td> <p>La variable $$USER.roleID hace referencia a la función principal del usuario que ha iniciado sesión. Con esta variable, puede informar sobre tareas o problemas asignados a una función específica.</p> <p>Por ejemplo, para ver todas las tareas asignadas a la función principal del usuario que ha iniciado sesión, puede utilizar la siguiente regla de filtro en un filtro de tareas:</p> <p><em>Tarea: ID de función es igual a $$USER.roleID.</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"><p><strong>$$USER.roleIDs</strong></p></td> 
   <td> <p>La variable $$USER.roleIDs hace referencia a todas las funciones de trabajo asociadas al usuario que ha iniciado sesión. Con esta variable, puede generar informes sobre las tareas o los problemas asignados a cualquiera de las funciones asociadas con el usuario que ha iniciado sesión. </p> <p>Por ejemplo, para ver todas las tareas asignadas a cualquiera de las funciones asociadas con el usuario que ha iniciado sesión, puede utilizar la siguiente regla de filtro en un filtro de tareas:</p> <p><i>Task: Role ID Equals $$USERID.roleIDs<br></i> </p> <p>Sugerencia: La regla de filtro <i>Task: Role ID Equals $$USERID.roleIDs</i> existe en los filtros integrados Tareas sin asignación en Mi función y Problemas sin asignación en Mi función. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Variables de filtro comodín basadas en objetos

Puede elegir entre los siguientes comodines basados en objetos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><b>$$OBJCODE</b> </td> 
   <td> 
    <div> 
     <p>La variable $$OBJCODE hace referencia al tipo de un objeto. </p> 
     <p>En un formulario personalizado, cuando los tipos de objeto seleccionados del formulario son incompatibles con un campo al que se hace referencia en un campo personalizado calculado, puede utilizar este comodín para evitar la solución alternativa de crear formularios duplicados para esos tipos de objeto.</p> 
     <p>En el campo personalizado calculado, puede hacerlo incluyendo el comodín en una expresión IF para que el cálculo pueda generar valores diferentes para cada uno de los tipos de objeto del formulario. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>
