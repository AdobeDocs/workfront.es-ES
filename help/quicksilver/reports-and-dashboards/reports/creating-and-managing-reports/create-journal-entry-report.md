---
title: Informe del área de actualizaciones con un informe de entrada de diario
description: El informe Entrada de cuaderno muestra las actualizaciones del sistema desde el área Actualizaciones de proyectos, tareas, problemas y otros objetos que anteriormente solo estaban disponibles a través de la API de Adobe Workfront. Aunque se trata de un informe avanzado diseñado para casos de uso específicos, el formato más asequible facilita la elaboración de informes sobre la actividad del proyecto y las actualizaciones del sistema en Workfront.
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: ecf947ce-54d8-4103-8903-f455b1d86c39
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '2763'
ht-degree: 94%

---

# Informe del área de Actualizaciones con un informe de Entrada de cuaderno

<!-- Audited: 11/2024 -->

El informe Entrada de cuaderno muestra las actualizaciones del sistema desde el área Actualizaciones de proyectos, tareas, problemas y otros objetos que anteriormente solo estaban disponibles a través de la API de Adobe Workfront. Aunque se trata de un informe avanzado diseñado para casos de uso específicos, el formato más asequible facilita la elaboración de informes sobre la actividad del proyecto y las actualizaciones del sistema en Workfront.

>[!TIP]
>
>El informe Entrada de cuaderno solo contiene actualizaciones del sistema en el área de Actualizaciones de objetos. Para informar sobre los comentarios que se dejan en el área de Actualizaciones, debe utilizar el informe Nota.\
>Para obtener más información sobre el informe Nota, consulte [Ver todas las actualizaciones en un informe Nota](../../../workfront-basics/updating-work-items-and-viewing-updates/view-all-updates-in-a-report.md).

El informe Entrada de cuaderno puede mostrar lo siguiente:

* Cuántos cambios de estado se han producido
* Eliminación de una tarea o un problema
* Cambio de los valores de los campos personalizados importantes a lo largo del ciclo de vida de un proyecto
* Cambio de fechas importantes durante el ciclo de vida de un proyecto
* Si el propietario de un proyecto ha cambiado

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
      <p>Estándar</p>
      <p>Plan</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuración de nivel de acceso</td> 
   <td> <p>Acceso de Edición a informes, paneles de control y calendarios</p> <p>Acceso de edición a filtros, vistas y agrupaciones</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de visualización de los objetos que contienen las entradas del diario que se muestran en el informe</p> <p>Obtendrá permisos de administración del informe después de crearlo</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Antes de realizar las acciones que se describen en este artículo, debe asegurarse de lo siguiente:

