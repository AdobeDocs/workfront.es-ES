---
content-type: overview;reference
navigation-topic: workfront-navigation
title: "[!DNL Adobe Workfront] objetos información general"
description: '"La información que se muestra en  [!DNL Adobe Workfront]  está representada por objetos almacenados en la base de datos  [!DNL Workfront] s. Los objetos son los que generan la información en  [!DNL Workfront]. Obtenga más información acerca de estos objetos en este artículo".'
feature: Get Started with Workfront
author: Alina
exl-id: f324f198-5472-4cf2-a46e-7fc24605ca90
source-git-commit: 25939493f6ffed31ae1bdaf26d417ce4e5e5c004
workflow-type: tm+mt
source-wordcount: '2419'
ht-degree: 1%

---

# Resumen de objetos [!DNL Adobe Workfront]

<!--Audited: 12/2023-->

<!--
<***Linked to several articles, do not remove/ change. 
-->

La información que se muestra en [!DNL Adobe Workfront] está representada por objetos almacenados en la base de datos [!DNL Workfront]. Los objetos son los que generan la información en [!DNL Workfront].

Es importante comprender cómo se definen los objetos en [!DNL Workfront] para que pueda utilizar el objeto correcto para las necesidades necesarias en su organización.

Por ejemplo, cuando planea una gran cantidad de trabajo, necesita usar el objeto [!UICONTROL Project] para definir ese trabajo. Para dividir este trabajo en incrementos planificados más pequeños, puede usar el objeto [!UICONTROL Task]. Para una menor cantidad de trabajo que no está planificado y que puede producirse de forma inesperada, puede utilizar el objeto Issue. Si desea realizar un seguimiento del progreso y del cumplimiento del presupuesto y la cronología de un grupo de proyectos, puede organizarlos en [!UICONTROL Portfolio] y [!UICONTROL Programas]. Para definir otros elementos que le ayuden a resolver su trabajo, desea usar otros objetos que están almacenados en [!UICONTROL Proyectos], [!UICONTROL Tareas], [!UICONTROL Problemas] o [!UICONTROL Portfolio], como [!UICONTROL Documentos], [!UICONTROL Actualizaciones], [!UICONTROL Horas], [!UICONTROL Usuarios] o [!UICONTROL Roles].

[!UICONTROL Informes] y [!UICONTROL Paneles] son otro ejemplo de objetos que pueden ayudarle a organizar visualmente la cantidad de datos que tiene en [!DNL Workfront] para que todos los usuarios puedan obtener acceso a ellos fácilmente.

Para obtener una lista completa de los objetos de [!DNL Workfront], consulte el [Explorador de API](../../../wf-api/general/api-explorer.md).

## Interdependencia y jerarquía de objetos

Los objetos están vinculados entre sí en [!UICONTROL Workfront]. Por ejemplo, una tarea o un problema nunca pueden existir de forma independiente fuera de un proyecto. [!UICONTROL Tareas] y [!UICONTROL problemas] son ejemplos de objetos almacenados en el objeto [!UICONTROL proyecto]. [!UICONTROL Las tareas] y [!UICONTROL problemas] se consideran objetos secundarios de los proyectos.

A continuación se muestran algunos de los objetos más utilizados en [!DNL Workfront] y sus respectivos objetos primarios e secundarios:

| **Objeto** | **Objetos principales** | **Objetos secundarios** |
|---|---|---|
| [!UICONTROL Portafolios] |  | [!UICONTROL Programas], [!UICONTROL Proyectos], [!UICONTROL Documentos], [!DNL Notes], [!UICONTROL Usuarios] |
| [!UICONTROL Programas] | [!UICONTROL Portafolios] | [!UICONTROL Proyectos], [!UICONTROL Documentos], [!UICONTROL Notas], [!UICONTROL Usuarios] |
| [!UICONTROL Proyectos] | [!UICONTROL Portfolio], [!UICONTROL Programas] | [!UICONTROL Tareas], [!UICONTROL Problemas], [!UICONTROL Documentos], [!UICONTROL Notas], [!UICONTROL Horas], [!UICONTROL Usuarios] |
| [!UICONTROL Tareas] | [!UICONTROL Proyectos] | [!UICONTROL Problemas], [!UICONTROL Tareas secundarias], [!UICONTROL Documentos], [!UICONTROL Notas], [!UICONTROL Horas], [!UICONTROL Usuarios] |
| [!UICONTROL Problemas] | [!UICONTROL Tareas], [!UICONTROL Proyectos] | [!UICONTROL Documentos], [!UICONTROL Notas], [!UICONTROL Horas], [!UICONTROL Usuarios] |
| [!UICONTROL Paneles] |  | [!UICONTROL Informes], páginas externas |
| [!UICONTROL Informes] | [!UICONTROL Paneles] |  |
| [!UICONTROL Grupos] |  | [!UICONTROL Usuarios] |
| [!UICONTROL Equipos] |  | [!UICONTROL Usuarios] |
| [!UICONTROL Usuarios] | [!UICONTROL Grupos], [!UICONTROL Equipos], [!UICONTROL Compañías] | [!UICONTROL Roles] |
| [!UICONTROL Compañías] |  | [!UICONTROL Usuarios] |
| [!UICONTROL Documentos] | [!UICONTROL Tareas], [!UICONTROL Problemas], [!UICONTROL Proyectos], [!UICONTROL Portfolio], [!UICONTROL Programas], [!UICONTROL Usuarios] |  |
| [!UICONTROL Planes]* |  | [!UICONTROL Iniciativas] |
| [!DNL Goals]* |  | [!UICONTROL Resultados], [!UICONTROL Actividades] |

Para obtener una lista completa de los objetos de [!DNL Workfront], consulte el [Explorador de API](../../../wf-api/general/api-explorer.md).

*Los planes son los objetos de [!DNL Adobe Workfront Scenario Planner]. Para obtener información sobre [!DNL Scenario Planner], consulte [Información general sobre el [!UICONTROL Planificador de escenarios]](../../../scenario-planner/scenario-planner-overview.md).

*[!UICONTROL Las metas] son los objetos de [!DNL Adobe Workfront Goals]. Para obtener información acerca de [!DNL Workfront Goals], vea [[!DNL Adobe Workfront Goals] descripción general](../../../workfront-goals/goal-management/wf-goals-overview.md).


## Personalizar nombres de objetos

Como administrador de [!DNL Workfront], puede personalizar los nombres de objetos en [!DNL Workfront] mediante una [!UICONTROL plantilla de diseño].

