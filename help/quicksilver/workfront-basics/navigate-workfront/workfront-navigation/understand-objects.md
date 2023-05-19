---
content-type: overview;reference
navigation-topic: workfront-navigation
title: Explicación de los objetos en [!DNL Adobe Workfront]
description: Explicación de los objetos en [!DNL Adobe Workfront]
feature: Get Started with Workfront
exl-id: f324f198-5472-4cf2-a46e-7fc24605ca90
source-git-commit: 888c938e5d649557df69374a55d4e4ecc2da6f55
workflow-type: tm+mt
source-wordcount: '2263'
ht-degree: 6%

---

# Explicación de los objetos en [!DNL Adobe Workfront]

<!--
<***Linked to several articles, do not remove/ change. 
-->

La información que se muestra en [!DNL Adobe Workfront] se representa mediante objetos que se almacenan en [!DNL Workfront] base de datos. Los objetos son los que generan la información [!DNL Workfront].

Explicación de cómo se definen los objetos en [!DNL Workfront] es importante para que pueda utilizar el objeto correcto para las necesidades necesarias en su organización.

Por ejemplo, cuando planea una gran cantidad de trabajo, debe utilizar la variable [!UICONTROL Proyecto] objeto para definir ese trabajo. Para dividir este trabajo en incrementos planificados más pequeños, puede usar el [!UICONTROL Tarea] objeto. Para una menor cantidad de trabajo que no está planificado y que puede producirse de forma inesperada, puede utilizar el objeto Issue. Si desea realizar un seguimiento del progreso y del cumplimiento del presupuesto y la cronología de un grupo de proyectos, puede organizarlos en [!UICONTROL Portfolio] y [!UICONTROL Programas]. Para definir otros elementos que le ayuden a resolver su trabajo, desea utilizar otros objetos almacenados en [!UICONTROL Proyectos], [!UICONTROL Tareas], [!UICONTROL Problemas], o [!UICONTROL Portfolio], como [!UICONTROL Documentos], [!UICONTROL Notas], [!UICONTROL Horas], [!UICONTROL Usuarios], o [!UICONTROL Funciones del puesto].

[!UICONTROL Informes] y [!UICONTROL Paneles] Este es otro ejemplo de objetos que pueden ayudarle a organizar la cantidad de datos que tiene en [!DNL Workfront] visualmente, para que sea fácilmente accesible para todos los usuarios.

Para obtener una lista completa de los objetos de [!DNL Workfront], consulte la [Explorador de API](../../../wf-api/general/api-explorer.md).

## Interdependencia y jerarquía de objetos

Los objetos están vinculados entre sí en [!UICONTROL Workfront]. Por ejemplo, una tarea o un problema nunca pueden existir de forma independiente fuera de un proyecto. [!UICONTROL Tareas] y [!UICONTROL problemas] son ejemplos de objetos que se almacenan en [!UICONTROL proyecto] objeto. [!UICONTROL Tareas] y [!UICONTROL problemas] se consideran objetos secundarios a los proyectos.

Los siguientes son algunos de los objetos más utilizados en [!DNL Workfront] y sus respectivos objetos principales y secundarios:

