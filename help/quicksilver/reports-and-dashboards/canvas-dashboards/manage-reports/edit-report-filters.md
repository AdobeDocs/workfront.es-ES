---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Edición de filtros de informes en un panel de lienzo
description: Puede editar los filtros de informe después de aplicarlos a un panel de lienzo.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: 5205c342-7f63-438e-97c8-e74f7dfecfd0
source-git-commit: 56d0b9281387cc7b35055461e7868c7e4a194f81
workflow-type: tm+mt
source-wordcount: '1048'
ht-degree: 44%

---

# Edición de filtros de informes en un panel de lienzo

>[!IMPORTANT]
>
>Actualmente, la función Paneles de lienzo solo está disponible para los usuarios que participan en la fase beta. Es posible que algunas partes de la función no estén completas o que no funcionen según lo previsto durante esta fase. Envíe cualquier comentario sobre su experiencia siguiendo las instrucciones de la sección [Proporcionar comentarios](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) del artículo Información general sobre la versión beta de los paneles de lienzo.<br>
>>Si tiene comentarios acerca de un posible error o problema técnico, envíe un ticket al equipo de asistencia de Workfront. Para obtener más información, consulte [Póngase en contacto con Atención al cliente](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>>Tenga en cuenta que esta versión beta no está disponible en los siguientes proveedores de la nube:
>
>* Traer su propia clave para Amazon Web Service
>* Azure
>* Google Cloud Platform

Puede editar los filtros de informe una vez que los haya aplicado a un panel de lienzo para actualizar los datos que se muestran a medida que avanza el proyecto.

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Plan de Adobe Workfront</p></td> 
   <td> 
<p>Cualquiera </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td> 
<p>Actual: plan </p> 
<p>Nuevo: estándar</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuraciones de nivel de acceso</p></td> 
   <td><p>Editar el acceso a Informes, Paneles de control y Calendarios</p>
  </td> 
  </tr>  
        <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td><p>Administración de permisos para el tablero</p>
  </td> 
  </tr>
</tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Requisitos previos

Debe agregar un filtro a un informe para poder editarlo.

## Edición de un filtro de informe

>[!NOTE]
>
>Hay muchas herramientas de configuración disponibles para crear y editar un filtro de informe. Para obtener más información sobre estas herramientas, consulte la siguiente sección en este artículo: [Consideraciones al editar un filtro de informe](#considerations-when-editing-a-report-filter).


{{step1-to-dashboards}}

1. En el panel izquierdo, haga clic en **Paneles de control de lienzo**.

1. En la página **Paneles de lienzo**, haga clic en el icono **Más** ![Más](assets/more-icon.png) en la esquina superior derecha del informe que contiene el filtro que desea editar y, a continuación, seleccione **Editar**.

   ![Editar un informe](assets/edit-report-box.png)

1. En la parte izquierda del cuadro de diálogo **Configurar**, seleccione el panel **Filtros**.

1. Haga clic en **Editar filtro**.

1. Seleccione el campo o el modificador que desea editar y, a continuación, ajuste las selecciones actuales según sea necesario.

   ![Agregar condición](assets/add-condition.png)

1. (Opcional) Haga clic en **Agregar grupo de filtros** para agregar otro conjunto de criterios de filtrado. El operador predeterminado entre los conjuntos es Y. Haga clic en el operador para cambiarlo a OR.

1. Haga clic en **Guardar**.

## Consideraciones al editar un filtro de informe

### Variables de filtro de comodines basados en fecha

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

### Variables de filtro comodín de usuario conectado

* Al filtrar por el atributo del usuario `name`, verá la opción **Yo (usuario conectado)**.

  ![Atributo de nombre de usuario](assets/user-name-attribute.png)

* Al filtrar un atributo del grupo `name`, verá las opciones **Mi grupo de inicio (Grupo de usuarios con sesión iniciada)** y **Mis otros grupos (Grupos de usuarios con sesión iniciada)** que se utilizarán en una condición de filtro.

  ![Atributo de nombre de grupo](assets/group-name-attribute.png)

* Al filtrar en un atributo de equipo `name`, verá las opciones de **Mi equipo predeterminado (Equipo de usuario con sesión iniciada)** y **Mis otros equipos (Equipos de usuario con sesión iniciada)** que puede elegir en la condición de filtro.

  ![Atributo de nombre de equipo](assets/team-name-attribute.png)


### Referencia a objetos secundarios

Las relaciones disponibles para columnas adicionales, opciones de filtro y atributos de agrupación generalmente se limitan a objetos superiores en la jerarquía de objetos de Workfront o tienen una sola selección en el objeto de entidad base del informe. Hay algunas excepciones a este respecto, que incluyen las siguientes:

* Proyecto > Tareas
* Aprobación de documento > Fases de aprobación de documento
* Fases de aprobación de documento > Participantes en la fase de aprobación de documento

Al utilizar cualquiera de las relaciones principal-secundario enumeradas anteriormente, verá una fila en la tabla para cada registro secundario conectado al objeto principal.

### Operadores de campo por tipo de campo

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