Para obtener más información acerca de cómo personalizar nombres de objetos mediante una [!UICONTROL plantilla de diseño], vea [Crear y administrar plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Después de personalizar una plantilla de diseño y asignarla a los usuarios, estos verán los nombres personalizados de los objetos. Los usuarios asignados a la plantilla de diseño ya no ven los nombres predeterminados para los objetos en ninguna parte de la aplicación web.

Por ejemplo, si la mayor cantidad de trabajo en su organización se conoce como &quot;Participación&quot;, puede reemplazar el nombre &#39;[!UICONTROL Proyecto]&#39; por &quot;Participación&quot;. La interfaz de [!DNL Workfront] muestra &#39;Participación&#39; en lugar de &#39;[!UICONTROL Proyecto]&#39; en todas partes donde aparecería el nombre &#39;[!UICONTROL Proyecto]&#39;.

>[!NOTE]
>
>Para que los usuarios puedan ver los nuevos nombres de los objetos, deben cerrar la sesión y volver a iniciarla en [!DNL Workfront] después de guardar [!UICONTROL la plantilla de diseño].

>[!IMPORTANT]
>
>La documentación [!DNL Workfront] siempre hace referencia a los nombres predeterminados de los objetos. Como administrador de [!DNL Workfront], asegúrese de notificar a los usuarios los cambios en los nombres de los objetos para que puedan comprender cómo usar la documentación de [!DNL Workfront], así como las áreas de las aplicaciones que no reflejan los cambios en los nombres de los objetos.

* [Nombres de objeto que se pueden personalizar mediante una [!UICONTROL plantilla de diseño]](#object-names-that-can-be-customized-using-a-layout-template)
* [Áreas de  [!DNL Workfront]  que reflejan los nombres de objeto personalizados](#areas-of-workfront-that-reflect-the-customized-object-names)
* [Áreas de  [!DNL Workfront]  que no reflejan los nombres de objeto personalizados](#areas-of-workfront-that-do-not-reflect-the-customized-object-names)

### Nombres de objeto que se pueden personalizar mediante una [!UICONTROL plantilla de diseño]

Como administrador de [!DNL Workfront], puede personalizar los nombres de los siguientes objetos para que coincidan con la terminología de su organización:

* [!UICONTROL Portfolio]
* [!UICONTROL Programa]
* [!UICONTROL Proyecto]
* [!UICONTROL Tarea]
* [!UICONTROL Problema]
* [!UICONTROL Objetivo]*
* [!UICONTROL Resultado]*
* [!UICONTROL Actividad]*

  *[!UICONTROL Las metas], [!UICONTROL resultados] y [!UICONTROL actividades] solo están disponibles si su compañía compró [!DNL Workfront Goals]. Para obtener información acerca de [!DNL Workfront Goals], vea [[!DNL Adobe Workfront Goals] descripción general](../../../workfront-goals/goal-management/wf-goals-overview.md).

* [!UICONTROL Iniciativa]**
* [!UICONTROL Escenario]**
* [!UICONTROL Plan]**

  **[!UICONTROL Iniciativas], [!UICONTROL escenarios] y [!UICONTROL planes] solo están disponibles si su compañía compró [!DNL Workfront Scenario Planner]. Para obtener información acerca de [!DNL Scenario Planner], vea [Introducción a  [!DNL Scenario Planner]](../../../scenario-planner/get-started-with-scenario-planning.md).



Para obtener más información acerca de cómo personalizar los nombres de objetos mediante [!UICONTROL Plantillas de diseño], vea [Crear y administrar plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

No se pueden personalizar los nombres de ningún otro objeto en Workfront. Para obtener una lista completa de los objetos de [!DNL Workfront], consulte el [Explorador de API](../../../wf-api/general/api-explorer.md).

Al personalizar el nombre de un objeto, el nuevo nombre de ese objeto aparece en la mayoría de las áreas de la aplicación [!DNL Workfront] en las que aparecería ese nombre de objeto.

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

* Complemento [!DNL Outlook]

### Implicaciones de la personalización de nombres de objetos

Debe tener en cuenta lo siguiente al personalizar los nombres de objeto en [!DNL Workfront]:

* Puede encontrar errores estilísticos o gramaticales en las pantallas del sistema. Por ejemplo, si cambia el nombre de &#39;[!UICONTROL Issue]&#39; a &#39;Request&#39; y ve en cualquier parte del sistema la frase &#39;An request&#39;, esto está funcionando según lo previsto y no debería considerarse un error.
* Los nombres personalizados de los objetos no se pueden traducir. Solo los nombres predeterminados de [!DNL Workfront] se pueden traducir a los idiomas compatibles. Para obtener más información acerca de los idiomas compatibles con [!DNL Workfront], vea [Idiomas compatibles en [!DNL Adobe Workfront]](../../../workfront-basics/supported-languages-in-workfront.md). Los campos de nombre de objeto personalizado admiten caracteres extranjeros para que pueda introducir la terminología en cualquier idioma.
* Cuando personalice los nombres de los objetos mediante una [!UICONTROL plantilla de diseño], le recomendamos que asigne las [!UICONTROL plantillas de diseño] en función de sus unidades de negocio (equipos o grupos).\
   Le recomendamos que utilice nombres que los usuarios de estas unidades de negocio entiendan claramente, para evitar confusiones.
* Las notificaciones por correo electrónico y los informes enviados siempre contienen nombres de objeto tal como se definen en la [!UICONTROL Plantilla de diseño] del usuario que genera el correo electrónico. Los usuarios deben estar preparados para ver nombres de objetos en sus correos electrónicos que no estén relacionados con su grupo o equipo si reciben notificaciones por correo electrónico de usuarios de otros equipos y grupos.\
   Como administrador de [!DNL Workfront], indique a los usuarios que observen los iconos asociados a cada objeto. Los iconos permanecen coherentes entre los distintos nombres de objeto y con el objeto predeterminado, tal como aparece en la base de datos. Para obtener una lista de todos los [!DNL Workfront] iconos asociados con objetos, consulte [Iconos de objetos](#object-icons).

  >[!TIP]
  >
  >Para tareas comunes en su organización, considere la posibilidad de crear documentación personalizada que refleje su terminología.

## Iconos de objeto

La documentación [!DNL Workfront] siempre hace referencia a los nombres predeterminados de los objetos. Si los objetos tienen sus nombres personalizados, puede confiar en el icono asociado a ellos para comprender qué objeto personalizado corresponde a qué objeto predeterminado de [!DNL Workfront].

Para obtener más información sobre qué objetos pueden tener nombres personalizados en [!DNL Workfront], vea [Nombres de objeto que se pueden personalizar mediante una [!UICONTROL plantilla de diseño]](#object-names-that-can-be-customized-using-a-layout-template).

A continuación se muestra una lista de objetos y sus iconos correspondientes en Workfront.

| **Objeto** | **Icono** | **Nombre de objeto personalizable** |
|---|---|---|
| [!UICONTROL Empresa] | ![](assets/company-icon-nwe.png), ![](assets/nwe-company-icon-54x54.png) |  |
| [!UICONTROL Tablero] | ![](assets/dashboard-icon-nwe.png), ![](assets/nwe-dashboards-icon.png) |  |
| [!UICONTROL Meta] | ![](assets/nwe-goal-icon.png) | ✔ |
| [!UICONTROL Grupo] | ![](assets/groups-icon-nwe.png), ![](assets/nwe-group-icon.png) |  |
| [!UICONTROL Problema] | ![](assets/issue-icon-nwe.png), ![](assets/nwe-issues-icon.png) | ✔ |
| [!UICONTROL Rol] | ![job_role_icon.png](assets/job-role-icon-52x50.png), ![job_role_icon__1_.png](assets/job-role-icon--1--53x44.png), ![](assets/job-role-nwe-no-color.png), ![](assets/job-role-icon-nwe-color.png) |  |
| [!UICONTROL Plan] | ![](assets/plan-icon.png), ![](assets/nwe-plan-icon-60x57.png) |  |
| [!UICONTROL Portfolio] | ![](assets/portfolio-icon-nwe.png), ![](assets/nwe-portfolios-icon.png) | ✔ |
| [!UICONTROL Programa] | ![](assets/program-icon-nwe.png), ![](assets/nwe-programs-icon.png) | ✔ |
| [!UICONTROL Proyecto] | ![](assets/project-icon-nwe.png), ![](assets/nwe-projects-icon.png) | ✔ |
| [!UICONTROL Informe] | ![](assets/report-icon-nwe.png), ![](assets/nwe-reports-icon.png) |  |
| [!UICONTROL Tarea] | ![](assets/task-icon-new.png), ![](assets/nwe-tasks-icon.png) | ✔ |
| [!UICONTROL Equipo] | ![](assets/team-icon-nwe.png), ![](assets/team-icon-nwe-color.png), ![](assets/nwe-teams-icon.png) |  |
| [!UICONTROL Plantilla] | ![](assets/template-icon-nwe.png), ![](assets/nwe-templates-icon.png) |  |
| [!UICONTROL Usuario] | ![](assets/users-icon-gray.png) , ![](assets/user-icon-blue.png) , ![](assets/user-icon-initials.png) , ![](assets/user-avatar.png) , ![](assets/user-main-menu-area.png) |  |

## Números de referencia de objetos

A cada objeto creado en [!DNL Workfront] se le asigna un número de referencia único. Los números de referencia son útiles para distinguir entre dos objetos similares (como tareas con el mismo nombre). Se pueden buscar objetos utilizando sus números de referencia y se pueden incluir números de referencia en los informes.

Para obtener información acerca de cómo buscar objetos por número de referencia, vea [Usar el número de referencia de objetos](../../../workfront-basics/navigate-workfront/search/reference-number-of-objects.md).

## Búsquedas específicas de objetos

Puede buscar en todos los objetos que se pueden buscar en [!DNL Workfront], o bien puede seleccionar un objeto específico para buscarlo en las búsquedas básicas y avanzadas.

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
| [!UICONTROL Notas] (o [!UICONTROL Actualizaciones]) | ✓ |  |

Para obtener más información acerca de cómo ejecutar búsquedas básicas y avanzadas en [!DNL Workfront], vea [Buscar [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md).


## Acceso restringido a objetos

Cuando un usuario no tiene acceso a un objeto, ve &quot;Sin acceso&quot; en cualquier lugar donde se muestra el nombre de ese objeto en Workfront.

El acceso a los objetos se puede restringir en el nivel de acceso o en los permisos de un objeto específico.

Esto se aplica a todos los objetos y objetos secundarios enumerados en la sección [Interdependencia y jerarquía de objetos](#interdependency-and-hierarchy-of-objects) de este artículo. Esto no se aplica a los objetos Equipo y Usuario.

## Informar sobre objetos

Es extremadamente importante comprender la jerarquía y la interdependencia de los objetos antes de empezar a crear informes en [!DNL Workfront]. Los informes son específicos de objetos. Debe seleccionar el objeto correcto para el informe antes de poder mostrar los datos deseados.

>[!IMPORTANT]
>
>Sólo puede crear informes sobre el objeto seleccionado y los objetos principales en el mismo informe. No se puede tener información sobre los objetos secundarios en un informe de objeto principal. Por ejemplo, se puede mostrar la información del proyecto en un informe de tareas, pero no la información de tareas en un informe de proyecto.

Puede crear informes sobre todos los objetos de la base de datos utilizando nuestra API abierta. Para obtener una lista completa de todos los objetos de la base de datos, consulte [Explorador de API](../../../wf-api/general/api-explorer.md).

>[!NOTE]
>
> * Si ha personalizado los nombres de los objetos mediante una plantilla de diseño, también se han personalizado los nombres de los objetos en Report Builder. Asegúrese de saber qué objetos se han personalizado y de buscar el nombre personalizado en Report Builder. Para obtener más información sobre qué objetos pueden tener nombres personalizados en [!DNL Workfront], vea [Nombres de objeto que se pueden personalizar con una [!UICONTROL plantilla de diseño]](#object-names-that-can-be-customized-using-a-layout-template) en este artículo.
> * Al utilizar el modo de texto en los informes, los nombres de los objetos en las expresiones del modo de texto son los nombres estándar de [!DNL Workfront], y no los nombres de objeto personalizados. Para obtener más información acerca del uso del modo de texto en los informes, vea [Información general sobre el modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Para obtener más información sobre cómo generar un informe, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
Para obtener más información sobre nuestra API, consulte [Explorador de API](../../../wf-api/general/api-explorer.md).

### Objetos disponibles para informes

Puede crear informes sobre los objetos siguientes al usar Report Builder en la aplicación web [!DNL Workfront]. Los puntos de viñeta con sangría proporcionan más información sobre el objeto y no representan objetos adicionales.

* [!UICONTROL Proyecto]
* [!UICONTROL Tarea]
* [!UICONTROL Hora]
* [!UICONTROL Problema]
* [!UICONTROL Usuario]
* [!UICONTROL Nivel de acceso]
* [!UICONTROL Aprobación]
* [!UICONTROL Proceso de aprobación]
* [!UICONTROL Asignación]
* [!UICONTROL Línea base]
* [!UICONTROL Tarea de línea base]
* [!UICONTROL Registro de facturación]
* [!UICONTROL Hora presupuestada]
   * Son las [!UICONTROL horas presupuestadas], tal como aparecen en las herramientas de administración de recursos obsoletas más antiguas.
   * El &quot;Bud&quot;. El campo &quot;Horas&quot; en el informe [!UICONTROL Horas presupuestadas] hace referencia a las horas presupuestadas para los roles del puesto en [!UICONTROL Planificador de recursos]. Para obtener más información, vea [Comprender [!UICONTROL Costo de mano de obra presupuestado] y [!UICONTROL Horas presupuestadas] para proyectos](../../../manage-work/projects/project-finances/budgeted-labor-cost.md).

* [!UICONTROL Evento de calendario]
* [!UICONTROL Empresa]
* [!UICONTROL Formulario personalizado]
* [!UICONTROL Tablero]
* [!UICONTROL Documento]
* [!UICONTROL Aprobación de documento]
* [!UICONTROL Versión del documento]
   * Puede ver información sobre la versión del documento, el documento con el que está asociada la versión, quién creó la versión y el usuario que creó la prueba en la versión del documento, si existe (Creador de pruebas).
* [!UICONTROL Plantilla de correo electrónico]
* [!UICONTROL Gasto]
* [!UICONTROL Tipo de gasto]
* [!UICONTROL Página externa]
* [!UICONTROL Favorito]
* [!UICONTROL Filtro]
* [!UICONTROL Meta]
   * Puede generar un informe para metas estratégicas o mostrar información relacionada con las metas en un informe de proyecto cuando los proyectos están asociados con metas como actividades de metas. Puede crear metas estratégicas y conectar proyectos con ellas solo si su organización ha adquirido una licencia de [!DNL Workfront Goals]. Para obtener información acerca de [!DNL Workfront Goals], vea [[!DNL Workfront Goals] descripción general](../../../workfront-goals/goal-management/wf-goals-overview.md). Para obtener información acerca de cómo conectar proyectos con metas estratégicas, vea [Agregar proyectos a metas en Adobe Workfront Goals](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).
*No puede informar sobre metas de proyecto que estén asociadas con [!UICONTROL Caso comercial]. Para obtener información sobre los objetivos del proyecto frente a los objetivos estratégicos, consulte [Glosario de [!DNL Adobe Workfront] terminología](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* [!UICONTROL Grupo]
* [!UICONTROL Agrupación]
* [!UICONTROL Tipo de hora]
* [!UICONTROL Iniciativa]
   * Puede generar un informe para las iniciativas que son los objetos secundarios de un plan solo si su compañía ha adquirido una licencia de [!DNL Workfront Scenario Planner]. Para obtener información acerca de las iniciativas, consulte [Información general sobre iniciativas en [!DNL Workfront Scenario Planner]](../../../scenario-planner/initiatives-overview.md).

* Función del puesto de la iniciativa
   * Puede generar un informe para los roles asociados con las iniciativas de un plan solo si su compañía ha adquirido una licencia de [!DNL Workfront Scenario Planner]. Para obtener información acerca de cómo crear iniciativas y asociarlas con roles, consulte [Crear y editar iniciativas en [!DNL Workfront Scenario Planner]](../../../scenario-planner/create-and-edit-initiatives.md).

* [!UICONTROL Iteración]
* [!UICONTROL Rol]
* [!UICONTROL Entrada de diario]
   * Puede informar sobre las actualizaciones del sistema rastreadas en el área de [!UICONTROL Actualizaciones] de objetos como tareas, proyectos, problemas, etc. Para obtener más información, consulte [Informe sobre el área de [!UICONTROL Actualizaciones]](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

* [!UICONTROL Plantilla de diseño]
* [!UICONTROL Hito]
* [!UICONTROL Ruta de hitos]
* [!UICONTROL Nota] o [!UICONTROL Actualizaciones]
   * Puede informar sobre los comentarios agregados por usuarios individuales.

* [!UICONTROL Parámetro] (o [!UICONTROL Campo personalizado])
* [!UICONTROL Grupo de parámetros] (o [!UICONTROL Salto de sección])
* [!UICONTROL Portfolio]
* [!UICONTROL Programa]
* [!UICONTROL Proyecto (datos financieros)]
   * La información financiera se rellena en [!UICONTROL Proyecto (datos financieros)] informes solamente cuando los datos asociados con ella tienen menos de 5 años. Por ejemplo, si se asignó un rol a una tarea en enero de 2015 y hoy es septiembre de 2021, un campo financiero como [!UICONTROL Fecha de asignación] para el rol no se rellena en el informe [!UICONTROL Proyecto (datos financieros)].

  >[!CAUTION]
  >
  >La ejecución de un informe de proyecto (datos financieros) realiza un nuevo cálculo de los datos financieros, que puede sobrescribir los datos financieros anteriores y puede tardar bastante tiempo. Para obtener más información sobre las consecuencias del cálculo de datos financieros, vea [Recalcular finanzas de proyectos](/help/quicksilver/manage-work/projects/project-finances/recalculate-project-finances.md).

* [!UICONTROL Aprobación de revisión]
   * Permite ver información diversa sobre la aprobación de pruebas, que incluye: la prueba que se envió para su aprobación, información sobre el [!UICONTROL aprobador], información sobre el solicitante (si el solicitante es un usuario con licencia [!DNL Workfront]), información de la versión, el ID de prueba y la fecha de creación de la prueba.\
      Los informes de [!UICONTROL Aprobación de pruebas] solo incluyen pruebas disponibles en las áreas de Mi trabajo de los usuarios en las que aún no se han tomado decisiones.\
   * Se han asignado aprobaciones de revisión en [!DNL Workfront] tal como se describe [Agregue usuarios a una revisión](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) en [Comparta una revisión en [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

* [!UICONTROL Cola]
* [!UICONTROL Tema de cola]
* [!UICONTROL Tarifa] (esto muestra la información de la función [!UICONTROL Tarifa de facturación])
* [!UICONTROL Notificación de recordatorio]
* [!UICONTROL Informe]
* [!UICONTROL Conjunto de recursos]
* [!UICONTROL Riesgo]
* [!UICONTROL Tipo de riesgo]
* [!UICONTROL Programación]
* [!UICONTROL informe de valoración]
* [!UICONTROL Equipo]
* [!UICONTROL Plantilla]
* [!UICONTROL Tarea de plantilla]
* [!UICONTROL Tiempo libre]
   * Puede crear informes sobre el tiempo libre de un usuario, tal como lo indique el usuario en su perfil.

* [!UICONTROL Hoja de horas]
* [!UICONTROL Perfil de hoja de horas]
* [!UICONTROL Grupo de temas]
* [!UICONTROL Aprobación de usuario]
* [!UICONTROL Delegación de usuario]

   * Puede informar sobre los usuarios que se han delegado para realizar las tareas y los problemas de otros mientras están fuera de la oficina. Este informe muestra el usuario que está fuera de la oficina, así como el usuario que cumple con sus obligaciones mientras está fuera.

* [!UICONTROL Decisiones de usuarios]

   * Puede crear informes sobre cuántas decisiones han tomado los usuarios en las pruebas y los documentos en el mes actual.

* [!UICONTROL Vista]
* [!UICONTROL Elemento de trabajo] (esto genera un informe para las tareas y los problemas)