| **Objeto** | **Objetos principales** | **Objetos secundarios** |
|---|---|---|
| [!UICONTROL Portafolios] |  | [!UICONTROL Programas], [!UICONTROL Proyectos], [!UICONTROL Documentos], [!DNL Notes], [!UICONTROL Usuarios] |
| [!UICONTROL Programas] | [!UICONTROL Portafolios] | [!UICONTROL Proyectos], [!UICONTROL Documentos], [!UICONTROL Notas], [!UICONTROL Usuarios] |
| [!UICONTROL Proyectos] | [!UICONTROL Portfolio], [!UICONTROL Programas] | [!UICONTROL Tareas], [!UICONTROL Problemas], [!UICONTROL Documentos], [!UICONTROL Notas], [!UICONTROL Horas], [!UICONTROL Usuarios] |
| [!UICONTROL Tareas] | [!UICONTROL Proyectos] | [!UICONTROL Problemas], [!UICONTROL Tareas secundarias], [!UICONTROL Documentos], [!UICONTROL Notas], [!UICONTROL Horas], [!UICONTROL Usuarios] |
| [!UICONTROL Problemas] | [!UICONTROL Tareas], [!UICONTROL Proyectos] | [!UICONTROL Documentos], [!UICONTROL Notas], [!UICONTROL Horas], [!UICONTROL Usuarios] |
| [!UICONTROL Paneles] |  | [!UICONTROL Informes], Páginas externas |
| [!UICONTROL Informes] | [!UICONTROL Paneles] |  |
| [!UICONTROL Grupos] |  | [!UICONTROL Usuarios] |
| [!UICONTROL Equipos] |  | [!UICONTROL Usuarios] |
| [!UICONTROL Usuarios] | [!UICONTROL Grupos], [!UICONTROL Equipos], [!UICONTROL Compañías] | [!UICONTROL Roles] |
| [!UICONTROL Compañías] |  | [!UICONTROL Usuarios] |
| [!UICONTROL Documentos] | [!UICONTROL Tareas], [!UICONTROL Problemas], [!UICONTROL Proyectos], [!UICONTROL Portfolio], [!UICONTROL Programas], [!UICONTROL Usuarios] |  |
| [!UICONTROL Planes]* |  | [!UICONTROL Iniciativas] |
| [!DNL Goals]* |  | [!UICONTROL Resultados], [!UICONTROL Actividades] |

Para obtener una lista completa de los objetos de [!DNL Workfront], consulte la [Explorador de API](../../../wf-api/general/api-explorer.md).

*Los planes son los objetos del [!DNL Workfront Scenario Planner]. Para obtener más información sobre [!DNL Scenario Planner], consulte [El [!UICONTROL Planificador de escenarios] descripción general](../../../scenario-planner/scenario-planner-overview.md).

*[!UICONTROL Metas] son los objetos de [!DNL Workfront Goals]. Para obtener información acerca de [!DNL Workfront Goals], consulte [[!DNL Adobe Workfront Goals] descripción general](../../../workfront-goals/goal-management/wf-goals-overview.md).


## Personalizar nombres de objetos

As a [!DNL Workfront] administrador, puede personalizar los nombres de los objetos en [!DNL Workfront] mediante un  [!UICONTROL Plantilla de diseño].

