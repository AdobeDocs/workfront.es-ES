---
content-type: overview;reference
navigation-topic: workfront-navigation
title: Información general sobre los objetos de [!DNL Adobe Workfront]
description: La información que se muestra en  [!DNL Adobe Workfront]  está representada por objetos que se almacenan en la base de datos  [!DNL Workfront] . Los objetos son los que generan la información en  [!DNL Workfront]. Obtenga más información acerca de estos objetos en este artículo.
feature: Get Started with Workfront
author: Alina
exl-id: f324f198-5472-4cf2-a46e-7fc24605ca90
source-git-commit: 0a2ff1ab802b2bd08cd680376321552a8018cb74
workflow-type: tm+mt
source-wordcount: '2508'
ht-degree: 95%

---

# Información general sobre los objetos de [!DNL Adobe Workfront]

<!--Audited: 12/2023-->

<!--
<***Linked to several articles, do not remove/ change. 
-->

La información que se muestra en [!DNL Adobe Workfront] está representada por objetos almacenados en la base de datos [!DNL Workfront]. Los objetos son los que generan la información en [!DNL Workfront].

Es importante comprender cómo se definen los objetos en [!DNL Workfront] para que pueda utilizar el objeto correcto para las necesidades de su organización.

Por ejemplo, cuando se planea una gran cantidad de trabajo, es necesario usar el objeto [!UICONTROL Project] para definir ese trabajo. Para dividir este trabajo en incrementos planificados más pequeños, puede utilizarse el objeto [!UICONTROL Task]. Para una menor cantidad de trabajo que no está planificado y que puede ocurrir de forma inesperada, puede utilizar el objeto Issue. Si desea realizar un seguimiento del progreso y del cumplimiento del presupuesto y la línea de tiempo de un grupo de proyectos, puede organizarlos en [!UICONTROL Portafolios] y [!UICONTROL Programas]. Para definir otros elementos que le ayuden a resolver su trabajo, es conveniente utilizar otros objetos que están almacenados en [!UICONTROL Proyectos], [!UICONTROL Tareas], [!UICONTROL Problemas] o [!UICONTROL Portafolios], como [!UICONTROL Documentos], [!UICONTROL Actualizaciones], [!UICONTROL Horas], [!UICONTROL Usuarios] o [!UICONTROL Funciones].

[!UICONTROL Informes] y [!UICONTROL Paneles] son otro ejemplo de objetos que pueden ayudarle a organizar visualmente la cantidad de datos incluidos en [!DNL Workfront] para que todos los usuarios puedan obtener acceso a ellos fácilmente.

Para obtener una lista completa de los objetos de [!DNL Workfront], consulte el [Explorador de API](../../../wf-api/general/api-explorer.md).

## Interdependencia y jerarquía de objetos

Los objetos están vinculados entre sí en [!UICONTROL Workfront]. Por ejemplo, una tarea o un problema nunca pueden existir de forma independiente fuera de un proyecto. [!UICONTROL Tareas] y [!UICONTROL problemas] son ejemplos de objetos almacenados en el objeto [!UICONTROL proyecto]. [!UICONTROL Las tareas] y los [!UICONTROL problemas] se consideran objetos secundarios de los proyectos.

A continuación se muestran algunos de los objetos más utilizados en [!DNL Workfront] y sus respectivos objetos primarios y secundarios:

| **Objeto** | **Objetos principales** | **Objetos secundarios** |
|---|---|---|
| [!UICONTROL Portafolios] |  | [!UICONTROL Programas], [!UICONTROL Proyectos], [!UICONTROL Documentos], [!DNL Notes], [!UICONTROL Usuarios] |
| [!UICONTROL Programas] | [!UICONTROL Portafolios] | [!UICONTROL Proyectos], [!UICONTROL Documentos], [!UICONTROL Notas], [!UICONTROL Usuarios] |
| [!UICONTROL Proyectos] | [!UICONTROL Portafolios], [!UICONTROL Programas] | [!UICONTROL Tareas], [!UICONTROL Problemas], [!UICONTROL Documentos], [!UICONTROL Notas], [!UICONTROL Horas], [!UICONTROL Usuarios] |
| [!UICONTROL Tareas] | [!UICONTROL Proyectos] | [!UICONTROL Problemas], [!UICONTROL Tareas secundarias], [!UICONTROL Documentos], [!UICONTROL Notas], [!UICONTROL Horas], [!UICONTROL Usuarios] |
| [!UICONTROL Problemas] | [!UICONTROL Tareas], [!UICONTROL Proyectos] | [!UICONTROL Documentos], [!UICONTROL Notas], [!UICONTROL Horas], [!UICONTROL Usuarios] |
| [!UICONTROL Paneles] |  | [!UICONTROL Informes], páginas externas |
| [!UICONTROL Informes] | [!UICONTROL Paneles] |  |
| [!UICONTROL Grupos] |  | [!UICONTROL Usuarios] |
| [!UICONTROL Equipos] |  | [!UICONTROL Usuarios] |
| [!UICONTROL Usuarios] | [!UICONTROL Grupos], [!UICONTROL Equipos], [!UICONTROL Compañías] | [!UICONTROL Funciones] |
| [!UICONTROL Empresas] |  | [!UICONTROL Usuarios] |
| [!UICONTROL Documentos] | [!UICONTROL Tareas], [!UICONTROL Problemas], [!UICONTROL Proyectos], [!UICONTROL Portafolios], [!UICONTROL Programas], [!UICONTROL Usuarios] |  |
| [!UICONTROL Planes]* |  | [!UICONTROL Iniciativas] |
| [!DNL Goals]* |  | [!UICONTROL Resultados], [!UICONTROL Actividades] |

Para obtener una lista completa de los objetos de [!DNL Workfront], consulte el [Explorador de la API](../../../wf-api/general/api-explorer.md).

*Los planes son los objetos del [!DNL Adobe Workfront Scenario Planner]. Para obtener información sobre [!DNL Scenario Planner], consulte [Información general sobre el [!UICONTROL Planificador de escenarios]](../../../scenario-planner/scenario-planner-overview.md).

*[!UICONTROL Las metas] son los objetos de [!DNL Adobe Workfront Goals]. Para obtener información acerca de [!DNL Workfront Goals], consulte la [[!DNL Adobe Workfront Goals] información general](../../../workfront-goals/goal-management/wf-goals-overview.md).


## Personalizar los nombres de los objetos

Como administrador de [!DNL Workfront], puede personalizar los nombres de objetos en [!DNL Workfront] mediante una [!UICONTROL plantilla de diseño].