* Cualquier campo (incluidos los campos personalizados) sobre el que desee crear un informe se rastrea en Workfront. Solo puede informar sobre los datos del área de Actualizaciones de la que se realiza un seguimiento.

  Para obtener información sobre cómo añadir campos de los que desea que Workfront realice un seguimiento, consulte [Configurar actualizaciones del sistema](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

## Información general del informe Entrada de cuaderno

Como el informe Entrada de cuaderno consulta las actualizaciones del sistema, puede devolver un número significativo de resultados. Por este motivo, le recomendamos que filtre en objetos específicos, como proyectos, programas, portafolios, grupos, etc., al crear el informe.

Para obtener más información sobre los distintos tipos de objetos en Workfront, consulte [Comprender los objetos en Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

>[!NOTE]
>
>Como el informe Entrada de cuaderno devuelve muchos datos, no se admite la exportación ni el envío del informe programado.

La vista predeterminada para este informe contiene las siguientes columnas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Campo</th> 
   <th>Explicación</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>Nombre de campo</strong> </td> 
   <td> <p><span style="font-weight: normal;">El nombre del campo afectado. Según la configuración del informe, esta columna puede contener los campos Estado, ID de propietario, Nombre de tarea, Fecha planificada de finalización u otros.</span> </p> <p><span style="font-weight: normal;">Cuando </span> <strong>DE</strong>:<span style="font-weight: normal;"> se muestra en esta columna, indica que el campo que se muestra es un campo personalizado.</span></p> </td> 
  </tr> 
  <tr> 
   <td><strong>Tipo de cambio</strong> </td> 
   <td> <p>El tipo de cambio realizado en el campo afectado. Según las reglas de filtro que configure y las acciones realizadas por los usuarios, puede aparecer lo siguiente en este campo:</p> 
    <ul> 
     <li> <p>Agregar</p> </li> 
     <li> <p>Auditar</p> </li> 
     <li> <p>Eliminar</p> </li> 
     <li> <p>Resumen</p> </li> 
     <li> <p>Editar</p> </li> 
     <li> <p>Restaurar</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>Código de objeto principal</strong> </td> 
   <td> <p>El objeto principal más alto de la jerarquía.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Ámbito</strong> </td> 
   <td> <p>El tipo de objeto que se ha cambiado.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Fecha de entrada</strong> </td> 
   <td> <p>La fecha en que se cambió el campo.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Editado por Nombre</strong> </td> 
   <td> <p>El usuario que cambió el campo.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para organizar la información de este informe, puede utilizar la agrupación integrada denominada Proyecto. La agrupación Proyecto proporciona una agrupación principal de Nombre del proyecto y una agrupación secundaria de Fecha de entrada. Puede aplicar esta agrupación existente durante la creación del informe o puede aplicarla cuando visualice el informe.

Para obtener información sobre la configuración de las vistas, filtros y agrupaciones que desee para el informe, consulte la sección correspondiente:

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: from&nbsp;Luke: Take this for what it's worth, but part of me wonders if all of these subsections should be separate articles.</p>
<p>The biggest reason for breaking these up would be searchability, in my mind. For example, as a user, I might want to know how to see if the owner of a project changed. If I search the help site for that, I would be a lot more likely to find a separate article called "See if the owner of a project changed" vs an article titled "Create a Journal Entry report" because "Journal Entry" might mean nothing to me.) </p>
</div>
-->

* [Ver qué cambios de estado se han producido](#see-what-status-changes-occurred)
* [Ver cuándo se ha eliminado una tarea o un problema](#see-when-a-task-or-issue-was-deleted)
* [Ver cómo han cambiado los campos personalizados durante el ciclo de vida de un proyecto](#see-how-custom-fields-changed-over-the-course-of-a-project-s-life-cycle)
* [Ver cómo ha cambiado la fecha planificada de finalización durante el ciclo de vida de un proyecto](#see-how-the-planned-completion-date-changed-over-the-course-of-a-project-s-life-cycle)
* [Ver si ha cambiado el propietario de un proyecto](#see-if-the-owner-of-a-project-changed)

## Ver qué cambios de estado se han producido {#see-what-status-changes-occurred}

Puede configurar el informe Entrada de cuaderno para que muestre lo siguiente:

* Cuántos cambios de estado se han realizado en un proyecto, tarea o problema

* Cuál era el estado anterior antes del cambio
* Quién cambió el estado
* Cuándo tuvo lugar el cambio de estado

Si desea ver el estado de un proyecto, también puede configurar el informe para que muestre esta misma información usando el campo **Condición** del proyecto.

Esta información se puede utilizar para ayudar con las auditorías y para ilustrar la buena planificación por parte de usted y su organización.

1. Haga clic en el icono **[!UICONTROL Main Menu]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el icono **[!UICONTROL Main Menu]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **Informes**.
1. Haga clic en **Nuevo informe** y, a continuación, seleccione **Entrada de cuaderno**.

   ![Seleccionar entrada de diario](assets/nwe-select-journal-entry-350x273.png)

   Se carga Report Builder.

1. En la pestaña **Columnas (Vista)**, añada las siguientes columnas:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Columna</th> 
      <th>Explicación</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">Nombre de campo</p> </td> 
      <td> <p>El nombre del campo afectado. En este caso, <strong>estado</strong> debería mostrarse en esta columna.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Cambiar tipo</p> </td> 
      <td> <p>El tipo de cambio realizado en el campo afectado, como <strong>Añadir</strong>, <strong>Eliminar</strong> o <strong>Editar</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Editado por Nombre</p> </td> 
      <td> <p>El nombre del usuario que ha actualizado el estado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Fecha de entrada</p> </td> 
      <td> <p>La fecha en la que se cambió el estado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Valor de texto anterior</p> </td> 
      <td> <p>La clave del estado anterior. A continuación, se indican las claves de estado de los estados del proyecto predeterminados:</p> 
       <ul> 
        <li> <p> <strong>CUR</strong>: actual</p> </li> 
        <li> <p><strong>DED</strong>: inactivo</p> </li> 
        <li> <p><strong>ONH</strong>: en espera</p> </li> 
        <li> <p><strong>PLN</strong>: planificando</p> </li> 
        <li> <p><strong>CPL</strong>: completado</p> </li> 
        <li> <p><strong>REQ</strong>: solicitado</p> </li> 
        <li> <p><strong>APR</strong>: aprobado</p> </li> 
        <li> <p><strong>REJ</strong>: rechazado</p> </li> 
        <li> <p><strong>IDA</strong>: idea</p> </li> 
       </ul> <p>Si su organización ha configurado estados personalizados, es posible que en esta columna aparezcan otras claves de estado. Para saber qué estado personalizado está relacionado con una clave de estado, póngase en contacto con el administrador de Workfront o de grupos.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nuevo valor de texto</p> </td> 
      <td> <p>La clave para el estado actualizado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Código de objeto superior</p> </td> 
      <td> <p>El objeto principal más alto para el campo que tuvo el cambio de estado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Ámbito</p> </td> 
      <td> <p>El tipo de objeto que tuvo el cambio de estado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nombre de problema<br> (opcional)</p> </td> 
      <td> <p>El nombre del problema que ha sufrido un cambio de estado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nombre de tarea<br> (opcional)</p> </td> 
      <td> <p>El nombre de la tarea cuyo estado ha cambiado.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Para obtener más información sobre cómo añadir columnas, consulte [Información general sobre las vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. En la ficha **Filtros**, haga clic en **Agregar una regla de filtro** y, a continuación, agregue la regla de filtro **Nombre de campo** > **Igual** > **estado**.

   ![Filtro de estado de entrada de diario](assets/nwe-journal-entry-status-filter-rules-350x90.png)

   >[!TIP]
   >
   >Para informar sobre los cambios de condición, puede añadir la regla de filtro **Nombre de campo** > **igual** > **Condición**.

   Para obtener más información sobre cómo añadir filtros, consulte [Información general de los filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Opcional) Para reducir el enfoque del informe y los tiempos de carga, añada una indicación.

   O

   Cree reglas de filtro adicionales para incluir proyectos, tareas o problemas específicos.

   >[!IMPORTANT]
   >
   >Crear una regla de filtro que use el modificador **Contiene** puede aumentar los tiempos de carga. Por este motivo, recomendamos usar un modificador diferente como **igual** cuando sea posible para filtrar por un proyecto específico o un ID de objeto de nivel superior.

   Para obtener información sobre cómo añadir una indicación, consulte [Añadir una indicación a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. En la pestaña **Agrupaciones**, haga clic en el menú **Aplicar una agrupación existente** y seleccione **Proyecto**.

   Para obtener más información sobre cómo añadir agrupaciones, consulte [Información general de agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Haga clic en **Guardar + Cerrar**.

   Se carga el nuevo informe.

## Ver cuándo se ha eliminado una tarea o un problema {#see-when-a-task-or-issue-was-deleted}

Puede configurar el informe Entrada de cuaderno para que muestre lo siguiente:

* Las tareas o problemas que se han eliminado
* Quién ha eliminado una tarea o un problema

Para ver cuándo se ha eliminado una tarea o un problema:

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **Informes**.
1. Haga clic en **Nuevo informe** y, a continuación, seleccione **Entrada de cuaderno**.

   ![Seleccionar entrada de diario](assets/nwe-select-journal-entry-350x273.png)

   Se carga Report Builder.

1. En la pestaña **Columnas (Vista)**, añada las siguientes columnas:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Columna</th> 
      <th>Explicación</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">Ámbito</p> </td> 
      <td> <p>El tipo de objeto que se ha eliminado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Cambiar tipo</p> </td> 
      <td> <p>El tipo de cambio que se ha realizado. El cambio <strong>Eliminar</strong> se muestra en esta columna.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Fecha de entrada</p> </td> 
      <td> <p>La fecha en la que se eliminó la tarea o el problema.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Editado por Nombre</p> </td> 
      <td> <p>El nombre del usuario que eliminó la tarea o el problema.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nombre del proyecto</p> </td> 
      <td> <p>El nombre del proyecto del que se eliminaron tareas o problemas.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Para obtener más información sobre la adición de columnas, consulte [Información general sobre las vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. En la pestaña **Filtros**, haga clic en **Añadir regla de filtro** y, a continuación, añada los siguientes filtros:

   * **Tipo de cambio** > **Igual** > **Eliminar**
   * **Id. de proyecto** > **Igual** > **&lt; nombre de proyecto >**

     <!--WRITER check link; this png file has spaces
     [![Task or issue deleted](assets/classic-task-or-issue-deleted-350x90.png)](../../../Resources/Images/Reports/Creating and Managing Reports/QS_Task or issue deleted.png)-->

   Para obtener más información sobre cómo añadir filtros, consulte [Información general de los filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Opcional) Para reducir el enfoque del informe y los tiempos de carga, añada una indicación.

   O

   Cree reglas de filtro adicionales para incluir proyectos, tareas o problemas específicos.

   >[!IMPORTANT]
   >
   >Crear una regla de filtro que use el modificador **Contiene** puede aumentar los tiempos de carga. Por este motivo, recomendamos usar un modificador diferente como **igual** cuando sea posible para filtrar por un proyecto específico o un ID de objeto de nivel superior.

   Para obtener información sobre cómo añadir una indicación, consulte [Añadir una indicación a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. (Opcional) En la pestaña **Agrupaciones**, haga clic en **Aplicar una agrupación existente** y seleccione **Proyecto**.

   Para obtener más información sobre cómo añadir agrupaciones, consulte [Información general de agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Haga clic en **Guardar + Cerrar**.

   Se carga el nuevo informe.

## Ver cómo han cambiado los campos personalizados durante el ciclo de vida de un proyecto {#see-how-custom-fields-changed-over-the-course-of-a-project-s-life-cycle}

Puede realizar el seguimiento de los cambios importantes en los campos a lo largo del proyecto. Para ello, puede configurar la Entrada de cuaderno para que realice un seguimiento:

* Si se han añadido, actualizado o editado determinados campos personalizados
* Cuándo tuvieron lugar estos cambios
* Quién realizó los cambios

Para ver cómo han cambiado los campos personalizados durante el ciclo de vida de un proyecto:

1. Haga clic en el icono **[!UICONTROL Main Menu]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el icono **[!UICONTROL Main Menu]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **Informes**.
1. Haga clic en **Nuevo informe** y, a continuación, seleccione **Entrada de cuaderno**.

   ![Seleccionar entrada de diario](assets/nwe-select-journal-entry-350x273.png)

   Se carga Report Builder.

1. En la ficha **Columnas (vista)**, asegúrese de que tiene o haga clic en **Agregar columna** para agregar las siguientes columnas:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Columna</th> 
      <th>Explicación</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">Nombre de campo</p> </td> 
      <td> <p>El nombre del campo personalizado afectado.</p> <p><span style="font-weight: normal;">Cuando </span> <strong>DE</strong>:<span style="font-weight: normal;"> se muestra en esta columna, indica que el campo que se muestra es un campo personalizado.</span></p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Cambiar tipo</p> </td> 
      <td> <p>El tipo de cambio realizado en el campo afectado, como <strong>Añadir</strong>, <strong>Eliminar</strong> o <strong>Editar</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Editado por Nombre</p> </td> 
      <td> <p>El nombre del usuario que ha actualizado el campo personalizado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Fecha de entrada</p> </td> 
      <td> <p>La fecha en la que se cambió el valor del campo personalizado.</p> <p>Debe ordenar por este campo en orden descendente.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Valor de número anterior</p> </td> 
      <td> <p>El valor numérico anterior del campo personalizado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nuevo valor de número</p> </td> 
      <td> <p>El valor de número actual del campo personalizado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Valor de fecha anterior</p> </td> 
      <td> <p>El valor de fecha anterior del campo personalizado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nuevo valor de fecha</p> </td> 
      <td> <p>El valor de fecha actual del campo personalizado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Valor de texto anterior</p> </td> 
      <td> <p>El valor de texto anterior del campo personalizado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nuevo valor de texto</p> </td> 
      <td> <p>El valor de texto actual del campo personalizado.</p> <p>Si el campo personalizado es un campo typeahead, la columna <strong>Nuevo valor de texto</strong> muestra el identificador de objeto.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Para obtener más información sobre cómo añadir columnas, consulte [Información general sobre las vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. En la ficha **Filtros**, haga clic en **Agregar una regla de filtro** y, a continuación, agregue los siguientes filtros:

   * **Nombre del campo de entrada de diario** > **Contains** > **DE**

     >[!TIP]
     >
     >Para limitar este informe a campos personalizados específicos, agregue la regla de filtro **Nombre del campo de entrada de diario** > **Igual** > **&lt; Nombre de campo personalizado>**.

   * **Id. de proyecto** > **Igual** > **&lt; proyecto >**.

   ![El formulario personalizado cambia el filtro](assets/qs-custom-form-changes-filter-350x92.png)

   Para obtener más información sobre cómo añadir filtros, consulte [Información general de los filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Opcional) Para reducir el enfoque del informe y los tiempos de carga, añada una indicación.

   O

   Cree reglas de filtro adicionales para incluir proyectos, tareas o problemas específicos.

   >[!IMPORTANT]
   >
   >Crear una regla de filtro que use el modificador **Contiene** puede aumentar los tiempos de carga. Por este motivo, recomendamos usar un modificador diferente como **igual** cuando sea posible para filtrar por un proyecto específico o un ID de objeto de nivel superior.

   Para obtener información sobre cómo añadir una indicación, consulte [Añadir una indicación a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. En la pestaña **Agrupaciones**, haga clic en el menú **Aplicar una agrupación existente** y seleccione **Proyecto**.

   Para obtener más información sobre cómo añadir agrupaciones, consulte [Información general de agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Haga clic en **Guardar + Cerrar**.

   Se carga el nuevo informe.

## Descubra cómo ha cambiado la fecha planificada de finalización a lo largo del ciclo de vida de un proyecto {#see-how-the-planned-completion-date-changed-over-the-course-of-a-project-s-life-cycle}

Puede configurar el informe Entrada de cuaderno para mostrar la frecuencia con la que cambia la fecha planificada de finalización en el transcurso de la vida de un proyecto.

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **Informes**.
1. Haga clic en **Nuevo informe** y, a continuación, seleccione **Entrada de cuaderno**.

   ![Seleccionar entrada de diario](assets/nwe-select-journal-entry-350x273.png)

   Se carga Report Builder.

1. En la pestaña **Columnas (Vista)**, añada las siguientes columnas:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Columna</th> 
      <th>Explicación</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">Nombre de campo</p> </td> 
      <td> <p>El nombre del campo afectado.</p> <p><span style="font-weight: normal;">Cuando </span> <strong>DE</strong>:<span style="font-weight: normal;"> se muestra en esta columna, indica que el campo que se muestra es un campo personalizado.</span></p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Cambiar tipo</p> </td> 
      <td>El tipo de cambio que se ha producido, como <strong>Añadir</strong>, <strong>Eliminar</strong> o <strong>Editar</strong>.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Editado por Nombre</p> </td> 
      <td> <p>El nombre del usuario que ha actualizado la fecha planificada de finalización del proyecto.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Fecha de entrada</p> </td> 
      <td> <p>La fecha en la que se modificó la fecha planificada de finalización del proyecto.</p> <p>Debe ordenar por este campo en orden descendente.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Código de objeto superior</p> </td> 
      <td> <p>El objeto principal más alto para el campo que tuvo el cambio de Fecha planificada de finalización.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Ámbito</p> </td> 
      <td> <p>El objeto que tuvo el cambio de Fecha planificada de finalización.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Valor de fecha anterior</p> </td> 
      <td> <p>El valor anterior de la fecha planificada de finalización.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nuevo valor de fecha</p> </td> 
      <td> <p>El valor actual para la fecha planificada de finalización.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nombre del proyecto</p> <p>(Opcional)</p> </td> 
      <td> <p>El nombre del proyecto cuya fecha planificada de finalización se ha cambiado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nombre de la tarea</p> <p>(Opcional)</p> </td> 
      <td> <p>El nombre de las tareas del proyecto cuya fecha planificada de finalización se ha cambiado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nombre del problema</p> <p>(Opcional)</p> </td> 
      <td>El nombre de los problemas del proyecto cuya fecha planificada de finalización se ha cambiado.</td> 
     </tr> 
    </tbody> 
   </table>

   Para obtener más información sobre la adición de columnas, consulte [Información general sobre las vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. En la ficha **Filtros**, haga clic en **Agregar una regla de filtro** y, a continuación, agregue lo siguiente:

   * **Nombre de campo** > **Igual** > **Fecha**
   * **Id. de proyecto** > **Igual** > **&lt; nombre de proyecto >**.

   ![Filtro de cambio de fecha planificada de finalización](assets/qs-planned-completion-date-change-filter-350x91.png)

   Para obtener más información sobre cómo añadir filtros, consulte [Información general de los filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Opcional) Para reducir el enfoque del informe y los tiempos de carga, añada una indicación.

   O

   Cree reglas de filtro adicionales para incluir proyectos, tareas o problemas específicos.

   >[!IMPORTANT]
   >
   >Crear una regla de filtro que use el modificador **Contiene** puede aumentar los tiempos de carga. Por este motivo, recomendamos usar un modificador diferente como **igual** cuando sea posible para filtrar por un proyecto específico o un ID de objeto de nivel superior.

   Para obtener información sobre cómo añadir una indicación, consulte [Añadir una indicación a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. En la pestaña **Agrupaciones**, haga clic en el menú **Aplicar una agrupación existente** y seleccione **Proyecto**.

   Para obtener más información sobre cómo añadir agrupaciones, consulte [Información general de agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Haga clic en **Guardar + Cerrar**.

   Se carga el nuevo informe.

## Ver si ha cambiado el propietario de un proyecto {#see-if-the-owner-of-a-project-changed}

Puede configurar el informe Entrada de cuaderno para que muestre cuántas veces cambia el propietario del proyecto (o el administrador del proyecto) a lo largo de la vida de un proyecto.

1. Haga clic en el icono **[!UICONTROL Main Menu]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el icono **[!UICONTROL Main Menu]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **Informes**.
1. Haga clic en **Nuevo informe** y, a continuación, seleccione **Entrada de cuaderno**.

   ![Seleccionar entrada de diario](assets/nwe-select-journal-entry-350x273.png)

   Se carga Report Builder.

1. En la pestaña **Columnas (Vista)**, añada las siguientes columnas:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Columna</th> 
      <th>Explicación</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">Nombre de campo</p> </td> 
      <td>El nombre del campo afectado. <strong>ownerID</strong> se muestra en esta columna.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Cambiar tipo</p> </td> 
      <td> <p>El tipo de cambio que se ha realizado, como <strong>Añadir</strong>, <strong>Eliminar</strong> o <strong>Editar</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Código de objeto superior</p> </td> 
      <td> <p>El objeto principal más alto del proyecto al que se ha actualizado el propietario del proyecto.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Fecha de entrada</p> </td> 
      <td>La fecha en la que se cambió al propietario del proyecto.<br>Debe ordenar por este campo en orden descendente.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Editado por Nombre</p> </td> 
      <td> <p>El nombre del usuario que actualizó al propietario del proyecto.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Información adicional 1</p> </td> 
      <td> <p>El propietario del proyecto actual del proyecto.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Información adicional 2</p> </td> 
      <td> <p>El propietario del proyecto anterior del proyecto.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nombre del proyecto</p> </td> 
      <td> <p>El proyecto al que se le ha actualizado el campo Propietario del proyecto.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Para obtener más información sobre la adición de columnas, consulte [Información general sobre las vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. En la pestaña **Filtros**, haga clic en **Añadir regla de filtro** y, a continuación, añada lo siguiente:

   * **Nombre de campo** > **Igual** > **ownerID**
   * **Id. de proyecto** > **Igual** > **&lt; nombre de proyecto >**.

   ![Filtro de cambio de propietario](assets/qs-owner-changes-filter-350x94.png)

   Para obtener más información sobre cómo añadir filtros, consulte [Información general de los filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Opcional) Para reducir el enfoque del informe y los tiempos de carga, añada una indicación.

   O

   Cree reglas de filtro adicionales para incluir proyectos, tareas o problemas específicos.

   >[!IMPORTANT]
   >
   >Crear una regla de filtro que use el modificador **Contiene** puede aumentar los tiempos de carga. Por este motivo, recomendamos usar un modificador diferente como **igual** cuando sea posible para filtrar por un proyecto específico o un ID de objeto de nivel superior.

   Para obtener información sobre cómo añadir una indicación, consulte [Añadir una indicación a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. (Opcional) En la pestaña **Agrupaciones**, haga clic en **Aplicar una agrupación existente** y seleccione **Proyecto**.

   Para obtener más información sobre cómo añadir agrupaciones, consulte [Información general de agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Haga clic en **Guardar + Cerrar**.

   Se muestra el informe de nueva entrada de diario.
