---
title: 20.4 Mejoras en la administración de proyectos
description: 20.4 Mejoras en la administración de proyectos
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: f21f33b3-5e49-4bb0-9eda-7cf4c016361c
source-git-commit: 12bab42ab13935fa284aa334120afcfb602bf412
workflow-type: tm+mt
source-wordcount: '1365'
ht-degree: 100%

---

# 20.4 Mejoras en la administración de proyectos

Esta página describe todas las mejoras realizadas en la administración de proyectos con la versión 20.4 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción el 9 de noviembre de 2020.

Para obtener una lista de todos los cambios disponibles con la versión 20.4, consulte [Información general de la versión 20.4](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## Nuevo para administradores: controle cómo se comparte un campo personalizado

Para brindar un mayor control sobre quién puede editar, eliminar y utilizar los campos personalizados que crea, hemos añadido la capacidad de configurar exactamente cómo desea que se compartan.

Hasta ahora, cuando creaba un campo personalizado, todos los miembros del sistema podían editarlo. Este sigue siendo el estado predeterminado de un campo personalizado, pero ahora puedes limitar el uso compartido de un campo personalizado a ciertos usuarios, roles, equipos, grupos y empresas. Y puede determinar si los destinatarios pueden administrar o solo ver el campo personalizado.

Además, para que esta experiencia te resulte familiar, hemos diseñado la interfaz de usuario de esta funcionalidad de manera similar a otras áreas de compartición de objetos en Workfront.

## Nuevo para administradores: uso compartido de formularios personalizados estandarizados

Hemos estandarizado el uso compartido de formularios personalizados para que puedas utilizar el mismo proceso de compartición de objetos de Workfront que ya conoces. Además, la nueva experiencia de uso compartido le proporciona un mayor control sobre quién puede editar, eliminar y utilizar formularios personalizados que cree. Puede limitar el uso compartido de un formulario personalizado a determinados usuarios, funciones, equipos, grupos y empresas. Además, puede determinar si esos destinatarios pueden ver o administrar el formulario personalizado.

Para obtener más información, consulte [Compartir un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).

## Exportar formularios personalizados e información general desde la sección detalles de un proyecto, tarea o problema

Ahora puede exportar la información del formulario personalizado a un archivo PDF. Puede exportar formularios personalizados desde proyectos, tareas o problemas cuando acceda al formulario en la sección de Detalles de los objetos.

Además de exportar los formularios personalizados de proyectos, tareas y problemas, ahora puede incluir el área Información general en el PDF exportado.

Para obtener información sobre cómo exportar formularios personalizados desde un objeto, consulte [Exportar formularios personalizados y detalles de objetos](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

## Añadir rápidamente una iteración

>[!NOTE]
>
>Esta función se ha eliminado temporalmente del entorno de producción. Esta página se actualizará cuando la función esté disponible.

Para simplificar la experiencia de creación de una iteración, se ha añadido un nuevo botón que permite añadir una iteración desde la pestaña iteraciones. Aquí puede crear una iteración y luego añadir tareas y problemas más adelante.

Puede seguir creando una iteración en la etiqueta de registro de pendientes como antes.

Para obtener más información, consulte [Crear una iteración](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

## Nueva sección de métricas disponible en proyectos

Para ahorrar tiempo y aumentar la comprensión del estado general de un proyecto, ahora hay una sección de Métricas disponible en un proyecto que incluye información sobre lo siguiente:

* Trabajo completado, incompleto, vencido y próximo
* Cantidades de tarea y problema agrupadas por estado o prioridad
* Esfuerzo laboral asignado a cada usuario

Puede hacer selecciones en los gráficos para ver diferentes aspectos de las tareas y problemas de un proyecto y hacer clic en ciertos elementos para mostrar la información de las tareas.

<!--This feature is now included in the [Planner Fundamentals, Part 3 learning path](https://one.workfront.com/s/learningpath3/planner-fundamentals-for-the-new-workfront-experience-part-3-manage-a-project-20Y0z000000bm7xEAA) on Workfront One. -->

## Nuevo para administradores: asignar un coordinador empresarial a un grupo

Para ayudarle a organizar y definir mejor sus grupos, hemos añadido la capacidad de asignar un usuario como coordinador empresarial para un grupo (o subgrupo). Un coordinador empresarial es un usuario de Workfront que toma decisiones comerciales para un grupo.

El nuevo campo de coordinador empresarial se puede utilizar en filtros, vistas y agrupaciones de informes. Por ejemplo, puedes filtrar por un determinado Líder de Negocios para listar solo los grupos a los que esa persona está asignada en ese rol.

Para obtener más información, consulte [Información general de Business Leader](../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md).

<!--This feature is now included in the [Administrator Fundamentals, Part 1 learning path](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) on Workfront One. -->

## Nuevo para administradores: asocie portafolios, programas y compañías con grupos

Cuando los administradores de Workfront crean o editan un portafolio, un programa o una compañía, pueden asignarlo a un grupo. Con los grupos asignados a estos objetos, es fácil identificar las responsabilidades de tu grupo para ellos.

Por ejemplo, puede enumerar todos los portafolios de su organización en un informe y ver la columna Grupo para ver en cuáles está trabajando su grupo.

Para obtener más información, consulte la sección “Acerca de la asociación de un grupo con un objeto” en el artículo [Descripción general de los Grupos](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

<!--This feature is now included in the [Administrator Fundamentals, Part 1 learning path](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) on Workfront One. -->

## Nuevo para administradores: los administradores de un grupo asignado a una compañía pueden administrar la compañía

Hemos facilitado a un administrador de grupo la gestión de una empresa asociada a su grupo en Workfront. El acceso para administrar la compañía está disponible automáticamente cuando se realiza la asociación. Esto es especialmente importante cuando el administrador del grupo no tiene acceso administrativo a las empresas.

Para obtener más información, consulte [Crear y editar empresas](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

Para obtener información acerca del acceso administrativo a las compañías, consulte [Conceder a los usuarios acceso administrativo a determinadas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

<!--This feature is now included in the [Administrator Fundamentals, Part 1 learning path](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) on Workfront One. -->

## Reemplazar el botón Trabajar en ello por el botón Inicio

Para ayudar a registrar la fecha y hora en que realmente comienza el trabajo en un elemento, los usuarios pueden reemplazar el botón Trabajar en ello por el botón Inicio que actualiza automáticamente el estado y la Fecha de Inicio Real del elemento de trabajo.

Actualizado el 24 de septiembre: Después de hacer clic en Iniciar tarea o Iniciar problema, ahora tienes la opción de revertir tu elección e indicar que tal vez no estés listo para comenzar a trabajar en un elemento haciendo clic en Deshacer. El elemento de trabajo vuelve al estado Nuevo y se eliminan la Fecha de confirmación y la Fecha real de inicio. La opción Deshacer se muestra por un tiempo muy corto y se elimina después de que navegues fuera de la página o la actualices.

Para obtener más información sobre cómo configurar esta opción, consulte [Reemplazar el botón Trabajar en ello por el botón Inicio](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

<!--This feature is now included in the [Worker Fundamentals learning path](https://one.workfront.com/s/learningpath3/worker-fundamentals-for-the-new-workfront-experience-20Y0z000000blg8EAA) and the [Administrator Fundamentals, Part 1 learning path](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) on Workfront One. -->

## Permitir varios borradores para un tema de cola

Para darle más libertad al trabajar con solicitudes, ya no hay un límite para la cantidad de borradores que puede guardar para un tema en cola. Al crear una nueva solicitud, puedes seleccionar un borrador existente de una lista de borradores para el mismo tema de la cola, sobrescribirlo y enviarlo como una nueva solicitud o puedes crear una nueva solicitud desde cero.

Antes de esta mejora, Workfront solo guardaba un borrador para cada tema de la cola en la cola de solicitudes.

Para obtener información sobre cómo enviar solicitudes, consulte [Crear y enviar solicitudes de Workfront](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

## Asignar un grupo a un equipo

Para facilitar la gestión y generación de informes sobre los equipos asociados a un grupo, ahora puedes asignar cualquier grupo a un equipo que tengas acceso para editar.

Al asignar un equipo a un grupo, sus administradores de grupo pueden administrar el equipo sin ser miembros de él. En la página Detalles del equipo, pueden ver los equipos asignados a los grupos que administran. Y pueden ejecutar un informe para enumerar todos los equipos asociados con un grupo determinado.

Para obtener más información, consulte [Crear un equipo](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).

<!--This feature is now included in the [Administrator Fundamentals, Part 1 learning path](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) on Workfront One. -->

## Los nuevos campos permiten informar sobre los datos de un grupo de nivel superior y todos sus subgrupos

Para identificar los datos asociados con un grupo de nivel superior y sus subgrupos, hemos añadido un nuevo campo de ID de Grupo Principal que puede usar en Filtros, Vistas y Agrupaciones cuando cree informes sobre objetos de Grupo.

Este campo debe ser especialmente útil para los administradores de grupo que administran grupos que contienen varios subgrupos.

Por ejemplo, imagine que administra un grupo denominado Marketing que tiene los subgrupos Marketing de campo y Marketing digital. Puede enumerar los proyectos que pertenecen a los 3 grupos creando un filtro de área de proyectos que tenga la siguiente regla de filtro:
<pre>Grupo: Nombre principal superior &gt; Igual a &gt; Marketing</pre>También hemos añadido un nuevo campo de Nombre del Grupo Principal que puede usar para identificar datos asociados con grupos de nivel superior en Vistas (no en Filtros ni Agrupaciones).

Para obtener información acerca del uso de campos en listas e informes, consulte [Glosario de terminología de Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## Nueva opción para cancelar su acción al descartar un borrador de solicitud

Al descartar un borrador guardado, ahora puede hacer clic en Cancelar en el mensaje de confirmación que le informa de que se eliminará el borrador. De este modo, no perderá el borrador en caso de que cambie de opinión sobre su descarte.

Esta función solo está disponible en la nueva experiencia de Workfront. Para obtener más información, consulte [Crear y enviar solicitudes de Workfront](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FManage_work%2FRequests%2FCreate_Requests%2Fcreate-submit-requests.html).

