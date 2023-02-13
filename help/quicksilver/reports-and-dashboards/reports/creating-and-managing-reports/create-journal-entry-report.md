---
title: Informe del área Actualizaciones
description: Informe del área Actualizaciones
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: ecf947ce-54d8-4103-8903-f455b1d86c39
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '2698'
ht-degree: 4%

---

# Informe del área Actualizaciones

El informe Entrada de diario muestra las actualizaciones del sistema desde el área Actualizaciones de proyectos, tareas, problemas y otros objetos que anteriormente solo estaban disponibles a través de la API de Adobe Workfront. Aunque este es un informe avanzado pensado para casos de uso específicos, el formato más digerible le facilita la realización de informes sobre la actividad del proyecto y las actualizaciones del sistema en Workfront.

>[!TIP]
>
>El informe Entrada de diario solo contiene actualizaciones del sistema desde el área Actualizaciones de objetos. Para informar sobre los comentarios que quedan en el área Actualizaciones , debe utilizar el informe Nota .\
>Para obtener más información sobre el informe Nota , consulte [Ver todas las actualizaciones en un informe de Nota](../../../workfront-basics/updating-work-items-and-viewing-updates/view-all-updates-in-a-report.md)‍

El informe Entrada de diario puede mostrar:

* Cuántos cambios de estado se han producido
* Cuando se elimina una tarea o un problema
* Cambio de los valores de campos personalizados importantes durante el ciclo de vida de un proyecto
* Qué fechas importantes han cambiado durante el ciclo de vida de un proyecto
* Si el propietario de un proyecto ha cambiado

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Editar acceso a filtros, vistas y grupos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos para los objetos que contienen las entradas del diario que se muestran en el informe</p> <p>Después de crearlo, obtendrá permisos de administración para el informe</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Antes de realizar las acciones descritas en este artículo, debe asegurarse de lo siguiente:

* Los campos sobre los que desee crear un informe se rastrean en Workfront. Solo puede generar informes de los datos del área Actualizaciones de la que se realiza el seguimiento.

   Para obtener información sobre cómo añadir campos que desea que Workfront rastree, consulte [Configurar actualizaciones del sistema](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

* Los campos personalizados de los que desee informar tendrán la configuración **Mostrar los cambios de campo en las fuentes de actualización** activada.

   Para obtener información sobre cómo habilitar esta configuración para un campo personalizado, consulte la sección [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create) en el artículo [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Resumen del informe Entrada en diario

Dado que el informe Entrada de diario consulta las actualizaciones del sistema, puede arrojar un número significativo de resultados. Por este motivo, le recomendamos que filtre a objetos específicos (como proyectos, programas, portafolios, grupos, etc.) al crear el informe.

Para obtener más información sobre los distintos tipos de objetos en Workfront, consulte [Explicación de los objetos en Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

>[!NOTE]
>
>Como el informe Entrada de diario devuelve tantos datos, no se admiten la exportación ni el envío de informes programados.

La vista predeterminada para este informe contiene las columnas siguientes:

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
   <td> <p><span style="font-weight: normal;">Nombre del campo afectado. Según la configuración del informe, esta columna puede contener los campos Estado, ID de propietario, Nombre de tarea, Fecha de finalización planeada u otros.</span> </p> <p><span style="font-weight: normal;">When</span> <strong>DE</strong>:<span style="font-weight: normal;"> en esta columna, indica que el campo enumerado es un campo personalizado.</span></p> </td> 
  </tr> 
  <tr> 
   <td><strong>Cambiar tipo</strong> </td> 
   <td> <p>Tipo de cambio realizado en el campo afectado. Según las reglas de filtro que configure y las acciones que realicen los usuarios, en este campo podría aparecer lo siguiente:</p> 
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
   <td><strong>Código de objeto superior</strong> </td> 
   <td> <p>El objeto principal más alto de la jerarquía.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Ámbito</strong> </td> 
   <td> <p>Tipo de objeto que se cambió.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Fecha de entrada</strong> </td> 
   <td> <p>La fecha en la que se cambió el campo.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Editado por nombre</strong> </td> 
   <td> <p>El usuario que ha cambiado el campo.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para organizar la información de este informe, puede utilizar la agrupación integrada Project. La agrupación Project le proporciona una agrupación principal de Nombre del proyecto y una agrupación secundaria de Fecha de entrada. Puede aplicar esta agrupación existente durante la creación del informe o aplicarla al ver el informe.

Para obtener información sobre cómo configurar las vistas, filtros y agrupaciones que desee para el informe, consulte la sección relevante:

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: from&nbsp;Luke: Take this for what it's worth, but part of me wonders if all of these subsections should be separate articles.</p>
<p>The biggest reason for breaking these up would be searchability, in my mind. For example, as a user, I might want to know how to see if the owner of a project changed. If I search the help site for that, I would be a lot more likely to find a separate article called "See if the owner of a project changed" vs an article titled "Create a Journal Entry report" because "Journal Entry" might mean nothing to me.) </p>
</div>
-->

* [Ver qué cambios de estado se han producido](#see-what-status-changes-occurred)
* [Ver cuándo se eliminó una tarea o un problema](#see-when-a-task-or-issue-was-deleted)
* [Ver cómo cambiaron los campos personalizados durante el ciclo de vida de un proyecto](#see-how-custom-fields-changed-over-the-course-of-a-project-s-life-cycle)
* [Ver cómo cambió la fecha de finalización planeada a lo largo del ciclo de vida de un proyecto](#see-how-the-planned-completion-date-changed-over-the-course-of-a-project-s-life-cycle)
* [Ver si el propietario de un proyecto ha cambiado](#see-if-the-owner-of-a-project-changed)

## Ver qué cambios de estado se han producido {#see-what-status-changes-occurred}

Puede configurar el informe Entrada de diario para que muestre:

* ¿Cuántos cambios de estado se han realizado en un proyecto, tarea o problema?

* Qué era el estado anterior antes del cambio
* Quién cambió el estado
* Cuando se produjo el cambio de estado

Si desea ver el estado de un proyecto, también puede configurar el informe para que muestre la misma información mediante el proyecto **Condición** campo .

Esta información se puede utilizar para ayudar con la auditoría e ilustrar cómo planifican usted y su organización.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;for tip below: When analytics adds the status option, update this note to say "these entries (status or condition changes)")</p>
-->

>[!TIP]
>
>Si desea comparar la diferencia de días entre los cambios de condición, puede utilizar el análisis mejorado.\
>Para obtener más información sobre el análisis mejorado, consulte [Resumen de análisis mejorado](../../../enhanced-analytics/enhanced-analytics-overview.md).

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Informes**.
1. Haga clic en **Nuevo informe** y, a continuación, seleccione **Entrada de diario**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   Se carga el Creador de informes.

1. En el **Columnas (Vista)** , agregue las columnas siguientes:

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
      <td> <p>Nombre del campo afectado. En este caso, <strong>status</strong> debe aparecer en esta columna.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Cambiar tipo</p> </td> 
      <td> <p>Tipo de cambio realizado en el campo afectado, como <strong>Agregar</strong>, <strong>Eliminar</strong>o <strong>Editar</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Editado por nombre</p> </td> 
      <td> <p>Nombre del usuario que ha actualizado el estado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Fecha de entrada</p> </td> 
      <td> <p>La fecha en la que se cambió el estado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Valor de texto anterior</p> </td> 
      <td> <p>La clave del estado anterior. Las siguientes son las claves de estado para los estados predeterminados del proyecto:</p> 
       <ul> 
        <li> <p> <strong>CUR</strong>: Actual</p> </li> 
        <li> <p><strong>DED</strong>: Muerto</p> </li> 
        <li> <p><strong>ONH</strong>: En espera</p> </li> 
        <li> <p><strong>PLN</strong>: Planificación</p> </li> 
        <li> <p><strong>CPL</strong>: Completar</p> </li> 
        <li> <p><strong>REQ</strong>: Solicitado</p> </li> 
        <li> <p><strong>APR</strong>: Aprobado</p> </li> 
        <li> <p><strong>REJ</strong>: Rechazado</p> </li> 
        <li> <p><strong>IDA</strong>: Idea</p> </li> 
       </ul> <p>Si su organización ha configurado estados personalizados, es posible que en esta columna aparezcan otras claves de estado. Para obtener información sobre el estado personalizado relacionado con una clave de estado, póngase en contacto con el administrador de Workfront o el administrador del grupo.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nuevo valor de texto</p> </td> 
      <td> <p>La clave para el estado actualizado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Código de objeto superior</p> </td> 
      <td> <p>El objeto principal más alto del campo que ha sufrido el cambio de estado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Ámbito</p> </td> 
      <td> <p>Tipo de objeto que ha cambiado el estado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nombre del problema<br>(Opcional)</p> </td> 
      <td> <p>Nombre del problema que ha cambiado de estado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nombre de la tarea<br>(Opcional)</p> </td> 
      <td> <p>Nombre de la tarea que ha tenido un cambio de estado.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Para obtener más información sobre cómo agregar columnas, consulte [Información general sobre las vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. En el **Filtros** , haga clic en **Agregar regla de filtro**, luego agregue la regla de filtro **Nombre del campo** > **Igual** > **status**.

   ![](assets/nwe-journal-entry-status-filter-rules-350x90.png)

   >[!TIP]
   >
   >Para informar sobre los cambios de condición, puede añadir la regla de filtro **Nombre del campo** > **Igual** > **Condición**.

   Para obtener más información sobre cómo agregar filtros, consulte [Información general sobre filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Opcional) Para reducir el foco del informe y los tiempos de carga, agregue una solicitud.

   O

   Cree reglas de filtro adicionales para incluir proyectos, tareas o problemas específicos.

   >[!IMPORTANT]
   >
   >Creación de una regla de filtro que utilice el modificador **Contiene** puede aumentar los tiempos de carga. Por este motivo, se recomienda utilizar un modificador diferente como **Igual** cuando sea posible, filtrar por un proyecto específico o ID de objeto de nivel superior.

   Para obtener información sobre cómo añadir un mensaje, consulte [Agregar solicitudes a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. En el **Agrupaciones** , haga clic en **Aplicar una agrupación existente** y, a continuación, seleccione **Proyecto**.

   Para obtener más información sobre cómo añadir agrupaciones, consulte [Información general sobre las agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Haga clic en **Guardar + Cerrar**.

   Se carga el nuevo informe.

## Ver cuándo se eliminó una tarea o un problema {#see-when-a-task-or-issue-was-deleted}

Puede configurar el informe Entrada de diario para que muestre:

* Qué tareas o problemas se han eliminado
* Quién eliminó una tarea o un problema

Para ver cuándo se eliminó una tarea o un problema:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Informes**.
1. Haga clic en **Nuevo informe** y, a continuación, seleccione **Entrada de diario**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   Se carga el Creador de informes.

1. En el **Columnas (Vista)** , agregue las columnas siguientes:

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
      <td> <p>Tipo de objeto que se eliminó.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Cambiar tipo</p> </td> 
      <td> <p>Tipo de cambio que se produjo. La variable <strong>Eliminar</strong> el cambio aparece en esta columna.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Fecha de entrada</p> </td> 
      <td> <p>La fecha en la que se eliminó la tarea o el problema.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Editado por nombre</p> </td> 
      <td> <p>Nombre del usuario que ha eliminado la tarea o el problema.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nombre del proyecto</p> </td> 
      <td> <p>Nombre del proyecto que tiene tareas o problemas eliminados.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Para obtener más información sobre cómo agregar columnas, consulte [Información general sobre las vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. En el **Filtros** , haga clic en **Agregar regla de filtro** y, a continuación, agregue lo siguiente:

   * **Tipo de cambio** > **Igual** > **Eliminar**
   * **ID del proyecto** > **Igual** > **`<project>`**

      <!--WRITER check link; this png file has spaces
     [![](assets/classic-task-or-issue-deleted-350x90.png)](../../../Resources/Images/Reports/Creating and Managing Reports/QS_Task or issue deleted.png)-->
   Para obtener más información sobre cómo agregar filtros, consulte [Información general sobre filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Opcional) Para reducir el foco del informe y los tiempos de carga, agregue una solicitud.

   O

   Cree reglas de filtro adicionales para incluir proyectos, tareas o problemas específicos.

   >[!IMPORTANT]
   >
   >Creación de una regla de filtro que utilice el modificador **Contiene** puede aumentar los tiempos de carga. Por este motivo, se recomienda utilizar un modificador diferente como **Igual** cuando sea posible, filtrar por un proyecto específico o ID de objeto de nivel superior.

   Para obtener información sobre cómo añadir un mensaje, consulte [Agregar solicitudes a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. (Opcional) En la **Agrupaciones** , haga clic en **Aplicar una agrupación existente** y, a continuación, seleccione **Proyecto**.

   Para obtener más información sobre cómo añadir agrupaciones, consulte [Información general sobre las agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Haga clic en **Guardar + Cerrar**.

   Se carga el nuevo informe.

## Ver cómo cambiaron los campos personalizados durante el ciclo de vida de un proyecto {#see-how-custom-fields-changed-over-the-course-of-a-project-s-life-cycle}

Puede realizar un seguimiento de los cambios importantes en los campos durante el curso del proyecto. Para ello, puede configurar la entrada de diario para realizar el seguimiento:

* Si se agregaron, actualizaron o editaron determinados campos personalizados
* Cuando se produjeron estos cambios
* Quién realizó los cambios

Para ver cómo han cambiado los campos personalizados durante el ciclo de vida de un proyecto:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Informes**.
1. Haga clic en **Nuevo informe** y, a continuación, seleccione **Entrada de diario**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   Se carga el Creador de informes.

1. En el **Columnas (Vista)** , agregue las columnas siguientes:

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
      <td> <p>Nombre del campo personalizado afectado.</p> <p><span style="font-weight: normal;">When</span> <strong>DE</strong>:<span style="font-weight: normal;"> en esta columna, indica que el campo enumerado es un campo personalizado.</span></p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Cambiar tipo</p> </td> 
      <td> <p>Tipo de cambio realizado en el campo afectado, como <strong>Agregar</strong>, <strong>Eliminar</strong>o <strong>Editar</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Editado por nombre</p> </td> 
      <td> <p>Nombre del usuario que ha actualizado el campo personalizado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Fecha de entrada</p> </td> 
      <td> <p>La fecha en la que cambió el valor en el campo personalizado.</p> <p>Debe ordenar por este campo en orden descendente.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Valor de número anterior</p> </td> 
      <td> <p>El valor de número anterior en el campo personalizado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nuevo valor de número</p> </td> 
      <td> <p>El valor del número actual en el campo personalizado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Valor de fecha anterior</p> </td> 
      <td> <p>El valor de fecha anterior en el campo personalizado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nuevo valor de fecha</p> </td> 
      <td> <p>El valor de fecha actual en el campo personalizado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Valor de texto anterior</p> </td> 
      <td> <p>Valor del texto anterior en el campo personalizado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nuevo valor de texto</p> </td> 
      <td> <p>El valor de texto actual en el campo personalizado.</p> <p>Si el campo personalizado es un campo de tipo adelante, la variable <strong>Nuevo valor de texto</strong> muestra el ID del objeto.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Para obtener más información sobre cómo agregar columnas, consulte [Información general sobre las vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. En el **Filtros** , haga clic en **Agregar regla de filtro** y, a continuación, agregue lo siguiente:

   * **Nombre de campo de entrada de diario** > **Contiene** > **DE**

      >[!TIP]
      >
      >Para limitar este informe a campos personalizados específicos, agregue la regla de filtro **Nombre de campo de entrada de diario** > **Igual** > **`<custom field>`**.

   * **ID del proyecto** > **Igual** > **`<project>`**

      ![](assets/qs-custom-form-changes-filter-350x92.png)
   Para obtener más información sobre cómo agregar filtros, consulte [Información general sobre filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Opcional) Para reducir el foco del informe y los tiempos de carga, agregue una solicitud.

   O

   Cree reglas de filtro adicionales para incluir proyectos, tareas o problemas específicos.

   >[!IMPORTANT]
   >
   >Creación de una regla de filtro que utilice el modificador **Contiene** puede aumentar los tiempos de carga. Por este motivo, se recomienda utilizar un modificador diferente como **Igual** cuando sea posible, filtrar por un proyecto específico o ID de objeto de nivel superior.

   Para obtener información sobre cómo añadir un mensaje, consulte [Agregar solicitudes a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. En el **Agrupaciones** , haga clic en **Aplicar una agrupación existente** y, a continuación, seleccione **Proyecto**.

   Para obtener más información sobre cómo añadir agrupaciones, consulte [Información general sobre las agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Haga clic en **Guardar + Cerrar**.

   Se carga el nuevo informe.

## Ver cómo cambió la fecha de finalización planeada a lo largo del ciclo de vida de un proyecto {#see-how-the-planned-completion-date-changed-over-the-course-of-a-project-s-life-cycle}

Puede configurar el informe Entrada de diario para mostrar con qué frecuencia cambia la Fecha de finalización planeada a lo largo de la vida de un proyecto.

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Informes**.
1. Haga clic en **Nuevo informe** y, a continuación, seleccione **Entrada de diario**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   Se carga el Creador de informes.

1. En el **Columnas (Vista)** , agregue las columnas siguientes:

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
      <td> <p>Nombre del campo afectado.</p> <p><span style="font-weight: normal;">When</span> <strong>DE</strong>:<span style="font-weight: normal;"> en esta columna, indica que el campo enumerado es un campo personalizado.</span></p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Cambiar tipo</p> </td> 
      <td>El tipo de cambio que se produjo, como <strong>Agregar</strong>, <strong>Eliminar</strong>o <strong>Editar</strong>.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Editado por nombre</p> </td> 
      <td> <p>Nombre del usuario que ha actualizado la fecha de finalización planeada del proyecto.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Fecha de entrada</p> </td> 
      <td> <p>La fecha en la que se cambió la fecha de finalización prevista del proyecto.</p> <p>Debe ordenar por este campo en orden descendente.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Código de objeto superior</p> </td> 
      <td> <p>El objeto principal más alto del campo que ha tenido el cambio Fecha de finalización planeada.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Ámbito</p> </td> 
      <td> <p>El objeto que tuvo el cambio de fecha de finalización planeada.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Valor de fecha anterior</p> </td> 
      <td> <p>Valor anterior de la fecha de finalización planeada.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nuevo valor de fecha</p> </td> 
      <td> <p>El valor actual de la fecha de finalización planeada.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nombre del proyecto</p> <p>(Opcional)</p> </td> 
      <td> <p>El nombre del proyecto que tuvo el cambio en la fecha de finalización planeada.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nombre de la tarea</p> <p>(Opcional)</p> </td> 
      <td> <p>Nombre de las tareas del proyecto que tuvieron el cambio en la fecha de finalización planeada.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nombre de problema</p> <p>(Opcional)</p> </td> 
      <td>Nombre de los problemas del proyecto que tienen el cambio Fecha de finalización planeada.</td> 
     </tr> 
    </tbody> 
   </table>

   Para obtener más información sobre cómo agregar columnas, consulte [Información general sobre las vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. En el **Filtros** , haga clic en **Agregar regla de filtro** y, a continuación, agregue lo siguiente:

   * **Nombre del campo** > **Igual** > **Fecha**
   * **ID del proyecto** > **Igual** > **`<project>`**

   ![](assets/qs-planned-completion-date-change-filter-350x91.png)

   Para obtener más información sobre cómo agregar filtros, consulte [Información general sobre filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Opcional) Para reducir el foco del informe y los tiempos de carga, agregue una solicitud.

   O

   Cree reglas de filtro adicionales para incluir proyectos, tareas o problemas específicos.

   >[!IMPORTANT]
   >
   >Creación de una regla de filtro que utilice el modificador **Contiene** puede aumentar los tiempos de carga. Por este motivo, se recomienda utilizar un modificador diferente como **Igual** cuando sea posible, filtrar por un proyecto específico o ID de objeto de nivel superior.

   Para obtener información sobre cómo añadir un mensaje, consulte [Agregar solicitudes a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. En el **Agrupaciones** , haga clic en **Aplicar una agrupación existente** y, a continuación, seleccione **Proyecto**.

   Para obtener más información sobre cómo añadir agrupaciones, consulte [Información general sobre las agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Haga clic en **Guardar + Cerrar**.

   Se carga el nuevo informe.

## Ver si el propietario de un proyecto ha cambiado {#see-if-the-owner-of-a-project-changed}

Puede configurar el informe Entrada de diario para mostrar cuántas veces el propietario del proyecto (o el administrador del proyecto) cambia a lo largo de la vida del proyecto.

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Informes**.
1. Haga clic en **Nuevo informe** y, a continuación, seleccione **Entrada de diario**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   Se carga el Creador de informes.

1. En el **Columnas (Vista)** , agregue las columnas siguientes:

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
      <td>Nombre del campo afectado. La variable <strong>ownerID</strong> se muestra en esta columna.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Cambiar tipo</p> </td> 
      <td> <p>El tipo de cambio que se produjo, como <strong>Agregar</strong>, <strong>Eliminar</strong>o <strong>Editar</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Código de objeto superior</p> </td> 
      <td> <p>El objeto principal más alto del proyecto que tenía actualizado el propietario del proyecto.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Fecha de entrada</p> </td> 
      <td>La fecha en la que se cambió el propietario del proyecto.<br>Debe ordenar por este campo en orden descendente.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Editado por nombre</p> </td> 
      <td> <p>Nombre del usuario que actualizó el propietario del proyecto.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Información adicional 1</p> </td> 
      <td> <p>El propietario actual del proyecto en el proyecto.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Información adicional 2</p> </td> 
      <td> <p>El propietario anterior del proyecto.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nombre del proyecto</p> </td> 
      <td> <p>Proyecto que tenía actualizado el campo Propietario del proyecto.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Para obtener más información sobre cómo agregar columnas, consulte [Información general sobre las vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. En el **Filtros** , haga clic en **Agregar regla de filtro** y, a continuación, agregue lo siguiente:

   * **Nombre del campo** > **Igual** > **ownerID**
   * **ID del proyecto** > **Igual** > **`<project name>`**

      ![](assets/qs-owner-changes-filter-350x94.png)
   Para obtener más información sobre cómo agregar filtros, consulte [Información general sobre filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Opcional) Para reducir el foco del informe y los tiempos de carga, agregue una solicitud.

   O

   Cree reglas de filtro adicionales para incluir proyectos, tareas o problemas específicos.

   >[!IMPORTANT]
   >
   >Creación de una regla de filtro que utilice el modificador **Contiene** puede aumentar los tiempos de carga. Por este motivo, se recomienda utilizar un modificador diferente como **Igual** cuando sea posible, filtrar por un proyecto específico o ID de objeto de nivel superior.

   Para obtener información sobre cómo añadir un mensaje, consulte [Agregar solicitudes a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. (Opcional) En la **Agrupaciones** , haga clic en **Aplicar una agrupación existente** y, a continuación, seleccione **Proyecto**.

   Para obtener más información sobre cómo añadir agrupaciones, consulte [Información general sobre las agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Haga clic en **Guardar + Cerrar**.

   Se carga el nuevo informe.
