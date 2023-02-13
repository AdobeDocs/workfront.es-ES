---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Acciones que deben realizarse después de instalar un modelo
description: Este artículo describe lo que debe hacer después de instalar un modelo en [!DNL Adobe Workfront] para implementar completamente el modelo para los usuarios del sistema.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6e5da58f-105a-4edf-8fc1-65e8762d43c6
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '1139'
ht-degree: 0%

---

# Acciones que deben realizarse después de instalar un modelo

Este artículo describe lo que debe hacer después de instalar un modelo en [!DNL Adobe Workfront] para implementar completamente el modelo para los usuarios del sistema.

* [Recomendaciones de plantillas de proyecto](#project-template-recommendations)
* [Recomendaciones sobre la estructura organizativa](#organizational-structure-recommendations)
* [Recomendaciones de tablero](#dashboard-recommendations)

## Recomendaciones de plantillas de proyecto {#project-template-recommendations}

Esta sección contiene recomendaciones para las plantillas de proyecto instaladas con los modelos.

### Asignar usuarios a las funciones y equipos recién creados {#assign-users-to-newly-created-roles-and-teams}

Las funciones o los equipos creados durante el proceso de instalación del modelo no tienen usuarios asociados automáticamente. Sin asignar usuarios a las funciones o equipos recién añadidos, creará trabajo para una función que nadie va a recoger. En algunos casos, es posible que tenga que crear nuevos usuarios para rellenar estas funciones y equipos. Para obtener información sobre la creación de nuevos usuarios, consulte [Agregar usuarios](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

### Aplicar un formulario personalizado a la plantilla y a las tareas de plantilla {#apply-a-custom-form-to-the-template-and-the-template-tasks}

El proceso de instalación no asocia la plantilla del proyecto con ningún formulario personalizado. Si los proyectos o las tareas requieren que se rellenen formularios o campos específicos para crear coherencia en los informes, o si el formulario de solicitud digital contiene campos que se deben conservar en el nivel de proyecto, se recomienda asociar la plantilla o las tareas de plantilla a esos formularios. Para obtener más información, consulte [Adición de un formulario personalizado a un objeto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

### Actualizar la duración y las estimaciones de esfuerzo de la tarea de plantilla {#update-template-task-duration-and-effort-estimates}

Cada tarea de la plantilla contiene una duración planificada y una estimación del esfuerzo planificado. Estas estimaciones sirven de punto de partida para las duraciones y el tiempo empleado en estas actividades. Sin embargo, las capacidades, habilidades y ritmo de su organización son únicos. Debe revisar la duración y el esfuerzo estimados de cada tarea para ajustarla a las necesidades de su organización. Para obtener más información, consulte [Administrar información de tarea en la [!UICONTROL Información general sobre los detalles de la tarea] area](../../manage-work/tasks/manage-tasks/task-information-in-overview.md).

### Asociación de una ruta de hitos y hitos {#associate-a-milestone-path-and-milestones}

El proceso de instalación no asocia la plantilla del proyecto con una ruta de hitos. Aplique una ruta de hitos a la plantilla y aplique hitos a las tareas clave de la plantilla para satisfacer las necesidades de informes de hitos. Para obtener más información, consulte [Asociar hitos con tareas](../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

### Despliegue la plantilla en su equipo {#roll-out-the-template-to-your-team}

Preparar materiales de capacitación tanto para los administradores de trabajo que utilizarán esta plantilla como para los colaboradores individuales que ejecutarán el trabajo dentro de la plantilla del proyecto.

### Crear o actualizar informes y tableros {#create-or-update-reports-and-dashboards}

Si la solución representa un nuevo tipo de trabajo que su organización no ha realizado anteriormente en [!DNL Workfront], es posible que necesite crear nuevos informes y tableros para que sean compatibles con el trabajo. Para obtener más información, consulte [Crear un informe personalizado](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) y [Crear un tablero](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

Si la solución es similar a un trabajo que ya ha estado ejecutando en [!DNL Workfront], debe comprobar que el trabajo se alimenta de los informes y tableros existentes según lo esperado. Si no se alimenta de los informes existentes, tome medidas para actualizar filtros o crear nuevos informes.

## Recomendaciones sobre la estructura organizativa {#organizational-structure-recommendations}

Esta sección contiene recomendaciones para los elementos de estructura organizativa instalados con los modelos.

### Compañías

Después de instalar un modelo que incluya a una empresa:

* Agregue un formulario personalizado para aumentar el registro de la empresa con detalles útiles (el formulario y sus detalles son exclusivos de usted). Para obtener más información, consulte [Adición de un formulario personalizado a un objeto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
* Si la empresa representa a un cliente, revise las tasas de anulación asociadas con la empresa. Para obtener más información, consulte [Anular las tasas de facturación de funciones de trabajo a nivel de empresa](../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).
* Si la empresa representa a un cliente y si hay otras plantillas de proyecto exclusivas para esa organización, primero preasocie las plantillas de proyecto con la empresa recién agregada. Para obtener más información, consulte [Editar plantillas de proyecto](../../manage-work/projects/create-and-manage-templates/edit-templates.md).
* Si la empresa representa a un cliente o a un proveedor, asocie los usuarios existentes de la organización externa que ya puedan estar en su entorno. Para obtener más información, consulte [Crear y editar empresas](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).
* Si la empresa representa a un cliente o a un proveedor, cree usuarios colaboradores adicionales para la organización externa que necesite en su entorno para optimizar la comunicación, la ejecución del trabajo y las aprobaciones. Para obtener información sobre la creación de nuevos usuarios, consulte [Agregar usuarios](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).
* Actualice las relaciones de organigrama para cualquier usuario ahora asociado con la empresa recién agregada. Para obtener más información, consulte [Crear informes directos](../../administration-and-setup/add-users/create-and-manage-users/create-direct-reports.md) y [Ver el organigrama](../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

Para obtener información adicional sobre las empresas, consulte [Crear y editar empresas](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## Recomendaciones de tablero {#dashboard-recommendations}

Esta sección contiene recomendaciones para los tableros y los informes instalados con un modelo.

### Actualizar los tableros recién creados para agregar o quitar informes

Los tableros agregados desde un modelo tienen uno o más informes, páginas externas o calendarios. Es probable que no necesite todos los informes y otros elementos de tablero, o que tenga que aumentar el tablero con informes, páginas externas y calendarios existentes antes de que esté listo para compartirlo con otras personas. Para obtener más información, consulte [Agregar un informe a un tablero](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

### Actualizar los informes recién creados para agregar o quitar columnas o criterios de filtro

Los informes distribuidos a través de un modelo de panel no tienen todas las columnas o criterios de filtro para admitir la configuración de [!DNL Workfront]. Se espera que realice algunos ajustes en los informes para adaptarlos a sus estándares. Para mantener la coherencia con otros informes de su entorno, es posible que desee agregar una columna que incluya en todos los informes del objeto que se enumera, o agregar algunos criterios de filtro que limiten los resultados a un tipo de proyecto o grupo de usuarios en particular. Para obtener más información, consulte [Crear o editar vistas](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md) y [Crear o editar filtros](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

### Uso compartido de tableros o informes con usuarios

Si no planea colocar el tablero en una plantilla de diseño, debe compartir el tablero con las personas que lo encuentren útil. Para obtener más información, consulte [Compartir un tablero](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md) y [Compartir un informe](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

### Agregar los tableros a las plantillas de diseño

La mejor manera de poner la información a disposición de otras personas es agregar tableros a las plantillas de diseño. Identifique las plantillas de diseño de las personas que más se beneficiarían de revisar el tablero de forma regular y añada el tablero recién creado a esas plantillas de diseño. Para obtener más información, consulte [Creación y administración de plantillas de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

### Actualizar otros tableros e informes

La introducción de un nuevo tablero y sus informes pueden hacer posible la retirada y el ajuste de otros tableros e informes existentes. Tómese el tiempo necesario para revisar los informes existentes e identificar cualquier informe redundante y contradictorio.

### Distribuir datos personalizados a formularios relevantes

Algunos informes incluidos en un modelo de tablero tienen campos de datos personalizados en la vista, el filtro o la agrupación del informe. En algunos casos, el modelo también tendrá un formulario al que están asociados estos campos. Sin embargo, la mayoría de las veces, los campos personalizados no se aplican a un formulario personalizado. Para que las columnas, filtros o agrupaciones funcionen correctamente, estos campos deben estar asociados a formularios conectados a un usuario, proyecto, tarea u otro registro de objeto. Para obtener más información, consulte [Añadir un campo personalizado a un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).
