---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Acciones que se deben realizar después de instalar un modelo
description: Este artículo describe lo que debe hacer después de instalar un modelo en  [!DNL Adobe Workfront]  para implementar completamente el modelo para los usuarios del sistema.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 6e5da58f-105a-4edf-8fc1-65e8762d43c6
source-git-commit: 55c8a3e5d0041a0e975bfd979a2d2e38930fea8d
workflow-type: tm+mt
source-wordcount: '1138'
ht-degree: 0%

---

# Acciones que se deben realizar después de instalar un modelo

Este artículo describe lo que debe hacer después de instalar un modelo en [!DNL Adobe Workfront] para implementar completamente el modelo para los usuarios del sistema.

* [Recomendaciones de plantilla de proyecto](#project-template-recommendations)
* [Recomendaciones sobre la estructura organizativa](#organizational-structure-recommendations)
* [Recomendaciones de panel](#dashboard-recommendations)

## Recomendaciones de plantilla de proyecto {#project-template-recommendations}

Esta sección contiene recomendaciones para las plantillas de proyecto instaladas con los modelos.

### Asignar usuarios a los roles y equipos recién creados {#assign-users-to-newly-created-roles-and-teams}

Los roles o equipos creados durante el proceso de instalación del modelo no tienen usuarios asociados automáticamente. Sin asignar usuarios a los roles o equipos recién agregados, creará trabajo para una función que nadie recogerá. En algunos casos, es posible que tenga que crear nuevos usuarios para desempeñar estas funciones y equipos. Para obtener información sobre cómo crear usuarios nuevos, consulte [Agregar usuarios](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

### Aplicar un formulario personalizado a las tareas de plantilla y de plantilla {#apply-a-custom-form-to-the-template-and-the-template-tasks}

El proceso de instalación no asocia la plantilla del proyecto con ningún formulario personalizado. Si los proyectos o las tareas requieren que se rellenen formularios o campos específicos para crear coherencia de la creación de informes, o si el formulario de solicitud digital contiene campos que deben conservarse en el nivel de proyecto, se recomienda asociar las tareas de plantilla o plantilla con esos formularios. Para obtener más información, vea [Agregar un formulario personalizado a un objeto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

### Actualizar la duración y las estimaciones de esfuerzo de la tarea de plantilla {#update-template-task-duration-and-effort-estimates}

Cada tarea de la plantilla contiene una duración planificada y una estimación del esfuerzo planificado. Estas estimaciones sirven de punto de partida para las duraciones y el tiempo empleado en estas actividades. Sin embargo, las capacidades, habilidades y ritmo de su organización son únicos. Debe revisar la duración y el esfuerzo estimados de cada tarea para ajustarlos y reflejar las necesidades de su organización. Para obtener más información, vea [Administrar información de tareas en el área [!UICONTROL Información general sobre detalles de tareas]](../../manage-work/tasks/manage-tasks/task-information-in-overview.md).

### Asociar una trayectoria e hitos de hito {#associate-a-milestone-path-and-milestones}

El proceso de instalación no asocia la plantilla de proyecto con una ruta de hitos. Aplique una trayectoria del hito a la plantilla y aplique hitos a las tareas clave de la plantilla para satisfacer sus necesidades de creación de informes de hito. Para obtener más información, vea [Asociar hitos con tareas](../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

### Despliegue la plantilla en su equipo {#roll-out-the-template-to-your-team}

Prepare materiales de formación tanto para los responsables de trabajo que utilizarán esta plantilla como para los colaboradores individuales que ejecutarán el trabajo en la plantilla del proyecto.

### Creación o actualización de informes y paneles {#create-or-update-reports-and-dashboards}

Si la solución representa un nuevo tipo de trabajo que su organización no ha realizado anteriormente en [!DNL Workfront], es posible que necesite crear nuevos informes y paneles para admitir el trabajo. Para obtener más información, consulte [Crear un informe personalizado](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) y [Crear un tablero](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

Si la solución es similar al trabajo que ya ha estado ejecutando en [!DNL Workfront], debe comprobar que el trabajo se alimenta de los informes y paneles existentes según lo esperado. Si no se incorpora a los informes existentes, tome medidas para actualizar los filtros o crear nuevos informes.

## Recomendaciones sobre la estructura organizativa {#organizational-structure-recommendations}

Esta sección contiene recomendaciones para los elementos de estructura organizativa instalados con los modelos.

### Compañías

Después de instalar un modelo que incluya una empresa:

* Agregue un formulario personalizado para aumentar el registro de la compañía con detalles útiles (el formulario y sus detalles son exclusivos de usted). Para obtener más información, vea [Agregar un formulario personalizado a un objeto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
* Si la compañía representa a un cliente, revise las tasas de anulación asociadas con la compañía. Para obtener más información, consulte [Anular tarifas de facturación de rol a nivel de compañía](../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).
* Si la compañía representa a un cliente y si hay otras plantillas de proyecto únicas para esa organización, primero asocie previamente las plantillas de proyecto a la compañía recién agregada. Para obtener más información, consulte [Editar plantillas de proyecto](../../manage-work/projects/create-and-manage-templates/edit-templates.md).
* Si la empresa representa a un cliente o a un proveedor, asocie a los usuarios existentes de la organización externa que ya estén en su entorno. Para obtener más información, consulte [Crear y editar compañías](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).
* Si la compañía representa a un cliente o a un proveedor, cree usuarios colaboradores adicionales para la organización externa que pueda necesitar en su entorno para optimizar la comunicación, la ejecución del trabajo y las aprobaciones. Para obtener información sobre cómo crear usuarios nuevos, consulte [Agregar usuarios](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).
* Actualice las relaciones del organigrama de los usuarios que ahora estén asociados a la compañía recién agregada. Para obtener más información, consulte [Crear informes directos](../../administration-and-setup/add-users/create-and-manage-users/create-direct-reports.md) y [Ver el organigrama](../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

Para obtener información adicional sobre compañías, consulte [Crear y editar compañías](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## Recomendaciones de panel {#dashboard-recommendations}

Esta sección contiene recomendaciones para los paneles e informes instalados con un modelo.

### Actualizar los paneles recién creados para agregar o quitar informes

Los paneles agregados desde un modelo tienen uno o más informes, páginas externas o calendarios. Es probable que no necesite todos los informes y otros elementos del panel, o que necesite aumentar el panel con informes, páginas externas y calendarios existentes antes de que esté listo para compartirse con otras personas. Para obtener más información, vea [Agregar un informe a un panel](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

### Actualizar los informes recién creados para agregar o quitar columnas o criterios de filtro

Los informes distribuidos a través de un modelo de panel no tienen todas las columnas ni criterios de filtro que admitan la configuración de [!DNL Workfront]. Se espera que realice algunos ajustes en los informes para adaptarlos a sus estándares. Para generar coherencia con otros informes de su entorno, puede que desee agregar una columna que incluya en todos los informes para el objeto que se muestra o agregar algunos criterios de filtro que limiten los resultados a un tipo de proyecto o grupo de usuarios en particular. Para obtener más información, consulte [Crear o editar vistas](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md) y [Crear o editar filtros](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

### Uso compartido de paneles o informes con los usuarios

Si no planea colocar el tablero en una plantilla de diseño, debe compartirlo con las personas que lo consideren útil. Para obtener más información, consulte [Compartir un tablero](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md) y [Compartir un informe](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

### Añadir los paneles a las plantillas de diseño

La mejor manera de poner la información a disposición de otras personas es agregar paneles a las plantillas de diseño. Identifique las plantillas de diseño de las personas que más se beneficiarían de revisar el panel regularmente y agregue el panel recién creado a esas plantillas de diseño. Para obtener más información, consulte [Crear y administrar plantillas de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

### Actualización de otros tableros e informes

La introducción de un nuevo tablero y sus informes puede hacer posible retirar y ajustar otros tableros e informes existentes. Tómese el tiempo necesario para revisar los informes existentes e identificar cualquier informe redundante y contradictorio.

### Distribuir datos personalizados en formularios relevantes

Algunos informes incluidos en un modelo de panel tienen campos de datos personalizados en la vista, el filtro o la agrupación del informe. En algunos casos, el modelo también tendrá un formulario al que están asociados estos campos. Sin embargo, la mayoría de las veces, los campos personalizados no se aplican a un formulario personalizado. Para que las columnas, los filtros o las agrupaciones funcionen correctamente, estos campos deben asociarse a formularios conectados a un registro de usuario, proyecto, tarea u otro registro de objeto. Para obtener más información, vea [Diseñar un formulario con el diseñador de formularios](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
