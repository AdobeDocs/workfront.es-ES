---
title: 20.4 Mejoras en la gestión de proyectos
description: 20.4 Mejoras en la gestión de proyectos
author: Luke
draft: Probably
feature: Product Announcements
exl-id: f21f33b3-5e49-4bb0-9eda-7cf4c016361c
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1542'
ht-degree: 0%

---

# 20.4 Mejoras en la gestión de proyectos

En esta página se describen todas las mejoras en la administración de proyectos realizadas con la versión 20.4 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción en la semana del 9 de noviembre de 2020.

Para obtener una lista de todos los cambios disponibles con la versión 20.4, consulte [Información general sobre la versión 20.4](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## Novedades para administradores: Controlar cómo se comparte un campo personalizado

Para darle un bueno control sobre quién puede editar, eliminar y utilizar los campos personalizados que cree, hemos añadido la capacidad de configurar exactamente cómo desea que se compartan.

Hasta ahora, cuando se creaba un campo personalizado, todo el sistema podía editarlo. Este sigue siendo el estado predeterminado de un campo personalizado, pero ahora puede limitar el uso compartido de un campo personalizado a ciertos usuarios, funciones, equipos, grupos y empresas. Y puede determinar si los destinatarios pueden administrar o solo ver el campo personalizado.

Además, para que esta experiencia le resulte familiar, hemos diseñado la interfaz de usuario para que esta capacidad sea similar a otras áreas de objeto que se comparten en Workfront.

Para obtener más información, consulte [Configuración del uso compartido para campos personalizados y widgets](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md).

## Novedades para administradores: Uso compartido estandarizado de formularios personalizados

Hemos estandarizado el uso compartido para Forms personalizado para que pueda utilizar el mismo proceso de uso compartido de objetos de Workfront que ya conoce. Además, la nueva experiencia de uso compartido le permite tener bueno control sobre quién puede editar, eliminar y usar el Forms personalizado que cree. Puede limitar el uso compartido de un formulario personalizado a ciertos usuarios, funciones, equipos, grupos y empresas. Y puede determinar si esos destinatarios pueden ver o administrar el formulario personalizado.

Para obtener más información, consulte [Compartir un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).

## Exportar formularios personalizados e información general de la sección Detalles de un proyecto, tarea o problema

Ahora puede exportar la información de formulario personalizada a un archivo .pdf. Los formularios personalizados se pueden exportar desde proyectos, tareas o problemas al acceder al formulario en la sección Detalles de los objetos.

Además de exportar los formularios personalizados de proyectos, tareas y problemas, ahora también puede incluir el área Información general en el pdf exportado.

Para obtener información sobre la exportación de formularios personalizados desde un objeto, consulte [Exportar formularios personalizados y detalles de objetos](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

## Agregar rápidamente una iteración

>[!NOTE]
>
>Esta función se ha eliminado temporalmente del entorno Producción. Esta página se actualizará cuando la función esté disponible.

Para simplificar la experiencia de crear una iteración, hemos agregado un nuevo botón que le permite agregar una iteración desde la pestaña iteraciones. Aquí puede crear una iteración y luego agregar tareas y problemas más tarde.

Puede seguir creando una iteración en la etiqueta de registro pendiente como antes.

Para obtener más información, consulte [Crear una iteración](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

## Nueva sección Métricas disponible en los proyectos

Para ahorrar tiempo y comprender mejor el estado general de un proyecto, ahora hay una sección Métricas disponible en un proyecto que incluye información sobre lo siguiente:

* Trabajo completo, incompleto, pendiente y próximo
* Importes de tarea y emisión agrupados por estado o prioridad
* esfuerzo de trabajo asignado a cada usuario

Puede realizar selecciones en los gráficos para ver diferentes aspectos de las tareas y los problemas en un proyecto y hacer clic en ciertos elementos para mostrar la información de la tarea.

Esta función ahora se incluye en la función [Aspectos básicos del planificador, parte 3, ruta de aprendizaje](https://one.workfront.com/s/learningpath3/planner-fundamentals-for-the-new-workfront-experience-part-3-manage-a-project-20Y0z000000bm7xEAA) en Workfront One.

## Novedades para administradores: Asignar un líder empresarial a un grupo

Para ayudarle a organizar y definir mejor sus grupos, hemos añadido la capacidad de asignar un usuario como líder empresarial para un grupo (o subgrupo). Un líder empresarial es un usuario de Workfront que toma decisiones comerciales para un grupo.

El nuevo campo Business Leader se puede utilizar en filtros de informes, vistas y agrupaciones. Por ejemplo, puede filtrar por un líder empresarial determinado para enumerar solo los grupos a los que se asigna esa persona en esa función.

Para obtener más información, consulte [Información general de Business Leader](../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md).

Esta función ahora se incluye en la función [Aspectos básicos del administrador, parte 1, ruta de aprendizaje](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) en Workfront One.

## Novedades para administradores: Asociar portafolios, programas y empresas con grupos

Cuando los administradores de Workfront crean o editan un portafolio, programa o empresa, pueden asignarlo a un grupo. Con los grupos asignados a estos objetos, es fácil identificar las responsabilidades de su grupo para ellos.

Por ejemplo, puede enumerar todas las carteras de su organización en un informe y mirar la columna Grupo para ver en qué carteras está trabajando su grupo.

Para obtener más información, consulte la sección &quot;Acerca de la asociación de un grupo con un objeto&quot; en el artículo [Información general sobre grupos](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

Esta función ahora se incluye en la función [Aspectos básicos del administrador, parte 1, ruta de aprendizaje](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) en Workfront One.

## Novedades para administradores: Los administradores de un grupo asignado a una empresa pueden administrar la empresa

Hemos facilitado a un administrador de grupos la administración de una empresa asociada a su grupo en Workfront. El acceso para administrar la empresa está disponible automáticamente cuando se crea la asociación. Esto es especialmente importante cuando el administrador del grupo no tiene acceso administrativo a las empresas.

Para obtener más información, consulte [Crear y editar empresas](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

Para obtener información sobre el acceso administrativo a las empresas, consulte [Conceder a los usuarios acceso administrativo a determinadas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Esta función ahora se incluye en la función [Aspectos básicos del administrador, parte 1, ruta de aprendizaje](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) en Workfront One.

## Reemplazar el botón Trabajar en él con un botón Inicio

Para ayudar a capturar la fecha y hora en que el trabajo se inicia en un elemento de trabajo, los usuarios pueden reemplazar el botón Trabajar en él con un botón Inicio que actualiza automáticamente el estado y la Fecha de inicio real del elemento de trabajo.

Actualizado el 24 de septiembre: Después de hacer clic en Iniciar tarea o en Iniciar problema, ahora tiene la opción de revertir su elección e indicar que puede que no esté listo para empezar a trabajar en un elemento de trabajo haciendo clic en Deshacer. El elemento de trabajo vuelve al estado Nuevo y se eliminan la Fecha de confirmación y la Fecha de inicio real. La opción Deshacer se muestra durante un período de tiempo muy breve y se borra después de salir de la página o de actualizarla.

Para obtener más información sobre la configuración de esta opción, consulte [Reemplazar el botón Trabajar en él con un botón Inicio](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

Esta función ahora se incluye en la función [Ruta de aprendizaje de fundamentos del trabajo](https://one.workfront.com/s/learningpath3/worker-fundamentals-for-the-new-workfront-experience-20Y0z000000blg8EAA) y [Aspectos básicos del administrador, parte 1, ruta de aprendizaje](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) en Workfront One.

## Permitir varios borradores para un tema de cola

Para darle más libertad al trabajar con solicitudes, ya no hay límite para cuántos borradores se pueden guardar para un tema de cola. Al crear una solicitud nueva, puede seleccionar un borrador existente de una lista de borradores para el mismo tema de cola, sobrescribirlo y enviarlo como una solicitud nueva o puede crear una solicitud nueva desde cero.

Antes de esta mejora, Workfront solo guardó un borrador para cada tema de cola en la cola de solicitudes.

Para obtener información sobre el envío de solicitudes, consulte &quot; [Crear y enviar solicitudes de Workfront](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

## Asignar un grupo a un equipo

Con el fin de facilitar la gestión y el informe de los equipos asociados a un grupo, ahora puede asignar cualquier grupo a un equipo al que tenga acceso para editarlo.

Cuando asigna un equipo a un grupo, sus administradores de grupo pueden administrarlo sin ser miembros de él. En la página Detalles del equipo , pueden ver los equipos asignados a los grupos que administran. Y pueden ejecutar un informe para enumerar todos los equipos asociados a un grupo determinado.

Para obtener más información, consulte [Crear un equipo](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).

Esta función ahora se incluye en la función [Aspectos básicos del administrador, parte 1, ruta de aprendizaje](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) en Workfront One.

## Los nuevos campos le permiten informar sobre los datos de un grupo de nivel superior y de todos sus subgrupos

Para ayudarle a identificar los datos asociados con un grupo de nivel superior y sus subgrupos, se ha añadido un nuevo campo de ID principal que puede utilizar en Filtros, Vistas y Agrupaciones al crear informes sobre objetos de grupo.

Este campo debe ser especialmente útil para los administradores de grupo que administran grupos que contienen varios subgrupos.

Por ejemplo, imaginemos que administra un grupo llamado Marketing que tiene los subgrupos Marketing de campo y Marketing digital. Puede enumerar los proyectos que pertenecen a los 3 grupos creando un filtro de área de Proyectos que tenga la siguiente regla de filtro:
<pre>Grupo: Nombre principal &gt; Igual &gt; Marketing</pre>También se ha agregado un nuevo campo Nombre principal superior que puede utilizar para identificar los datos asociados con los grupos de nivel superior en Vistas (no en Filtros ni Agrupaciones).

Para obtener información sobre el uso de campos en listas e informes, consulte [Glosario de terminología de Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## Nueva opción para cancelar la acción al descartar un borrador de solicitud

Al descartar un borrador guardado, ahora puede hacer clic en Cancelar en el mensaje de confirmación que le informa de que el borrador se eliminará. De esta manera, no pierdes el borrador en caso de que cambies de idea sobre descartarlo.

Esta función solo está disponible en la nueva experiencia de Workfront. Para obtener más información, consulte [Crear y enviar solicitudes de Workfront](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FManage_work%2FRequests%2FCreate_Requests%2Fcreate-submit-requests.html).

