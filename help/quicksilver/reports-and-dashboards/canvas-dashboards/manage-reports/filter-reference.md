---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Referencia del filtro de informes para paneles de lienzo
description: Referencia para los campos, operadores, comodines y reglas especiales que puede utilizar al filtrar un informe en un panel de lienzo.
author: Courtney
feature: Reports and Dashboards
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: dc9caae8cc85543986eaefb1d3debdebfdf6ce96
workflow-type: tm+mt
source-wordcount: '1210'
ht-degree: 34%
---
# Referencia del filtro de informes para paneles de lienzo

>[!IMPORTANT]
>
>Actualmente, la función Paneles de lienzo solo está disponible para los usuarios que participan en la fase beta. Es posible que algunas partes de la función no estén completas o que no funcionen según lo previsto durante esta fase. Envíe cualquier comentario sobre su experiencia siguiendo las instrucciones de la sección [Proporcionar comentarios](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) del artículo Información general sobre la versión beta de los paneles de lienzo.<br>
>Si tiene comentarios acerca de un posible error o problema técnico, envíe un ticket al equipo de asistencia de Workfront. Para obtener más información, consulte [Contacto con el servicio de asistencia al cliente](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Tenga en cuenta que esta versión beta no está disponible en los siguientes proveedores de la nube:
>
>* Traer su propia clave para Amazon Web Service
>* Azure
>* Google Cloud Platform

Este artículo describe los campos, operadores, caracteres comodín y reglas especiales disponibles al filtrar un informe. Para ver los pasos para crear o editar un filtro, consulte [Filtrar un informe en un panel de lienzo](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-reports/filter-a-report.md).

## Operadores de campo por tipo de campo

+++ Amplíe para ver la lista de operadores de campo por tipo de campo. 

<table>
    <tr>
        <td><b>Tipo de campo</b></td>
        <td><b>Ejemplo</b></td>
       <td><b>Operadores</b></td>
        <td><b>Comodines</b></td>
    </tr>
    <tr>
        <td>Nombre de objeto/referencia</td>
        <td>Cualquier atributo de nombre nativo o búsqueda personalizada</td>
              <td><ul>
        <li>Igual (no distingue mayúsculas y minúsculas)</li>
        <li>No es igual</li>
        <li>Contiene</li>
          <li>No contiene</li>
            <li>Es nulo</li>
              <li>No es nulo</li>
        </ul></td>
        <td>Usuario: nombre
        <ul>
        <li>Yo (usuario con sesión iniciada)</li>
        </ul>
        Grupo: nombre
        <ul>
          <li>Mi grupo de inicio (grupo de usuarios con sesión iniciada)</li>
            <li>Mis otros grupos (grupos de usuarios con sesión iniciada)</li>
          </ul>
          Equipo: Nombre
                  <ul>
          <li>Mi equipo predeterminado (equipo de usuarios con sesión iniciada)</li>
            <li>Mis otros equipos (equipos de usuarios con sesión iniciada)</li>
          </ul>
        </td>
    </tr>
    <tr>
        <td>Entrada de texto/cadena </td>
                <td>Proyecto: Descripción</td>
                      <td><ul>
             <li>Igual (no distingue mayúsculas y minúsculas)</li>
        <li>No es igual</li>
        <li>Contiene</li>
          <li>No contiene</li>
            <li>Es nulo</li>
              <li>No es nulo</li>
        </ul></td>
        <td></td>
    </tr>
    <tr>
        <td>Entero/Doble</td>
             <td>Proyecto: Horas planificadas
        <br>Tarea: Porcentaje completado</td>
              <td><ul>
        <li>Igual (no distingue mayúsculas y minúsculas)</li>
        <li>No es igual</li>
        <li>Mayor que</li>
          <li>Mayor o igual que</li>
          <li>Menor que</li>
          <li>Menor o igual que</li>
            <li>Es nulo</li>
              <li>No es nulo</li>
        </ul></td>
        <td></td>
    </tr>
       <tr>
        <td> Fecha / Fecha y hora </td>
                    <td>Proyecto: Fecha planificada de inicio
        <br>Hora: Fecha de entrada</td>
              <td><ul>
        <li>Igual (no distingue mayúsculas y minúsculas)</li>
        <li>No es igual</li>
        </ul></td>
        <td>Al alternar la opción <b>Establecer fecha relativa</b>, puede aplicar caracteres comodín de fecha relativa para que el informe sea más dinámico y se ajuste automáticamente en función de periodos de fecha comunes. 
         <ul><li>$$TODAY</li>
         <li>$$NOW</li>
         </ul>
        </td>
    </tr>
       <tr>
        <td>Booleano </td>
                  <td>Proyecto: Tiene documentos
        <br>Tarea: Es Crítica
        Usuario <br>: está activo</td>
        <td><ul>
        <li>Igual (no distingue mayúsculas y minúsculas)</li>
        <li>No es igual</li>
        </ul></td>
        <td> </td>
    </tr>
   </table>

+++

## Variables de filtro comodín basadas en fechas

Las opciones de carácter comodín basadas en fechas se pueden utilizar en combinación con cualquier atributo de filtro de fecha. Para obtener información sobre cómo agregar un comodín basado en fecha a un informe, consulte [Usar comodines basados en fecha para generalizar informes](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

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
   <td> <p>Le recomendamos que genere filtros con distinción de fechas utilizando este comodín para evitar volver a generar el filtro mañana, la semana que viene o el mes que viene.</p> <p>Por ejemplo, si desea mostrar todas las tareas que vencen antes de hoy, puede usar la siguiente regla en un filtro de tareas: <em>Fecha de inicio planificada menor que $$TODAY</em>.</p> <p>$$TODAY siempre equivale a la medianoche del día actual.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$NOW</strong> </p> </td> 
   <td> <p>Es similar al comodín $$TODAY, pero incluye la fecha y la hora actuales. $$NOW es igual a la fecha y hora actuales.</p> <p>Por ejemplo, si desea mostrar todas las entradas de horas proporcionadas hasta la hora actual, puede hacerlo usando la siguiente regla en un filtro de horas: <em>Fecha de inicio planificada inferior a $$NOW</em>.</p> <p>Nota: Este comodín no es compatible con el Planificador de recursos.</p> </td> 
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

| **Calificadores** |   |
|---|---|
| **b** | inicio del período (sin un atributo especificado, el valor predeterminado es el inicio de la semana: domingo) |
| **e** | final del período (sin un atributo especificado, el valor predeterminado es el fin de semana: sábado) |

{style="table-layout:auto"}

| **Operadores** |   |
|---|---|
| **+** | añadir valor al valor comodín |
| **-** | restar valor de valor comodín |

{style="table-layout:auto"}

Por ejemplo, el comodín `$$TODAYb+2w` hace referencia a “2 semanas a partir del inicio de esta semana”. El comodín `$$NOW+2h` hace referencia a &quot;2 horas a partir de ahora&quot;.

## Variables de filtro comodín de usuario conectado

* Al filtrar por el atributo del usuario `name`, verá la opción **Yo (usuario conectado)**.

  ![Atributo de nombre de usuario](assets/user-name-attribute.png)

* Al filtrar un atributo del grupo `name`, verá las opciones **Mi grupo de inicio (Grupo de usuarios con sesión iniciada)** y **Mis otros grupos (Grupos de usuarios con sesión iniciada)** que se utilizarán en una condición de filtro.

  ![Atributo de nombre de grupo](assets/group-name-attribute.png)

* Al filtrar en un atributo de equipo `name`, verá las opciones de **Mi equipo predeterminado (Equipo de usuario con sesión iniciada)** y **Mis otros equipos (Equipos de usuario con sesión iniciada)** que puede elegir en la condición de filtro.

  ![Atributo de nombre de equipo](assets/team-name-attribute.png)

## Referencia a objetos secundarios

Las relaciones disponibles para columnas adicionales, opciones de filtro y atributos de agrupación generalmente se limitan a objetos superiores en la jerarquía de objetos de Workfront o tienen una sola selección en el objeto de entidad base del informe. Hay algunas excepciones a este respecto, que incluyen las siguientes:

* Proyecto > Tareas
* Aprobación de documento > Fases de aprobación de documento
* Fases de aprobación de documento > Participantes en la fase de aprobación de documento

Al utilizar cualquiera de las relaciones principal-secundario enumeradas anteriormente, verá una fila en la tabla para cada registro secundario conectado al objeto principal.

<div class="preview">

## Filtro en las relaciones de colección en la vista previa

Una colección es un campo que se vincula a un grupo de registros relacionados en lugar de a un único registro. Por ejemplo, los participantes en las fases de aprobación de un proyecto son una colección. Al generar un filtro, puede filtrar colecciones directamente, sin cambiar al modo de texto.

Para filtrar una colección, abra el panel Seleccionar un campo y, a continuación, seleccione Colecciones. Esta sección enumera únicamente las relaciones de colección. Las relaciones de registro único permanecen en Relaciones.

![relaciones de colección](assets/collections.png)

Después de seleccionar una colección, puede hacer dos cosas:

* Filtre por los campos propios de la colección. Por ejemplo, desde los proyectos de un portafolio, puede filtrar el estado de un proyecto.
* Seguir una relación de registro único de la colección. Por ejemplo, desde los proyectos de un portafolio, puede llegar al propietario del proyecto.

Las colecciones no admiten una navegación más profunda. No se puede abrir una colección anidada dentro de otra, seguir más de una relación o seleccionar la relación que lleva al punto de inicio.

La sección Colecciones solo aparece cuando genera un filtro. No aparece en otros selectores de campos, como los de columnas de tabla, agrupaciones o campos de gráfico.

</div>

## Excluir proyectos personales, tareas y usuarios de bots

>[!NOTE]
>
>Si un informe de paneles de lienzo devuelve más resultados de lo esperado en comparación con un informe clásico similar, es posible que se incluyan proyectos personales, tareas personales o usuarios de bots de forma predeterminada. Añada una condición de filtro para excluirlos.

En los informes Proyecto y tarea de paneles de lienzo, el filtro `isPersonal` no se aplica automáticamente, por lo que los proyectos personales y las tareas personales se incluyen en los resultados de forma predeterminada. Para excluirlos, agregue una condición de filtro como `isPersonal=false`.

Del mismo modo, los informes de usuario de los paneles de lienzo incluyen a todos los usuarios de forma predeterminada, incluidos los colaboradores de IA (usuarios de bots). Para excluir usuarios de bots, agregue una condición de filtro como `isBot=false`.

Los informes clásicos de proyectos y tareas excluyen automáticamente los proyectos personales y las tareas personales, y los informes clásicos de usuarios excluyen automáticamente a los usuarios de bots. Para incluirlos en un informe clásico, agregue una condición de filtro como `isPersonal=true` (solo elementos personales) o `isPersonal_Mod=notnull` (elementos personales y no personales).