Para obtener más información acerca de cómo personalizar nombres de objetos mediante una [!UICONTROL plantilla de diseño], consulte [Crear y administrar plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Después de personalizar una plantilla de diseño y asignarla a los usuarios, estos verán los nombres personalizados de los objetos. Los usuarios asignados a la plantilla de diseño ya no ven los nombres predeterminados para los objetos en ninguna sección de la aplicación web.

Por ejemplo, si la mayor cantidad de trabajo en su organización se conoce como “Participación”, puede reemplazar el nombre “[!UICONTROL Proyecto]” por “Participación”. La interfaz de [!DNL Workfront] muestra “Participación” en lugar de “[!UICONTROL Proyecto]” en todas las partes donde aparecería el nombre “[!UICONTROL Proyecto]”.

>[!NOTE]
>
>Para que los usuarios puedan ver los nuevos nombres de los objetos, deben cerrar la sesión y volver a iniciarla en [!DNL Workfront] después de guardar la [!UICONTROL plantilla de diseño].

>[!IMPORTANT]
>
>La documentación de [!DNL Workfront] siempre hace referencia a los nombres predeterminados de los objetos. Como administrador de [!DNL Workfront], asegúrese de notificar a los usuarios los cambios en los nombres de los objetos para que puedan comprender cómo usar la documentación de [!DNL Workfront], así como las áreas de las aplicaciones que no reflejan los cambios en los nombres de los objetos.

* [Nombres de objeto que se pueden personalizar mediante una [!UICONTROL plantilla de diseño]](#object-names-that-can-be-customized-using-a-layout-template)
* [Áreas de  [!DNL Workfront]  que reflejan los nombres de objeto personalizados](#areas-of-workfront-that-reflect-the-customized-object-names)
* [Áreas de  [!DNL Workfront]  que no reflejan los nombres de objeto personalizados](#areas-of-workfront-that-do-not-reflect-the-customized-object-names)

### Nombres de objeto que se pueden personalizar mediante una [!UICONTROL plantilla de diseño]

Como administrador de [!DNL Workfront], puede personalizar los nombres de los siguientes objetos para que coincidan con la terminología de su organización:

* [!UICONTROL Portafolios]
* [!UICONTROL Programa]
* [!UICONTROL Proyecto]
* [!UICONTROL Tarea]
* [!UICONTROL Problema]
* [!UICONTROL Meta]*
* [!UICONTROL Resultado]*
* [!UICONTROL Actividad]*

  *[!UICONTROL Las metas], [!UICONTROL resultados] y [!UICONTROL actividades] solo están disponibles si su compañía adquirió [!DNL Workfront Goals]. Para obtener información acerca de [!DNL Workfront Goals], consulte la [[!DNL Adobe Workfront Goals] información general](../../../workfront-goals/goal-management/wf-goals-overview.md).

* [!UICONTROL Iniciativa]**
* [!UICONTROL Escenario]**
* [!UICONTROL Plan]**

  **Las [!UICONTROL iniciativas], [!UICONTROL escenarios] y [!UICONTROL planes] solo están disponibles si su compañía compró [!DNL Workfront Scenario Planner]. Para obtener información acerca de [!DNL Scenario Planner], consulte [Introducción a  [!DNL Scenario Planner]](../../../scenario-planner/get-started-with-scenario-planning.md).



Para obtener más información acerca de cómo personalizar los nombres de objetos mediante [!UICONTROL Plantillas de diseño], consulte [Crear y administrar plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

No se pueden personalizar los nombres de ningún otro objeto en Workfront. Para obtener una lista completa de los objetos de [!DNL Workfront], consulte el [explorador de API](../../../wf-api/general/api-explorer.md).

Al personalizar el nombre de un objeto, el nuevo nombre de ese objeto aparece en la mayoría de las áreas de la aplicación [!DNL Workfront] en las que aparecería ese nombre de objeto.

### Áreas de [!DNL Workfront] que reflejan los nombres de objeto personalizados

Las áreas siguientes muestran el nombre actualizado de los objetos:

* Navegación superior
* Todas las secciones de la navegación del panel izquierdo
* Todos los menús
* Notificaciones en la aplicación
* Generador de informes y elementos de creación de informes (vistas, filtros y agrupaciones)
* Botones [!UICONTROL Guardar] 
* Archivos exportados
* Correos electrónicos
* Aplicaciones móviles

### Áreas de [!DNL Workfront] que no reflejan los nombres de objeto personalizados

Las áreas siguientes no muestran el nombre actualizado de los objetos:

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Referenced Object Type selection for a Typeahead field in a Custom Form </p> <p>(NOTE: drafting this because I don't think this is true)</p> </li>
  -->

* Complemento de [!DNL Outlook]

### Implicaciones de la personalización de los nombres de los objetos

Debe tener en cuenta lo siguiente al personalizar los nombres de los objetos en [!DNL Workfront]:

* Puede encontrar errores estilísticos o gramaticales en las pantallas del sistema. Por ejemplo, si cambia el nombre de “[!UICONTROL Issue]” a “Request” y observa en cualquier parte del sistema la frase “An request”, esto está funcionando según lo previsto y no debería considerarse un error.
* Los nombres personalizados de los objetos no se pueden traducir. Solo los nombres predeterminados de [!DNL Workfront] se pueden traducir a los idiomas compatibles. Para obtener más información acerca de los idiomas compatibles con [!DNL Workfront], consulte [Idiomas compatibles en [!DNL Adobe Workfront]](../../../workfront-basics/supported-languages-in-workfront.md). Los campos de nombre de objeto personalizado admiten caracteres extranjeros para que pueda introducir la terminología en cualquier idioma.
* Cuando personalice los nombres de los objetos mediante una [!UICONTROL plantilla de diseño], le recomendamos que asigne las [!UICONTROL plantillas de diseño] en función de sus unidades de negocio (equipos o grupos).\
   Le recomendamos que utilice nombres que los usuarios de estas unidades de negocio entiendan claramente, para evitar confusiones.
* Las notificaciones por correo electrónico y los informes enviados siempre contienen nombres de objeto tal como se definen en la [!UICONTROL Plantilla de diseño] del usuario que genera el correo electrónico. Los usuarios deben estar preparados para ver nombres de objetos en sus correos electrónicos que no estén relacionados con su grupo o equipo si reciben notificaciones por correo electrónico de usuarios de otros equipos y grupos.\
   Como administrador de [!DNL Workfront], indique a los usuarios que observen los iconos asociados a cada objeto. Los iconos permanecen coherentes entre los distintos nombres de objeto y con el objeto predeterminado, tal como aparece en la base de datos. Para obtener una lista de todos los iconos de [!DNL Workfront] asociados con objetos, consulte [Iconos de objetos](#object-icons).

  >[!TIP]
  >
  >Para tareas comunes en su organización, considere la posibilidad de crear documentación personalizada que refleje su terminología.

## Iconos de objeto

La documentación [!DNL Workfront] siempre hace referencia a los nombres predeterminados de los objetos. Si sus objetos tienen nombres personalizados, puede confiar en el icono que tienen asociado para comprender qué objeto personalizado corresponde a qué objeto predeterminado de [!DNL Workfront].

Para obtener más información sobre qué objetos pueden tener nombres personalizados en [!DNL Workfront], consulte [Nombres de objeto que se pueden personalizar mediante una [!UICONTROL plantilla de diseño]](#object-names-that-can-be-customized-using-a-layout-template).

A continuación se muestra una lista de objetos y sus iconos correspondientes en Workfront.

| **Objeto** | **Icono** | **Nombre de objeto personalizable** |
|---|---|---|
| [!UICONTROL Compañía] | ![Icono de la compañía](assets/company-icon-nwe.png), ![icono de la compañía azul](assets/nwe-company-icon-54x54.png) |  |
| [!UICONTROL Panel] | ![Icono de panel](assets/dashboard-icon-nwe.png), ![icono de panel azul](assets/nwe-dashboards-icon.png) |  |
| [!UICONTROL Meta] | ![Icono de meta](assets/nwe-goal-icon.png) | ✔ |
| [!UICONTROL Grupo] | ![Icono de grupos](assets/groups-icon-nwe.png) , ![Icono de grupos](assets/nwe-group-icon.png) |  |
| [!UICONTROL Problema] | ![Icono de problema](assets/issue-icon-nwe.png) , ![Icono de problema rosa](assets/nwe-issues-icon.png) | ✔ |
| [!UICONTROL Función] | ![job_role_icon.png](assets/job-role-icon-52x50.png), ![job_role_icon__1_.png](assets/job-role-icon--1--53x44.png), ![icono de rol](assets/job-role-nwe-no-color.png), ![color de icono de rol](assets/job-role-icon-nwe-color.png) |  |
| [!UICONTROL Plan] | ![Icono de plan](assets/plan-icon.png), ![icono de plan azul](assets/nwe-plan-icon-60x57.png) |  |
| [!UICONTROL Portafolio] | ![Portfolio](assets/portfolio-icon-nwe.png) , ![icono Portfolio azul](assets/nwe-portfolios-icon.png) | ✔ |
| [!UICONTROL Programa] | ![Icono del programa](assets/program-icon-nwe.png) , ![Icono del programa naranja](assets/nwe-programs-icon.png) | ✔ |
| [!UICONTROL Proyecto] | ![Icono del proyecto](assets/project-icon-nwe.png), ![Icono del proyecto púrpura](assets/nwe-projects-icon.png) | ✔ |
| [!UICONTROL Informe] | ![Icono de informe](assets/report-icon-nwe.png) , ![Icono de informe verde](assets/nwe-reports-icon.png) |  |
| [!UICONTROL Tarea] | ![Icono de tarea](assets/task-icon-new.png) , ![Icono de tarea verde](assets/nwe-tasks-icon.png) | ✔ |
| [!UICONTROL Equipo] | ![Icono del equipo](assets/team-icon-nwe.png), ![Icono del equipo ronda](assets/team-icon-nwe-color.png) , ![Icono de equipos](assets/nwe-teams-icon.png) |  |
| [!UICONTROL Plantilla] | ![Icono de plantilla](assets/template-icon-nwe.png) , ![Icono de plantilla verde](assets/nwe-templates-icon.png) |  |
| [!UICONTROL Usuario] | ![Icono de usuario gris](assets/users-icon-gray.png) , ![Icono de usuario azul](assets/user-icon-blue.png) , ![Icono de usuario con iniciales](assets/user-icon-initials.png) , ![Avatar](assets/user-avatar.png) , ![Menú principal del icono de usuario](assets/user-main-menu-area.png) |  |

## Números de referencia de objetos

A cada objeto creado en [!DNL Workfront] se le asigna un número de referencia único. Los números de referencia son útiles para distinguir entre dos objetos similares (como tareas con el mismo nombre). Se pueden buscar objetos utilizando sus números de referencia y se pueden incluir números de referencia en los informes.

Para obtener información acerca de cómo buscar objetos por número de referencia, consulte [Utilizar el número de referencia de los objetos](../../../workfront-basics/navigate-workfront/search/reference-number-of-objects.md).

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
| [!UICONTROL Empresas] | ✓ | ✓ |
| [!UICONTROL Notas] (o [!UICONTROL Actualizaciones]) | ✓ |  |

Para obtener más información acerca de cómo ejecutar búsquedas básicas y avanzadas en [!DNL Workfront], consulte [Buscar [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md).


## Acceso restringido a objetos

Cuando un usuario no tiene acceso a un objeto, ve el mensaje “Sin acceso” en cualquier lugar donde se muestra el nombre de ese objeto en Workfront.

El acceso a los objetos se puede restringir en el nivel de acceso o en los permisos de un objeto específico.

Esto se aplica a todos los objetos y objetos secundarios enumerados en la sección [Interdependencia y jerarquía de objetos](#interdependency-and-hierarchy-of-objects) de este artículo. Esto no se aplica a los objetos Equipo y Usuario.

## Informar sobre objetos

Es extremadamente importante comprender la jerarquía y la interdependencia de los objetos antes de comenzar a crear informes en [!DNL Workfront]. Los informes son específicos de los objetos. Debe seleccionar el objeto correcto para el informe antes de poder mostrar los datos deseados.

>[!IMPORTANT]
>
>Solo puede crear informes sobre el objeto seleccionado y los objetos principales en el mismo informe. No se puede tener información sobre los objetos secundarios en un informe de objeto principal. Por ejemplo, se puede mostrar la información del proyecto en un informe de tareas, pero no la información de tareas en un informe de proyecto.

Puede crear informes sobre todos los objetos de la base de datos utilizando nuestra API abierta. Para obtener una lista completa de todos los objetos de la base de datos, consulte [Explorador de API](../../../wf-api/general/api-explorer.md).

>[!NOTE]
>
> * Si ha personalizado los nombres de los objetos mediante una plantilla de diseño, también se han personalizado los nombres de los objetos en el generador de informes. Asegúrese de saber qué objetos se han personalizado y de buscar el nombre personalizado en el generador de informes. Para obtener más información sobre qué objetos pueden tener nombres personalizados en [!DNL Workfront], consulte [Nombres de objeto que se pueden personalizar con una [!UICONTROL plantilla de diseño]](#object-names-that-can-be-customized-using-a-layout-template) en este artículo.
> * Al utilizar el modo de texto en los informes, los nombres de los objetos en las expresiones del modo de texto son los nombres estándar de [!DNL Workfront], y no los nombres de objeto personalizados. Para obtener más información acerca del uso del modo de texto en los informes, consulte [Información general sobre el modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Para obtener más información sobre cómo generar un informe, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
Para obtener más información sobre nuestra API, consulte [Explorador de API](../../../wf-api/general/api-explorer.md).

### Objetos disponibles para informes

Puede crear informes sobre los objetos siguientes al usar el generador de informes en la aplicación web [!DNL Workfront]. Los puntos de viñeta con sangría proporcionan más información sobre el objeto, y no representan objetos adicionales.

* [!UICONTROL Proyecto]
* [!UICONTROL Tarea]
* [!UICONTROL Hora]
* [!UICONTROL Problema]
* [!UICONTROL Usuario]
* Nivel de [!UICONTROL acceso]
* [!UICONTROL Aprobación]
* [!UICONTROL Proceso de aprobación]
* [!UICONTROL Asignación]
* [!UICONTROL Línea de base]
* [!UICONTROL Tarea de la línea de base]
* [!UICONTROL Registro de facturación]
* [!UICONTROL Horas presupuestadas]
   * Son las [!UICONTROL horas presupuestadas], tal como aparecen en las herramientas de administración de recursos obsoletas más antiguas.
   * El campo “Horas pres.” en el informe [!UICONTROL Horas presupuestadas] hace referencia a las horas presupuestadas para las funciones del [!UICONTROL Planificador de recursos]. Para obtener más información, consulte [Comprender [!UICONTROL el coste presupuestado de la mano de obra] y las [!UICONTROL Horas presupuestadas] para proyectos](../../../manage-work/projects/project-finances/budgeted-labor-cost.md).

* [!UICONTROL Evento de calendario]
* [!UICONTROL Compañía]
* [!UICONTROL Formulario personalizado]
* [!UICONTROL Panel]
* [!UICONTROL Documento]
* [!UICONTROL Aprobación de documento]
* [!UICONTROL Versión del documento]
   * Puede ver información sobre la versión del documento, el documento con el que está asociada la versión, quién creó la versión y el usuario que creó la prueba en la versión del documento, si existe (Creador de revisiones).
* [!UICONTROL Plantilla del correo electrónico]
* [!UICONTROL Gasto]
* [!UICONTROL Tipo de gasto]
* [!UICONTROL Página externa]
* [!UICONTROL Favorito]
* [!UICONTROL Filtro]
* [!UICONTROL Meta]
   * Puede generar un informe para metas estratégicas o mostrar información relacionada con las metas en un informe de proyecto cuando los proyectos están asociados con metas como actividades de metas. Puede crear metas estratégicas y conectar proyectos con ellas solo si su organización ha adquirido una licencia de [!DNL Workfront Goals]. Para obtener información acerca de [!DNL Workfront Goals], consulte la información general de [[!DNL Workfront Goals] ](../../../workfront-goals/goal-management/wf-goals-overview.md). Para obtener información acerca de cómo conectar proyectos con metas estratégicas, consulte [Añadir proyectos a metas en Adobe Workfront Goals](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).
*No puede informar sobre metas de proyecto que estén asociadas con un [!UICONTROL Caso empresarial]. Para obtener información sobre los objetivos del proyecto frente a los objetivos estratégicos, consulte el [Glosario de [!DNL Adobe Workfront] terminología](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* [!UICONTROL Grupo]
* [!UICONTROL Agrupación]
* [!UICONTROL Tipo de hora]
* [!UICONTROL Iniciativa]
   * Puede generar un informe para las iniciativas que son los objetos secundarios de un plan solo si su compañía ha adquirido una licencia de [!DNL Workfront Scenario Planner]. Para obtener información acerca de las iniciativas, consulte [Información general sobre iniciativas en  [!DNL Workfront Scenario Planner]](../../../scenario-planner/initiatives-overview.md).

* Función del puesto de la iniciativa
   * Puede generar un informe para las funciones asociadas con las iniciativas de un plan solo si su compañía ha adquirido una licencia de [!DNL Workfront Scenario Planner]. Para obtener información acerca de cómo crear iniciativas y asociarlas con funciones, consulte [Crear y editar iniciativas en [!DNL Workfront Scenario Planner]](../../../scenario-planner/create-and-edit-initiatives.md).

* [!UICONTROL Iteración]
* [!UICONTROL Función]
* [!UICONTROL Entrada de cuaderno]
   * Puede informar sobre las actualizaciones del sistema rastreadas en el área de [!UICONTROL Actualizaciones] de objetos como tareas, proyectos, problemas, etc. Para obtener más información, consulte [Informe sobre el área de actualizaciones con un informe de entrada de diario](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

* [!UICONTROL Plantilla de diseño]
* [!UICONTROL Hito]
* [!UICONTROL Ruta de hitos]
* [!UICONTROL Nota] o [!UICONTROL Actualizaciones]
   * Puede informar sobre los comentarios añadidos por usuarios individuales.

* [!UICONTROL Parámetro] (o [!UICONTROL Campo personalizado])
* [!UICONTROL Grupo de parámetros] (o [!UICONTROL Salto de sección])
* [!UICONTROL Portafolios]
* [!UICONTROL Programa]
* [!UICONTROL Proyecto (datos financieros)]
   * La información financiera se rellena en los informes de [!UICONTROL Proyecto (datos financieros)] solamente cuando los datos asociados a ella tienen menos de 5 años. Por ejemplo, si se asignó una función a una tarea en enero de 2015 y hoy es septiembre de 2021, un campo financiero como [!UICONTROL Fecha de asignación] para la función no se rellena en el informe [!UICONTROL Proyecto (datos financieros)].

  >[!CAUTION]
  >
  >La ejecución de un informe de proyecto (datos financieros) realiza un nuevo cálculo de los datos financieros, que puede sobrescribir los datos financieros anteriores y puede tardar un tiempo considerable. Para obtener más información sobre las consecuencias del cálculo de datos financieros, consulte [Recalcular las finanzas de un proyecto](/help/quicksilver/manage-work/projects/project-finances/recalculate-project-finances.md).

* [!UICONTROL Aprobación de revisión]
   * Permite ver información diversa sobre la aprobación de la revisión, que incluye: la prueba que se envió para su aprobación, información sobre el [!UICONTROL aprobador], información sobre el solicitante (si el solicitante es un usuario con licencia de [!DNL Workfront]), información de la versión, el ID de la prueba y la fecha de creación de la prueba.\
      Los informes de [!UICONTROL Aprobación de revisión] solo incluyen pruebas disponibles en las áreas de Mi trabajo de los usuarios en las que aún no se han tomado decisiones.\
   * Se han asignado aprobaciones de revisión en [!DNL Workfront] tal como se describe en [Añadir usuarios a una prueba](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) en [Compartir una prueba en [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

* [!UICONTROL Cola]
* [!UICONTROL Tema de la cola]
* [!UICONTROL Tarifa] (esto muestra la información de la función [!UICONTROL Tarifa de facturación])
* [!UICONTROL Notificación de un recordatorio]
* [!UICONTROL Informe]
* [!UICONTROL Conjunto de recursos]
* [!UICONTROL Riesgo]
* [!UICONTROL Tipo de riesgo]
* [!UICONTROL Programación]
* [!UICONTROL Cuadro de resultados]
* [!UICONTROL Equipo]
* [!UICONTROL Plantilla]
* [!UICONTROL Tarea de plantilla]
* [!UICONTROL Días libres]
   * Puede crear informes sobre los días libres personales de un usuario, tal como lo indique el usuario en su perfil.

* [!UICONTROL Plantilla de horas]
* [!UICONTROL Perfil de plantilla de horas]
* [!UICONTROL Grupo de temas]
* [!UICONTROL Aprobación del usuario]
* [!UICONTROL Delegación de usuarios]

   * Puede informar sobre los usuarios que se han delegado para realizar las tareas y los problemas de otros mientras están fuera de la oficina. Este informe muestra el usuario que está fuera de la oficina, así como el usuario que cumple con sus obligaciones mientras está fuera.

* [!UICONTROL Decisiones de los usuarios]

   * Puede crear informes sobre cuántas decisiones han tomado los usuarios en relación con las pruebas y los documentos en el mes actual.

* [!UICONTROL Vista]
* [!UICONTROL Elemento de trabajo] (esto genera un informe para las tareas y los problemas)
