---
content-type: overview;reference
navigation-topic: workfront-navigation
title: Explicación de los objetos de [!DNL Adobe Workfront]
description: Explicación de los objetos de [!DNL Adobe Workfront]
feature: Get Started with Workfront
exl-id: f324f198-5472-4cf2-a46e-7fc24605ca90
source-git-commit: 9c78d8e08e62c86a4e1340644ed76c61ce7f2674
workflow-type: tm+mt
source-wordcount: '2308'
ht-degree: 6%

---

# Explicación de los objetos de [!DNL Adobe Workfront]

<!--
<***Linked to several articles, do not remove/ change. 
-->

La información que se muestra en [!DNL Adobe Workfront] se representa mediante objetos almacenados en la variable [!DNL Workfront] base de datos. Los objetos son lo que impulsa la información en [!DNL Workfront].

Explicación de cómo se definen los objetos en [!DNL Workfront] es importante para poder usar el objeto correcto según las necesidades de su organización.

Por ejemplo, cuando planifica una gran cantidad de trabajo, debe usar la variable [!UICONTROL Proyecto] para definir ese trabajo. Para dividir este trabajo en incrementos planificados más pequeños, puede usar la variable [!UICONTROL Tarea] objeto. Para una menor cantidad de trabajo que no está planificado y que puede producirse de forma inesperada, puede utilizar el objeto Problema . Si desea realizar un seguimiento del progreso y del cumplimiento del presupuesto y la cronología de un grupo de proyectos, puede organizarlos en [!UICONTROL Portfolio] y [!UICONTROL Programas]. Para definir otros elementos que le ayuden a resolver su trabajo, desea utilizar otros objetos almacenados en [!UICONTROL Proyectos], [!UICONTROL Tareas], [!UICONTROL Problemas]o [!UICONTROL Portfolio], like [!UICONTROL Documentos], [!UICONTROL Notas], [!UICONTROL Horas], [!UICONTROL Usuarios]o [!UICONTROL Funciones del trabajo].

[!UICONTROL Informes] y [!UICONTROL Tableros] son otro ejemplo de objetos que puede ayudarle a organizar la cantidad de datos que tiene en [!DNL Workfront] visualmente, para que sea fácilmente accesible para todos los usuarios.

Para obtener una lista completa de los objetos de [!DNL Workfront], consulte la [Explorador de API](../../../wf-api/general/api-explorer.md).

## Interdependencia y jerarquía de objetos

Los objetos están vinculados entre sí en [!UICONTROL Workfront]. Por ejemplo, una tarea o un problema nunca pueden existir de forma independiente fuera de un proyecto. [!UICONTROL Tareas] y [!UICONTROL problemas] son ejemplos de objetos almacenados en la variable [!UICONTROL proyecto] objeto. [!UICONTROL Tareas] y [!UICONTROL problemas] se consideran objetos secundarios de los proyectos.

A continuación se indican algunos de los objetos más utilizados en [!DNL Workfront] y sus respectivos objetos principales y secundarios:

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

*Los planes son los objetos del [!DNL Workfront Scenario Planner]. Para obtener información sobre la variable [!DNL Scenario Planner], consulte [La variable [!UICONTROL Planificador de escenario] información general](../../../scenario-planner/scenario-planner-overview.md).

*[!UICONTROL Objetivos] son los objetos de [!DNL Workfront Goals]. Para obtener información sobre [!DNL Workfront Goals], consulte [[!DNL Adobe Workfront Goals] información general](../../../workfront-goals/goal-management/wf-goals-overview.md).


## Personalizar nombres de objeto

Como [!DNL Workfront] administrador, puede personalizar nombres de objeto en [!DNL Workfront] mediante una  [!UICONTROL Plantilla de diseño].