Para obtener más información acerca de cómo personalizar nombres de objetos mediante una  [!UICONTROL Plantilla de diseño], consulte [Creación y administración de plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Después de personalizar una plantilla de diseño y asignarla a los usuarios, estos verán los nombres personalizados de los objetos. Los usuarios asignados a la plantilla de diseño ya no ven los nombres predeterminados para los objetos en ninguna parte de la aplicación web.

>[!NOTE]
>
>Para que los usuarios puedan ver los nuevos nombres de los objetos, deben cerrar la sesión y volver a iniciarla en [!DNL Workfront] después de guardar el  [!UICONTROL Plantilla de diseño].

>[!IMPORTANT]
>
>El [!DNL Workfront] La documentación de siempre hace referencia a los nombres predeterminados de los objetos. As a [!DNL Workfront] administrador, asegúrese de notificar a los usuarios los cambios en los nombres de los objetos, de modo que puedan comprender cómo utilizar el [!DNL Workfront] , así como las áreas de las aplicaciones que no reflejan los cambios en los nombres de los objetos.

* [Nombres de objeto que se pueden personalizar mediante una  [!UICONTROL Plantilla de diseño]](#object-names-that-can-be-customized-using-a-layout-template)
* [Áreas de [!DNL Workfront] que reflejan los nombres de objeto personalizados](#areas-of-workfront-that-reflect-the-customized-object-names)
* [Áreas de [!DNL Workfront] que no reflejan los nombres de objeto personalizados](#areas-of-workfront-that-do-not-reflect-the-customized-object-names)

### Nombres de objeto que se pueden personalizar mediante una [!UICONTROL Plantilla de diseño]

As a [!DNL Workfront] administrador, puede personalizar los nombres de los siguientes objetos para que coincidan con la terminología de su organización:

* [!UICONTROL Portafolio]
* [!UICONTROL Programar]
* [!UICONTROL Proyecto]
* [!UICONTROL Tarea]
* [!UICONTROL Problema]
* [!UICONTROL Meta]*
* [!UICONTROL Resultado]*
* [!UICONTROL Actividad]*

   *[!UICONTROL Metas], [!UICONTROL resultados], y [!UICONTROL actividades] solo están disponibles si su empresa ha adquirido [!DNL Workfront Goals]. Para obtener información acerca de [!DNL Workfront Goals], consulte [[!DNL Adobe Workfront Goals] descripción general](../../../workfront-goals/goal-management/wf-goals-overview.md).

* [!UICONTROL Iniciativa]**
* [!UICONTROL Escenario]**
* [!UICONTROL Plan]**

   **[!UICONTROL Iniciativas], [!UICONTROL escenarios], y [!UICONTROL planes] solo están disponibles si su empresa ha adquirido el [!DNL Workfront Scenario Planner]. Para obtener más información sobre [!DNL Scenario Planner], consulte [Introducción a la [!DNL Scenario Planner]](../../../scenario-planner/get-started-with-scenario-planning.md).


Por ejemplo, si la mayor cantidad de trabajo en su organización se conoce como &quot;Participación&quot;, puede reemplazar el nombre &quot;[!UICONTROL Proyecto]&#39; con &#39;Participación&#39;. Su [!DNL Workfront] La interfaz muestra &quot;Participación&quot; en lugar de &quot;[!UICONTROL Proyecto]&#39; en todas partes donde el nombre &#39;[!UICONTROL Proyecto]&#39; aparecería.

Para obtener más información acerca de cómo personalizar nombres de objetos mediante  [!UICONTROL Plantillas de diseño], consulte [Creación y administración de plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

No se pueden personalizar los nombres de ningún otro objeto en Workfront. Para obtener una lista completa de los objetos de [!DNL Workfront], consulte la [Explorador de API](../../../wf-api/general/api-explorer.md).

Al personalizar el nombre de un objeto, el nuevo nombre para ese objeto aparece en la mayoría de las áreas del [!DNL Workfront] aplicación en la que aparecería ese nombre de objeto.

### Áreas de [!DNL Workfront] que reflejan los nombres de objeto personalizados

Las áreas siguientes muestran el nombre actualizado de los objetos:

* Navegación superior
* Todas las secciones de la navegación del panel izquierdo
* Todos los menús
* Notificaciones en la aplicación
* Report Builder y los elementos de informes (vistas, filtros y agrupaciones)
* [!UICONTROL Guardar] botones
* Archivos exportados
* Correos electrónicos
* Aplicaciones móviles

### Áreas de [!DNL Workfront] que no reflejan los nombres de objeto personalizados

Las áreas siguientes no muestran el nombre actualizado de los objetos:

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Referenced Object Type selection for a Typeahead field in a Custom Form </p> <p>(NOTE: drafting this because I don't think this is true)</p> </li>
  -->

* [!DNL Outlook] Complemento de

## Implicaciones de la personalización de nombres de objetos

Debe tener en cuenta lo siguiente al personalizar los nombres de objeto en [!DNL Workfront]:

* Puede encontrar errores estilísticos o gramaticales en las pantallas del sistema. Por ejemplo, si cambia el nombre a[!UICONTROL Problema]&#39; a &#39;Solicitud&#39; y ve en cualquier parte del sistema la frase &#39;Una solicitud&#39;, esto está funcionando según lo previsto y no debe considerarse un error.
* Los nombres personalizados de los objetos no se pueden traducir. Solo el [!DNL Workfront] los nombres predeterminados se pueden traducir a los idiomas compatibles. Para obtener más información sobre los idiomas compatibles con [!DNL Workfront], consulte [Idiomas admitidos en [!DNL Adobe Workfront]](../../../workfront-basics/supported-languages-in-workfront.md). Los campos de nombre de objeto personalizado admiten caracteres extranjeros para que pueda introducir la terminología en cualquier idioma.
* Cuando se personalizan los nombres de objeto mediante una  [!UICONTROL Plantilla de diseño], le recomendamos que asigne sus  [!UICONTROL Plantillas de diseño] en torno a sus unidades de negocio (equipos o grupos).\
   Le recomendamos que utilice nombres que los usuarios de estas unidades de negocio entiendan claramente, para evitar confusiones.
* Las notificaciones por correo electrónico y los informes enviados siempre contienen nombres de objeto tal como se define en la variable  [!UICONTROL Plantilla de diseño] del usuario que genera el correo electrónico. Los usuarios deben estar preparados para ver nombres de objetos en sus correos electrónicos que no estén relacionados con su grupo o equipo si reciben notificaciones por correo electrónico de usuarios de otros equipos y grupos.\
   As a [!DNL Workfront] administrador, aconseje a los usuarios que observen los iconos asociados a cada objeto. Los iconos permanecen coherentes entre los distintos nombres de objeto y con el objeto predeterminado, tal como aparece en la base de datos. Para obtener una lista de todos [!DNL Workfront] iconos asociados a objetos, consulte [Iconos de objeto](#object-icons).

   >[!TIP]
   >
   >Para tareas comunes en su organización, considere la posibilidad de crear documentación personalizada que refleje su terminología.

## Iconos de objeto

El [!DNL Workfront] La documentación de siempre hace referencia a los nombres predeterminados de los objetos. Si los objetos tienen sus nombres personalizados, puede confiar en el icono asociado a ellos para comprender qué objeto personalizado corresponde a qué [!DNL Workfront] objeto predeterminado.

Para obtener más información sobre los objetos que pueden tener nombres personalizados en [!DNL Workfront], consulte [Nombres de objeto que se pueden personalizar mediante una  [!UICONTROL Plantilla de diseño]](#object-names-that-can-be-customized-using-a-layout-template).

A continuación se muestra una lista de objetos y sus iconos correspondientes en Workfront.

| **Objeto** | **Icono** | **Nombre de objeto personalizable** |
|---|---|---|
| [!UICONTROL Compañía] | ![](assets/company-icon-nwe.png)  , ![](assets/nwe-company-icon-54x54.png) |  |
| [!UICONTROL Panel] | ![](assets/dashboard-icon-nwe.png)  , ![](assets/nwe-dashboards-icon.png) |  |
| [!UICONTROL Meta] | ![](assets/nwe-goal-icon.png) | ✔ |
| [!UICONTROL Grupo] | ![](assets/groups-icon-nwe.png)  , ![](assets/nwe-group-icon.png) |  |
| [!UICONTROL Problema] | ![](assets/issue-icon-nwe.png)  , ![](assets/nwe-issues-icon.png) | ✔ |
| [!UICONTROL Función] | ![job_role_icon.png](assets/job-role-icon-52x50.png), ![job_role_icon__1_.png](assets/job-role-icon--1--53x44.png), ![](assets/job-role-nwe-no-color.png), ![](assets/job-role-icon-nwe-color.png) |  |
| [!UICONTROL Plan] | ![](assets/plan-icon.png), ![](assets/nwe-plan-icon-60x57.png) |  |
| [!UICONTROL Portafolio] | ![](assets/portfolio-icon-nwe.png)  , ![](assets/nwe-portfolios-icon.png) | ✔ |
| [!UICONTROL Programar] | ![](assets/program-icon-nwe.png)  , ![](assets/nwe-programs-icon.png) | ✔ |
| [!UICONTROL Proyecto] | ![](assets/project-icon-nwe.png)  , ![](assets/nwe-projects-icon.png) | ✔ |
| [!UICONTROL Informe] | ![](assets/report-icon-nwe.png) , ![](assets/nwe-reports-icon.png) |  |
| [!UICONTROL Tarea] | ![](assets/task-icon-new.png)  , ![](assets/nwe-tasks-icon.png) | ✔ |
| [!UICONTROL Equipo] | ![](assets/team-icon-nwe.png), ![](assets/team-icon-nwe-color.png) , ![](assets/nwe-teams-icon.png) |  |
| [!UICONTROL Plantilla] | ![](assets/template-icon-nwe.png)  , ![](assets/nwe-templates-icon.png) |  |

## Números de referencia de objetos

Cada objeto creado en [!DNL Workfront] tiene asignado un número de referencia único. Los números de referencia son útiles para distinguir entre dos objetos similares (como tareas con el mismo nombre). Se pueden buscar objetos utilizando sus números de referencia y se pueden incluir números de referencia en los informes.

Para obtener información sobre cómo buscar objetos por número de referencia, consulte [Utilizar el número de referencia de objetos](../../../workfront-basics/navigate-workfront/search/reference-number-of-objects.md).

## Búsquedas específicas de objetos

Puede buscar en todos los objetos en los que se puede buscar [!DNL Workfront]o bien, puede seleccionar un objeto específico para buscarlo en las búsquedas básicas y avanzadas.

No se pueden buscar todos los objetos en [!DNL Workfront]. Puede ejecutar búsquedas básicas y avanzadas de los siguientes objetos en [!DNL Workfront]:

| **Objeto** | **Búsqueda básica** | **Búsqueda avanzada** |
|---|---|---|
| [!UICONTROL Proyectos] | ✓ | ✓ |
| [!UICONTROL Tareas] | ✓ | ✓ |
| [!UICONTROL Problemas] | ✓ | ✓ |
| [!UICONTROL Informes] | ✓ | ✓ |
| [!UICONTROL Usuarios] | ✓ | ✓ |
| [!UICONTROL Plantillas] | ✓ | ✓ |
| [!UICONTROL Documentos] | ✓ | ✓ |
| [!UICONTROL Portafolios] | ✓ | ✓ |
| [!UICONTROL Programas] | ✓ | ✓ |
| [!UICONTROL Paneles] | ✓ | ✓ |
| [!UICONTROL Compañías] | ✓ | ✓ |
| [!UICONTROL Notas] | ✓ |  |

Para obtener más información sobre cómo ejecutar búsquedas básicas y avanzadas en [!DNL Workfront], consulte [Buscar [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

## Informar sobre objetos

Es extremadamente importante comprender la jerarquía y la interdependencia de los objetos antes de empezar a crear informes en [!DNL Workfront]. Los informes son específicos de objetos. Debe seleccionar el objeto correcto para el informe antes de poder mostrar los datos deseados.

Según el objeto que haya seleccionado para el informe, sólo podrá acceder a los objetos que estén directamente vinculados al objeto del informe.

>[!IMPORTANT]
>
>Sólo puede crear informes sobre el objeto seleccionado y los objetos principales en el mismo informe. No se puede tener información sobre los objetos secundarios en un informe de objeto principal. Por ejemplo, se puede mostrar la información del proyecto en un informe de tareas, pero no la información de tareas en un informe de proyecto.

Puede crear informes sobre todos los objetos de la base de datos utilizando nuestra API abierta. Para obtener una lista completa de todos los objetos de la base de datos, consulte [Explorador de API](../../../wf-api/general/api-explorer.md).

>[!NOTE]
>
>Si ha personalizado los nombres de los objetos mediante una plantilla de diseño, también se han personalizado los nombres de los objetos en Report Builder. Asegúrese de saber qué objetos se han personalizado y de buscar el nombre personalizado en Report Builder. Para obtener más información sobre los objetos que pueden tener nombres personalizados en [!DNL Workfront], consulte *[Nombres de objeto que se pueden personalizar mediante una  [!UICONTROL Plantilla de diseño]](#object-names-that-can-be-customized-using-a-layout-template).*
>Cuando se utiliza el modo de texto en los informes, los nombres de los objetos en las expresiones del modo de texto son los nombres estándar en [!DNL Workfront]y no los nombres de objeto personalizados. Para obtener más información sobre el uso del modo de texto en los informes, consulte [Introducción al modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Para obtener más información sobre la creación de informes, consulte [Creación de un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
Para obtener más información sobre nuestra API, consulte [Explorador de API](../../../wf-api/general/api-explorer.md).

Puede crear informes sobre los siguientes objetos al usar Report Builder en [!DNL Workfront] aplicación web:

* [!UICONTROL Proyecto]
* [!UICONTROL Tarea]
* [!UICONTROL Hora]
* [!UICONTROL Problema]
* [!UICONTROL Usuario]
* [!UICONTROL Nivel de acceso]
* [!UICONTROL Ruta de aprobación]
* [!UICONTROL Proceso de aprobación]
* [!UICONTROL Asignación]
* [!UICONTROL Elemento de trabajo pendiente]\
   Muestra tareas o problemas en el registro de pendientes Agile. Para obtener más información sobre el registro de pendientes de Agile, consulte [Administrar el registro de pendientes Agile](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

* [!UICONTROL Línea base]
* [!UICONTROL Tarea de línea base]
* [!UICONTROL Registro de facturación]
* [!UICONTROL Hora presupuestadas]

   Este es el [!UICONTROL Horas presupuestadas], tal como aparecen en las herramientas de administración de recursos obsoletas más antiguas.

   El &quot;Bud&quot;. &quot;Horas&quot; en el campo [!UICONTROL Hora presupuestada] hace referencia a las horas presupuestadas para los roles en el [!UICONTROL Planificador de recursos]. Para obtener más información, consulte [Comprender [!UICONTROL Costo laboral presupuestado] y [!UICONTROL Horas presupuestadas] para proyectos](../../../manage-work/projects/project-finances/budgeted-labor-cost.md).

* [!UICONTROL Evento de calendario]
* [!UICONTROL Categoría] (o [!UICONTROL Formulario personalizado])
* [!UICONTROL Compañía]
* [!UICONTROL Panel]
* [!UICONTROL Documento]
* [!UICONTROL Aprobación de documento]
* [!UICONTROL Versión de documento]\
   Permite ver información diversa acerca de la versión del documento, el documento con el que está asociada la versión, quién creó la versión y el usuario que creó la prueba en la versión del documento, si existe (Creador de pruebas).
* [!UICONTROL Plantilla de mensaje de correo electrónico]
* [!UICONTROL Gasto]
* [!UICONTROL Tipo de gasto]
* [!UICONTROL Página externa]
* [!UICONTROL Favorito]
* [!UICONTROL Filtro]
* [!UICONTROL Meta]

   Puede generar un informe para metas estratégicas o mostrar información relacionada con las metas en un informe de proyecto cuando los proyectos están asociados con metas como actividades de metas. Puede crear objetivos estratégicos y conectar proyectos con ellos solo si su organización ha adquirido un [!DNL Workfront Goals] licencia. Para obtener información acerca de [!DNL Workfront Goals], consulte [[!DNL Workfront Goals] descripción general](../../../workfront-goals/goal-management/wf-goals-overview.md). Para obtener información sobre cómo conectar proyectos con objetivos estratégicos, consulte [Agregar proyectos a metas en Adobe Workfront Goals](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: hardcoded links in this paragraph)
  </MadCap:conditionalText>
  -->

   >[!TIP]
   >
   >No se puede informar sobre los objetivos del proyecto asociados a una [!UICONTROL Caso comercial]. Para obtener información sobre los objetivos del proyecto frente a los objetivos estratégicos, consulte [Glosario de [!DNL Adobe Workfront] terminología](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* [!UICONTROL Grupo]
* [!UICONTROL Agrupación]
* [!UICONTROL Tipo de hora]
* [!UICONTROL Iniciativa]

   Puede crear un informe para iniciativas que sean los objetos secundarios de un plan solo si su compañía ha adquirido un [!DNL Workfront Scenario Planner] licencia. Para obtener información sobre las iniciativas, consulte [Resumen de las iniciativas en [!DNL Workfront Scenario Planner]](../../../scenario-planner/initiatives-overview.md).


* Función del puesto de la iniciativa

   Puede crear un informe para las funciones del puesto asociadas con las iniciativas de un plan solo si su empresa ha adquirido un [!DNL Workfront Scenario Planner] licencia. Para obtener información sobre la creación de iniciativas y su asociación con funciones del puesto, consulte [Cree y edite iniciativas en [!DNL Workfront Scenario Planner]](../../../scenario-planner/create-and-edit-initiatives.md).


* [!UICONTROL Iteración]
* [!UICONTROL Función]
* [!UICONTROL Entrada de cuaderno]

   Puede informar sobre las actualizaciones del sistema rastreadas en el [!UICONTROL Actualizaciones] área de objetos como tareas, proyectos, problemas, etc. Para obtener más información, consulte [Informe sobre la [!UICONTROL Actualizaciones] área](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

* [!UICONTROL Plantilla de diseño]
* [!UICONTROL Hito]
* [!UICONTROL Ruta de hitos]
* [!UICONTROL Nota]

   >[!NOTE]
   >
   >Puede informar sobre los comentarios agregados por usuarios individuales.

* [!UICONTROL Parámetro] (o [!UICONTROL Campo personalizado])
* [!UICONTROL Grupo de parámetros] (o [!UICONTROL Salto de sección])
* [!UICONTROL Perfil de portal] (esto muestra información que se ha desaprobado)
* [!UICONTROL Portafolio]
* [!UICONTROL Programar]
* [!UICONTROL Proyecto] ([!UICONTROL Datos financieros])

   >[!NOTE]
   >
   >La información financiera se rellena en [!UICONTROL Proyecto] ([!UICONTROL Datos financieros]) informa solamente cuando los datos asociados con él tienen menos de 5 años. Por ejemplo, si se asignó una función a una tarea en enero de 2015 y hoy es septiembre de 2021, un campo financiero como el [!UICONTROL Fecha de asignación] para el rol no se rellena en la variable [!UICONTROL Proyecto (datos financieros)] informe.

* [!UICONTROL Aprobación de revisión]\
   Permite ver información diversa acerca de la aprobación de pruebas, incluyendo: la prueba que se envió para su aprobación, información acerca de [!UICONTROL Aprobador], información sobre el solicitante (si el solicitante tiene licencia para [!DNL Workfront] usuario), información de la versión, el ID de prueba y la fecha de creación de la prueba.\
   [!UICONTROL Aprobación de revisión] Los informes de solo incluyen pruebas disponibles en las áreas de Mi trabajo de los usuarios en las que aún no se han tomado decisiones.\
   Las aprobaciones de revisión se asignan en [!DNL Workfront] como se describe [Adición de usuarios a una prueba](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) in [Compartir una prueba en [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

* [!UICONTROL Cola]
* [!UICONTROL Tema de la cola]
* [!UICONTROL Tarifa] (muestra el rol [!UICONTROL Tarifa de facturación] information)
* [!UICONTROL Notificación de recordatorio]
* [!UICONTROL Informe]
* [!UICONTROL Conjunto de recursos]
* [!UICONTROL Riesgo]
* [!UICONTROL Tipo de riesgo]
* [!UICONTROL Programación]
* [!UICONTROL Tarjeta de puntuación]
* [!UICONTROL Equipo]
* [!UICONTROL Plantilla]
* [!UICONTROL Tarea de plantilla]
* [!UICONTROL Tiempo libre]

   Puede crear informes sobre el tiempo libre de un usuario, tal como lo indique el usuario en su perfil.

* [!UICONTROL Hoja de horas]
* [!UICONTROL Perfil de hoja de horas]
* [!UICONTROL Grupo de temas]
* [!UICONTROL Delegación de usuario]

   Puede informar sobre los usuarios que se han delegado para realizar las tareas y los problemas de otros mientras están fuera de la oficina. Este informe muestra el usuario que está fuera de la oficina, así como el usuario que cumple con sus obligaciones mientras está fuera.

* [!UICONTROL Vista]
* [!UICONTROL Elemento de trabajo] (se refiere a tareas y problemas)
