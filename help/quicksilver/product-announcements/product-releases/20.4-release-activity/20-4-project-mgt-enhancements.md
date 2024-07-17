---
title: 20.4 Mejoras en la gestión de proyectos
description: 20.4 Mejoras en la gestión de proyectos
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: f21f33b3-5e49-4bb0-9eda-7cf4c016361c
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1485'
ht-degree: 0%

---

# 20.4 Mejoras en la gestión de proyectos

Esta página describe todas las mejoras realizadas en la administración de proyectos con la versión 20.4 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción el 9 de noviembre de 2020.

Para obtener una lista de todos los cambios disponibles con la versión 20.4, consulte [Descripción general de la versión 20.4](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## Nuevo para administradores: Controle cómo se comparte un campo personalizado

Para darle un mayor control sobre quién puede editar, eliminar y utilizar los campos personalizados que cree, hemos añadido la capacidad de configurar exactamente cómo desea que se compartan.

Hasta ahora, cuando creaba un campo personalizado, todos los miembros del sistema podían editarlo. Este sigue siendo el estado predeterminado de un campo personalizado, pero ahora puede limitar el uso compartido de un campo personalizado a determinados usuarios, roles, equipos, grupos y empresas. Y puede determinar si los destinatarios pueden administrar o solo ver el campo personalizado.

Además, para que esta experiencia le resulte familiar, hemos diseñado la interfaz de usuario para que esta capacidad sea similar a otras áreas de objetos que se comparten en Workfront.

Para obtener más información, consulte [Configurar el uso compartido para campos y widgets personalizados](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md).

## Nuevo para administradores: uso compartido de formularios personalizados estandarizados

Hemos estandarizado el uso compartido para Custom Forms para que pueda utilizar el mismo proceso de uso compartido de objetos de Workfront que ya conoce. Además, la nueva experiencia de uso compartido le proporciona un mayor control sobre quién puede editar, eliminar y utilizar Forms personalizado que cree. Puede limitar el uso compartido de un formulario personalizado a determinados usuarios, funciones, equipos, grupos y empresas. Además, puede determinar si esos destinatarios pueden ver o administrar el formulario personalizado.

Para obtener más información, vea [Compartir un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).

## Exportar formularios personalizados e información general desde la sección Detalles de un proyecto, tarea o problema

Ahora puede exportar la información del formulario personalizado a un archivo .pdf. Puede exportar formularios personalizados desde proyectos, tareas o problemas al acceder al formulario en la sección Detalles de los objetos.

Además de exportar los formularios personalizados de proyectos, tareas y problemas, ahora puede incluir el área Información general en el PDF exportado.

Para obtener información sobre cómo exportar formularios personalizados desde un objeto, consulte [Exportar formularios personalizados y detalles del objeto](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

## Añadir rápidamente una iteración

>[!NOTE]
>
>Esta función se ha eliminado temporalmente del entorno de producción. Esta página se actualizará cuando la función esté disponible.

Para simplificar la experiencia de creación de una iteración, se ha agregado un nuevo botón que permite agregar una iteración desde la pestaña iteraciones. Aquí puede crear una iteración y luego agregar tareas y problemas más adelante.

Puede seguir creando una iteración en la etiqueta de registro de pendientes como antes.

Para obtener más información, vea [Crear una iteración](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

## Nueva sección de métricas disponible en los proyectos

Para ahorrar tiempo y mejorar la comprensión del estado general de un proyecto, ahora hay una sección de Métricas disponible en un proyecto que incluye información sobre lo siguiente:

* Trabajo completado, incompleto, vencido y próximo
* Cantidades de tarea y problema agrupadas por estado o prioridad
* Esfuerzo de trabajo asignado a cada usuario

Puede realizar selecciones en los gráficos para ver diferentes aspectos de las tareas y problemas de un proyecto y hacer clic en ciertos elementos para mostrar la información de las tareas.

Esta característica ahora se incluye en la ruta de aprendizaje [Aspectos básicos del planificador, parte 3](https://one.workfront.com/s/learningpath3/planner-fundamentals-for-the-new-workfront-experience-part-3-manage-a-project-20Y0z000000bm7xEAA) en Workfront One.

## Nuevo para administradores: asignar un coordinador empresarial a un grupo

Para ayudarle a organizar y definir mejor sus grupos, hemos añadido la capacidad de asignar un usuario como coordinador empresarial para un grupo (o subgrupo). Un coordinador empresarial es un usuario de Workfront que toma decisiones comerciales para un grupo.

El nuevo campo de coordinador empresarial se puede utilizar en filtros, vistas y agrupaciones de informes. Por ejemplo, puede filtrar por un coordinador empresarial concreto para que sólo se incluyan en la lista los grupos para los que está asignada esa persona en esa función.

Para obtener más información, vea [Resumen del coordinador empresarial](../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md).

Esta característica ahora se incluye en la ruta de aprendizaje [Aspectos básicos del administrador, parte 1](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) en Workfront One.

## Nuevo para administradores: asociar portafolios, programas y compañías con grupos

Cuando los administradores de Workfront crean o editan un portafolio, un programa o una compañía, pueden asignarlo a un grupo. Con los grupos asignados a estos objetos, es fácil identificar las responsabilidades de su grupo para ellos.

Por ejemplo, puede enumerar todos los portafolios de su organización en un informe y ver la columna Grupo para ver en cuáles está trabajando su grupo.

Para obtener más información, consulte la sección &quot;Acerca de la asociación de un grupo con un objeto&quot; en el artículo [Información general de grupos](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

Esta característica ahora se incluye en la ruta de aprendizaje [Aspectos básicos del administrador, parte 1](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) en Workfront One.

## Nuevo para administradores: los administradores de un grupo asignado a una compañía pueden administrar la compañía

Hemos facilitado a un administrador de grupo la gestión de una empresa asociada a su grupo en Workfront. El acceso para administrar la compañía está disponible automáticamente cuando se realiza la asociación. Esto es especialmente importante cuando el administrador del grupo no tiene acceso administrativo a las empresas.

Para obtener más información, consulte [Crear y editar compañías](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

Para obtener información acerca del acceso administrativo a las compañías, vea [Conceder acceso administrativo a los usuarios a ciertas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Esta característica ahora se incluye en la ruta de aprendizaje [Aspectos básicos del administrador, parte 1](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) en Workfront One.

## Reemplazar el botón Trabajar en ello por un botón Iniciar

Para ayudar a capturar la fecha y la hora en la que el trabajo comienza realmente en un elemento de trabajo, los usuarios pueden reemplazar el botón Trabajar en ello por un botón Iniciar que actualice automáticamente el estado y la Fecha real de inicio del elemento de trabajo.

Actualizado el 24 de septiembre: después de hacer clic en Iniciar tarea o Iniciar problema, ahora tiene la opción de revertir su elección e indicar que podría no estar listo para comenzar a trabajar en un elemento de trabajo al hacer clic en Deshacer. El elemento de trabajo vuelve al estado Nuevo y se eliminan la Fecha de confirmación y la Fecha de inicio real. La opción Deshacer se muestra durante un tiempo muy corto y se borra después de salir de la página o de actualizarla.

Para obtener más información sobre cómo configurar esta opción, vea [Reemplazar el botón Trabajar en ello por un botón Iniciar](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

Esta característica ahora se incluye en la ruta de aprendizaje [Aspectos básicos del trabajador](https://one.workfront.com/s/learningpath3/worker-fundamentals-for-the-new-workfront-experience-20Y0z000000blg8EAA) y en la ruta de aprendizaje [Aspectos básicos del administrador, parte 1](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) en Workfront One.

## Permitir varios borradores para un tema de cola

Para darle más libertad al trabajar con solicitudes, ya no hay un límite para la cantidad de borradores que puede guardar para un tema en cola. Al crear una solicitud nueva, puede seleccionar un borrador existente de una lista de borradores para el mismo tema de la cola, sobrescribirlo y enviarlo como una solicitud nueva, o puede crear una solicitud nueva desde cero.

Antes de esta mejora, Workfront solo guardaba un borrador para cada tema de la cola en la cola de solicitudes.

Para obtener información sobre cómo enviar solicitudes, consulte &quot; [Crear y enviar solicitudes de Workfront](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

## Asignar un grupo a un equipo

Para facilitar la administración y la creación de informes sobre los equipos asociados a un grupo, ahora puede asignar cualquier grupo a un equipo al que tenga acceso para editar.

Al asignar un equipo a un grupo, sus administradores de grupo pueden administrar el equipo sin ser miembros de él. En la página Detalles del equipo, pueden ver los equipos asignados a los grupos que administran. Y pueden ejecutar un informe para enumerar todos los equipos asociados con un grupo determinado.

Para obtener más información, consulte [Crear un equipo](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).

Esta característica ahora se incluye en la ruta de aprendizaje [Aspectos básicos del administrador, parte 1](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) en Workfront One.

## Los nuevos campos permiten crear informes sobre los datos de un grupo de nivel superior y todos sus subgrupos

Para ayudarle a identificar los datos asociados a un grupo de nivel superior y sus subgrupos, hemos agregado un nuevo campo Identificador de elemento principal superior que puede utilizar en Filtros, Vistas y Agrupaciones al crear informes sobre objetos de grupo.

Este campo debe ser especialmente útil para los administradores de grupo que administran grupos que contienen varios subgrupos.

Por ejemplo, imagine que administra un grupo denominado Marketing que tiene los subgrupos Marketing de campo y Marketing digital. Puede enumerar los proyectos que pertenecen a los 3 grupos creando un filtro de área de proyectos que tenga la siguiente regla de filtro:
<pre>Grupo: Nombre principal superior &gt; Igual a &gt; Marketing</pre>También hemos agregado un nuevo campo Nombre principal superior que puede utilizar para identificar los datos asociados con grupos de nivel superior en Vistas (no en Filtros o Agrupaciones).

Para obtener información acerca del uso de campos en listas e informes, consulte [Glosario de terminología de Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## Nueva opción para cancelar la acción al descartar un borrador de solicitud

Al descartar un borrador guardado, ahora puede hacer clic en Cancelar en el mensaje de confirmación que le informa de que se eliminará el borrador. De este modo, no perderá el borrador en caso de que cambie de opinión sobre su descarte.

Esta función solo está disponible en la nueva experiencia de Workfront. Para obtener más información, consulte [Crear y enviar solicitudes de Workfront](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FManage_work%2FRequests%2FCreate_Requests%2Fcreate-submit-requests.html).