Para obtener más información sobre cómo personalizar nombres de objetos mediante un  [!UICONTROL Plantilla de diseño], consulte [Creación y administración de plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Después de personalizar una plantilla de diseño y asignarla a los usuarios, estos verán los nombres personalizados de los objetos. Los usuarios asignados a la plantilla de diseño ya no ven los nombres predeterminados de los objetos en ninguna parte de la aplicación web.

>[!NOTE]
>
>Para que los usuarios puedan ver los nuevos nombres de los objetos, deben cerrar la sesión y volver a iniciarla en [!DNL Workfront] después de guardar la variable  [!UICONTROL Plantilla de diseño].

>[!IMPORTANT]
>
>La variable [!DNL Workfront] La documentación siempre hace referencia a los nombres predeterminados de los objetos. Como [!DNL Workfront] administrador, asegúrese de notificar a los usuarios los cambios en los nombres de los objetos para que puedan comprender cómo usar la variable [!DNL Workfront] documentación, así como las áreas de las aplicaciones que no reflejan los cambios en los nombres de los objetos.

* [Nombres de objetos que se pueden personalizar mediante un  [!UICONTROL Plantilla de diseño]](#object-names-that-can-be-customized-using-a-layout-template)
* [Áreas de [!DNL Workfront] que reflejan los nombres de objeto personalizados](#areas-of-workfront-that-reflect-the-customized-object-names)
* [Áreas de [!DNL Workfront] que no reflejan los nombres de objeto personalizados](#areas-of-workfront-that-do-not-reflect-the-customized-object-names)

### Nombres de objetos que se pueden personalizar mediante un [!UICONTROL Plantilla de diseño]

Como [!DNL Workfront] administrador, puede personalizar los nombres de los siguientes objetos para que coincidan con la terminología de su organización:

* [!UICONTROL Portafolio]
* [!UICONTROL Programar]
* [!UICONTROL Proyecto]
* [!UICONTROL Tarea]
* [!UICONTROL Problema]
* [!UICONTROL Meta]*
* [!UICONTROL Resultado]*
* [!UICONTROL Actividad]*

   *[!UICONTROL Objetivos], [!UICONTROL resultados]y [!UICONTROL actividades] solo están disponibles si su empresa ha comprado [!DNL Workfront Goals]. Para obtener información sobre [!DNL Workfront Goals], consulte [[!DNL Adobe Workfront Goals] información general](../../../workfront-goals/goal-management/wf-goals-overview.md).

* [!UICONTROL Iniciativa]**
* [!UICONTROL Escenario]**
* [!UICONTROL Plan]**

   **[!UICONTROL Iniciativas], [!UICONTROL escenarios]y [!UICONTROL planes] solo están disponibles si su empresa ha adquirido la variable [!DNL Workfront Scenario Planner]. Para obtener información sobre la variable [!DNL Scenario Planner], consulte [Introducción a [!DNL Scenario Planner]](../../../scenario-planner/get-started-with-scenario-planning.md).


Por ejemplo, si la mayor cantidad de trabajo de su organización se conoce como &quot;Participación&quot;, puede reemplazar el nombre &quot;[!UICONTROL Proyecto]&#39; con &#39;Participación&#39;. Su [!DNL Workfront] la interfaz muestra &quot;Participación&quot; en lugar de &quot;[!UICONTROL Proyecto]&#39; en todas partes donde el nombre &#39;[!UICONTROL Proyecto]&#39; aparecería.

Para obtener más información sobre cómo personalizar nombres de objetos mediante  [!UICONTROL Plantillas de diseño], consulte [Creación y administración de plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

No se pueden personalizar los nombres de ningún otro objeto en Workfront. Para obtener una lista completa de los objetos de [!DNL Workfront], consulte la [Explorador de API](../../../wf-api/general/api-explorer.md).

Cuando se personaliza el nombre de un objeto, el nuevo nombre de ese objeto aparece en la mayoría de las áreas del [!DNL Workfront] aplicación donde aparecerá ese nombre de objeto.

### Áreas de [!DNL Workfront] que reflejan los nombres de objeto personalizados

Las siguientes áreas muestran el nombre actualizado de los objetos:

* Navegación superior
* Todas las secciones del panel de navegación izquierdo
* Todos los menús
* Notificaciones en la aplicación
* Creador de informes y elementos de informes (vistas, filtros y agrupaciones)
* [!UICONTROL Guardar] botones
* Archivos exportados
* Correos electrónicos
* Aplicaciones móviles

### Áreas de [!DNL Workfront] que no reflejan los nombres de objeto personalizados

Las siguientes áreas no muestran el nombre actualizado de los objetos:

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Referenced Object Type selection for a Typeahead field in a Custom Form </p> <p>(NOTE: drafting this because I don't think this is true)</p> </li>
  -->

* [!DNL Outlook] Complemento

## Implicaciones de personalizar nombres de objetos

Debe tener en cuenta lo siguiente al personalizar nombres de objeto en [!DNL Workfront]:

* Puede encontrar errores estilísticos o gramaticales en las visualizaciones del sistema. Por ejemplo, si cambia el nombre de &#39;[!UICONTROL Problema]&#39; para &#39;Solicitar&#39; y usted ve en cualquier parte del sistema la frase &#39;Una solicitud&#39;, esto está funcionando como se pretende y no debe considerarse un error.
* Los nombres personalizados de los objetos no se pueden traducir. Solo el [!DNL Workfront] los nombres predeterminados se pueden traducir a los idiomas compatibles. Para obtener más información sobre los idiomas compatibles con [!DNL Workfront], consulte [Idiomas admitidos en [!DNL Adobe Workfront]](../../../workfront-basics/supported-languages-in-workfront.md). Los campos de nombre de objeto personalizados admiten caracteres extranjeros, por lo que se puede introducir la terminología en cualquier idioma.
* Al personalizar los nombres de los objetos mediante un  [!UICONTROL Plantilla de diseño], le recomendamos que asigne su  [!UICONTROL Plantillas de diseño] alrededor de las unidades de negocio (equipos o grupos).\
   Para evitar confusiones, le recomendamos que utilice nombres que los usuarios de estas unidades de negocio entiendan claramente.
* Las notificaciones por correo electrónico y los informes enviados siempre contienen nombres de objeto según se define en la variable  [!UICONTROL Plantilla de diseño] del usuario que genera el correo electrónico. Los usuarios deben estar preparados para ver los nombres de objetos en sus correos electrónicos que no están relacionados con su grupo o equipo, si reciben notificaciones por correo electrónico de usuarios de otros equipos y grupos.\
   Como [!DNL Workfront] administrador, aconseje a los usuarios que observen los iconos asociados a cada objeto. Los iconos siguen siendo coherentes entre los distintos nombres de objeto y con el objeto predeterminado, tal como aparece en la base de datos. Para una lista de todos [!DNL Workfront] iconos asociados a objetos, consulte [Iconos de objetos](#object-icons).

   >[!TIP]
   >
   >Para tareas comunes en su organización, considere la posibilidad de crear documentación personalizada para reflejar su terminología.

## Iconos de objetos

La variable [!DNL Workfront] La documentación siempre hace referencia a los nombres predeterminados de los objetos. Si los nombres de los objetos se han personalizado, puede confiar en el icono asociado a ellos para comprender qué objeto personalizado corresponde a cuál [!DNL Workfront] objeto predeterminado.

Para obtener más información sobre los objetos que pueden tener nombres personalizados en [!DNL Workfront], consulte [Nombres de objetos que se pueden personalizar mediante un  [!UICONTROL Plantilla de diseño]](#object-names-that-can-be-customized-using-a-layout-template).

A continuación se muestra una lista de objetos y sus iconos correspondientes en Workfront.

| **Objeto** | **Icono** | **Nombre de objeto personalizable** |
|---|---|---|
| [!UICONTROL Compañía] | ![](assets/company-icon-nwe.png)  , ![](assets/nwe-company-icon-54x54.png) |  |
| [!UICONTROL Panel] | ![](assets/dashboard-icon-nwe.png)  , ![](assets/nwe-dashboards-icon.png) |  |
| [!UICONTROL Meta] | ![](assets/nwe-goal-icon.png) | š |
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

Cada objeto creado en [!DNL Workfront] se asigna un número de referencia único. Los números de referencia son útiles para distinguir entre dos objetos similares (como tareas con el mismo nombre). Puede buscar objetos utilizando sus números de referencia y puede incluir números de referencia en los informes.

Para obtener información sobre cómo buscar objetos por número de referencia, consulte [Usar el número de referencia de los objetos](../../../workfront-basics/navigate-workfront/search/reference-number-of-objects.md).

## Búsquedas específicas de objetos

Puede buscar en todos los objetos en los que se puede buscar [!DNL Workfront]o puede seleccionar un objeto específico para buscarlo en las búsquedas básicas y avanzadas.

No todos los objetos se pueden buscar en [!DNL Workfront]. Puede ejecutar búsquedas básicas y avanzadas de los siguientes objetos en [!DNL Workfront]:

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

Comprender la jerarquía y la interdependencia de los objetos es extremadamente importante antes de comenzar a crear informes en [!DNL Workfront]. Los informes son específicos de cada objeto. Debe seleccionar el objeto correcto para el informe antes de poder mostrar los datos que desee.

Según el objeto que haya seleccionado para el informe, solo puede acceder a los objetos directamente vinculados al objeto del informe.

>[!IMPORTANT]
>
>Solo se puede informar sobre el objeto seleccionado y los objetos principales del mismo informe. No se puede tener información sobre los objetos secundarios en un informe de objeto principal. Por ejemplo, puede mostrar la información del proyecto en un informe de tareas, pero no la información de tareas en un informe de proyecto.

Puede informar sobre todos los objetos de la base de datos mediante nuestra API abierta. Para obtener una lista completa de todos los objetos de la base de datos, consulte [Explorador de API](../../../wf-api/general/api-explorer.md).

>[!NOTE]
>
>Si ha personalizado los nombres de los objetos mediante una plantilla de diseño, también se han personalizado los nombres del objeto en el Creador de informes. Asegúrese de saber qué objetos se han personalizado y de buscar el nombre personalizado en el Creador de informes. Para obtener más información sobre los objetos que pueden tener nombres personalizados en [!DNL Workfront], consulte *[Nombres de objetos que se pueden personalizar mediante un  [!UICONTROL Plantilla de diseño]](#object-names-that-can-be-customized-using-a-layout-template).*
>Cuando se utiliza el modo de texto en los informes, los nombres de los objetos en las expresiones del modo de texto son los nombres estándar en [!DNL Workfront]y no los nombres de objeto personalizados. Para obtener más información sobre el uso del modo de texto en los informes, consulte [Información general sobre el modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Para obtener más información sobre cómo crear un informe, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
Para obtener más información sobre nuestra API, consulte [Explorador de API](../../../wf-api/general/api-explorer.md).

Con el Creador de informes en la variable [!DNL Workfront] aplicación web:

* [!UICONTROL Proyecto]
* [!UICONTROL Tarea]
* [!UICONTROL Hora]
* [!UICONTROL Problema]
* [!UICONTROL Usuario]
* [!UICONTROL Nivel de acceso]
* [!UICONTROL Ruta de aprobación]
* [!UICONTROL Proceso de aprobación]
* [!UICONTROL Asignación]
* [!UICONTROL Elemento de trabajo atrasado]\
   Muestra las tareas o los problemas en el registro de trabajo acumulado. Para obtener más información sobre el trabajo atrasado en Agile, consulte [Administrar el trabajo atrasado ágil](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

* [!UICONTROL Línea base]
* [!UICONTROL Tarea de línea base]
* [!UICONTROL Registro de facturación]
* [!UICONTROL Hora presupuestadas]

   Esta es la [!UICONTROL Horas presupuestadas], tal y como aparecen en el en herramientas de administración de recursos obsoletas y antiguas.

   El &quot;Bud&quot;. Horas&quot; en el campo [!UICONTROL Hora presupuestada] hace referencia a las horas presupuestadas para las funciones de trabajo en la variable [!UICONTROL Planificador de recursos]. Para obtener más información, consulte [Comprender [!UICONTROL Coste de trabajo presupuestado] y [!UICONTROL Horas presupuestadas] para proyectos](../../../manage-work/projects/project-finances/budgeted-labor-cost.md).

* [!UICONTROL Evento de calendario]
* [!UICONTROL Categoría] (o [!UICONTROL Formulario personalizado])
* [!UICONTROL Compañía]
* [!UICONTROL Panel]
* [!UICONTROL Documento]
* [!UICONTROL Aprobación de documento]
* [!UICONTROL Versión de documento]\
   Permite ver información diversa sobre la versión del documento, el documento al que está asociada la versión, quién creó la versión y el usuario que creó la prueba en la versión del documento si existe (Creador de pruebas).
* [!UICONTROL Plantilla de mensaje de correo electrónico]
* [!UICONTROL Gasto]
* [!UICONTROL Tipo de gasto]
* [!UICONTROL Página externa]
* [!UICONTROL Favorito]
* [!UICONTROL Filtro]
* [!UICONTROL Meta]

   Puede crear un informe para objetivos estratégicos o mostrar información relacionada con objetivos en un informe de proyecto cuando los proyectos estén asociados a objetivos como actividades de objetivos. Puede crear objetivos estratégicos y conectar proyectos solo si su organización ha adquirido un [!DNL Workfront Goals] licencia. Para obtener información sobre [!DNL Workfront Goals], consulte [[!DNL Workfront Goals] información general](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FWorkfront_Goals%2FGoal_management%2Fwf-goals-overview.htm&amp;_LANG=en). Para obtener información sobre la conexión de proyectos a objetivos estratégicos, consulte [Agregar proyectos a objetivos en Objetivos de Adobe Workfront](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FWorkfront_Goals%2FResults_and_activities%2Fconnect-projects-to-goals-overview.htm&amp;_LANG=en).

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: hardcoded links in this paragraph)
  </MadCap:conditionalText>
  -->

   >[!TIP]
   >
   >No puede generar informes sobre los objetivos de proyecto asociados con un [!UICONTROL Caso empresarial]. Para obtener información sobre los objetivos del proyecto frente a los objetivos estratégicos, consulte [Glosario de [!DNL Adobe Workfront] terminología](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* [!UICONTROL Grupo]
* [!UICONTROL Agrupación]
* [!UICONTROL Tipo de hora]
* [!UICONTROL Iniciativa]

   Puede crear un informe para iniciativas que sean los objetos secundarios de un plan solo si su empresa ha adquirido un [!DNL Workfront Scenario Planner] licencia. Para obtener información sobre iniciativas, consulte [Información general sobre las iniciativas de [!DNL Workfront Scenario Planner]](https://one.workfront.com/s/csh?context=2066&amp;pubname=the-new-workfront-experience).

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this link is hardcoded)
  </MadCap:conditionalText>
  -->

* Función del puesto de la iniciativa

   Puede crear un informe para las funciones de trabajo asociadas con las iniciativas de un plan solo si su empresa ha adquirido un [!DNL Workfront Scenario Planner] licencia. Para obtener información sobre cómo crear iniciativas y asociarlas a funciones de trabajo, consulte [Cree y edite iniciativas en la [!DNL Workfront Scenario Planner]](https://one.workfront.com/s/csh?context=2061&amp;pubname=the-new-workfront-experience).

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this link is hardcoded)
  </MadCap:conditionalText>
  -->

* [!UICONTROL Iteración]
* [!UICONTROL Función]
* [!UICONTROL Entrada de cuaderno]

   Puede crear informes sobre las actualizaciones del sistema rastreadas en la variable [!UICONTROL Actualizaciones] área de objetos como tareas, proyectos, problemas, etc. Para obtener más información, consulte [Informe sobre [!UICONTROL Actualizaciones] area](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

* [!UICONTROL Plantilla de diseño]
* [!UICONTROL Hito]
* [!UICONTROL Ruta de hitos]
* [!UICONTROL Nota]

   >[!NOTE]
   >
   >Puede informar sobre los comentarios agregados por usuarios individuales.

* [!UICONTROL Parámetro] (o [!UICONTROL Campo personalizado])
* [!UICONTROL Grupo de parámetros] (o [!UICONTROL Salto de sección])
* [!UICONTROL Perfil del portal] (muestra información en desuso)
* [!UICONTROL Portafolio]
* [!UICONTROL Programar]
* [!UICONTROL Proyecto] ([!UICONTROL Datos financieros])

   >[!NOTE]
   >
   >La información financiera se rellena en [!UICONTROL Proyecto] ([!UICONTROL Datos financieros]) solo aparece cuando los datos asociados tienen menos de 5 años. Por ejemplo, si una función de trabajo se asignó a una tarea en enero de 2015 y hoy es septiembre de 2021, un campo financiero como la [!UICONTROL Fecha de asignación] para la función de trabajo no se rellena en la variable [!UICONTROL Proyecto (datos financieros)] informe.

* [!UICONTROL Aprobación de revisión]\
   Permite ver información diversa sobre la aprobación de la prueba, como: la prueba que se presentó para su aprobación, la información sobre [!UICONTROL Aprobador], información sobre el solicitante (si el solicitante tiene licencia) [!DNL Workfront] usuario), información de versión, ID de prueba y fecha de creación de la prueba.\
   [!UICONTROL Aprobación de prueba] los informes solo incluyen pruebas disponibles en las áreas de Mi trabajo de los usuarios en las que aún no se han tomado decisiones.\
   Las aprobaciones de prueba se asignan en [!DNL Workfront] tal como se describe [Agregar usuarios a una prueba](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) en [Compartir una prueba en [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

* [!UICONTROL Cola]
* [!UICONTROL Tema de la cola]
* [!UICONTROL Rate] (muestra la función del trabajo) [!UICONTROL Tasa de facturación] información)
* [!UICONTROL Notificación de recordatorio]
* [!UICONTROL Informe]
* [!UICONTROL Conjunto de recursos]
* [!UICONTROL Riesgo]
* [!UICONTROL Tipo de riesgo]
* [!UICONTROL Horario]
* [!UICONTROL Tarjeta de puntuación]
* [!UICONTROL Equipo]
* [!UICONTROL Plantilla]
* [!UICONTROL Tarea de plantilla]
* [!UICONTROL Tiempo libre]

   Puede informar sobre el tiempo de espera de un usuario, tal como lo indica el usuario en su perfil.

* [!UICONTROL Hoja de horas]
* [!UICONTROL Perfil de hoja de horas]
* [!UICONTROL Grupo de temas]
* [!UICONTROL Delegación de usuario]

   Puede informar sobre los usuarios a los que se ha delegado para realizar las tareas y los problemas de otros mientras están fuera de la oficina. Este informe muestra el usuario que está fuera de la oficina, así como el usuario que cumple con sus obligaciones mientras está fuera.

* [!UICONTROL Vista]
* [!UICONTROL Elemento de trabajo] (se refiere a tareas y problemas)
