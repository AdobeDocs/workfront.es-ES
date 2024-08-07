---
content-type: release-notes
navigation-topic: product-releases-archive
title: Actividad de la versión 2018.3 de Beta 4
description: Esta página describe todos los cambios disponibles más recientemente en el entorno de vista previa con la versión Beta 4 2018.3. La funcionalidad estará disponible en el entorno de vista previa el 30 de agosto de 2018. Estará disponible en el entorno de producción en noviembre de 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: b40eda2c-8ad4-4945-a7e3-cb28ed8a14db
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1126'
ht-degree: 0%

---

# Actividad de la versión 2018.3 de Beta 4

Esta página describe todos los cambios disponibles más recientemente en el entorno de vista previa con la versión Beta 4 2018.3. La funcionalidad estará disponible en el entorno de vista previa el 30 de agosto de 2018. Estará disponible en el entorno de producción en noviembre de 2018.

Para ver una lista de todos los cambios realizados en 2018.3, consulte  [resumen de la actividad de la versión 2018.3](../../../../product-announcements/product-releases/quarterly-release-archive/2018.3-release-activity/2018-3-release-activity-overview.md).

La versión 2018.3 de Beta 4 contiene mejoras para administradores de Workfront y otros usuarios:

**Para Administradores**

* [Actualizar la estructura de informes en el perfil de usuario como administrador de grupo](#update-reporting-structure-in-the-user-profile-as-a-group-administrator) 

**Para Todos Los Usuarios**

* [Exportar más información del Planificador de recursos](#export-more-information-from-the-resource-planner)
* [Mejoras en la lista de tareas](#task-list-improvements) eliminadas de la versión
* [Mejoras en la lista de proyectos](#project-list-improvements)
* Se eliminó la edición [de la lista de tareas en el modo de edición del gráfico Gantt](#editing-the-task-list-in-gantt-chart-edit-mode) de la versión
* [Colores de herramienta de medición](#measurement-tool-colors)
* Se eliminaron [Pruebas abiertas en una nueva pestaña](#proofs-open-in-a-new-tab) de la versión

* [Mejoras en el resumen de impresión](#print-summary-enhancements)
* [Registrar el tiempo en días en la aplicación móvil de Workfront](#log-time-in-days-in-the-workfront-mobile-app)

## Actualizar la estructura de informes en el perfil de usuario como administrador de grupo {#update-reporting-structure-in-the-user-profile-as-a-group-administrator}

Los administradores de grupo ahora pueden editar los campos Subordinados directos e Subordinados directos a los usuarios de los grupos que administran.

Anteriormente, solo los administradores de Workfront y los usuarios con acceso administrativo a los usuarios tenían esta capacidad.

Para obtener información sobre los administradores de grupos, consulte [Administradores de grupos](../../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

## Exportar más información del Planificador de recursos {#export-more-information-from-the-resource-planner}

Ahora puede exportar información de hasta 52 semanas, 36 meses o 12 trimestres en el Planificador de recursos. Si la cantidad de información que está exportando es demasiado grande, recibirá un correo electrónico con el archivo exportado adjunto. El archivo está disponible para su descarga durante una semana desde el momento en que se inició la descarga.

Anteriormente, solo se podía exportar un máximo de 4 semanas, meses o trimestres a la vez.

Para obtener más información, consulte [Exportar información del Planificador de recursos](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

## Mejoras en la lista de tareas {#task-list-improvements}

>[!NOTE]
>
>* Esta función se ha eliminado del entorno de vista previa y no se incluirá en la versión 2018.3. Se publicará en una fecha posterior.

Ahora hay disponible una nueva experiencia al ver una lista de tareas. Esta experiencia incluye un mayor rendimiento, así como una navegación por listas más rápida y fluida.

También están disponibles los siguientes cambios visibles:

* Las agrupaciones se contraen de forma predeterminada.\
  Antes de este cambio, las agrupaciones se expandían de forma predeterminada.
* Se han agregado filtros rápidos a la lista de tareas.
* El encabezado de Proyecto permanece visible cuando se desplaza hacia abajo por la lista de tareas.
* Hay nuevos iconos de estado disponibles.

Se ha cambiado la siguiente funcionalidad en las listas de tareas:

* Clic con el botón derecho en la capacidad y el menú contextual que proporcionó.\
  En lugar de hacer clic con el botón derecho en las tareas para editarlas, puede hacer lo siguiente:

   * Al seleccionar una sola tarea, ahora puede utilizar el menú Más con las mismas opciones que el menú anterior del botón secundario.
   * Al seleccionar varias tareas, puede utilizar los iconos de la parte superior de la lista para realizar cualquiera de las acciones incluidas en el menú contextual anterior.

     Todos los cambios se pueden ver en las listas de tareas dentro de los proyectos, así como en la ficha Subtareas debajo de las tareas.

Para obtener más información sobre cómo trabajar en listas, consulte [Introducción a las listas en Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

Para obtener más información sobre cómo encadenar tareas en el gráfico Gantt, vea [Crear relaciones de predecesoras encadenando tareas](../../../../manage-work/tasks/use-prdcssrs/create-predecessors-by-chaining-tasks.md).

## Mejoras en la lista de proyectos {#project-list-improvements}

La capacidad de reordenar columnas se ha vuelto a añadir a una lista de proyectos en las siguientes subpestañas:

* Proyectos de mi propiedad
* Proyectos en los que participo
* Todos los proyectos

Esta funcionalidad se eliminó en la versión 2018.2.

Para obtener más información sobre cómo trabajar en listas, consulte [Introducción a las listas en Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Edición de la lista de tareas en el modo de edición del gráfico Gantt {#editing-the-task-list-in-gantt-chart-edit-mode}

>[!NOTE]
>
>* Esta función se ha eliminado del entorno de vista previa y no se incluirá en la versión 2018.3. Se publicará en una fecha posterior.

Ahora puede realizar las siguientes acciones en las tareas de un proyecto cuando se muestren en el modo de edición del gráfico Gantt:

* Añadir tareas
* Eliminar tareas
* Tareas de edición en línea

Aunque puede ver cómo afectan los cambios a la escala de tiempo del proyecto, no son inmediatos. Puede guardarlos para actualizar la cronología del proyecto o puede cancelarlos.

Anteriormente, no se podían realizar estas acciones en tareas cuando se mostraban en el modo de edición del gráfico Gantt. Puede realizar estos cambios en una lista de tareas que no se muestre en el diagrama de Gantt, pero que sean inmediatos.

Para obtener información acerca de la edición de tareas en el diagrama de Gantt, vea [Actualizar información en la lista de tareas Diagrama de Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Colores de herramienta de medición {#measurement-tool-colors}

Al utilizar la herramienta de medición para medir áreas en una prueba, ahora puede cambiar el color y la opacidad de la herramienta. Workfront recuerda esta configuración en todas las pruebas que abra hasta que vacíe la memoria caché del explorador.

El color predeterminado ahora es el rojo.

Anteriormente, la herramienta de medición solo se mostraba en azul, lo que dificultaba la visualización en pruebas de contenido que contuviera tonos de azul similares.

## Pruebas abiertas en una nueva pestaña {#proofs-open-in-a-new-tab}

>[!NOTE]
>
>* Esta función se ha eliminado del entorno de vista previa y no se incluirá en la versión 2018.3.

Cuando abre una prueba en cualquier lugar de Workfront o Workfront Proof, el visor de pruebas ahora se inicia en una nueva pestaña del explorador y el enfoque cambia a esa pestaña. Puede trabajar en varias pestañas del explorador, revisar las pruebas y continuar con su trabajo en proyectos, tareas y problemas en Workfront o Workfront Proof.

Anteriormente, el visor de revisión se iniciaba en un marco en la parte superior de la pestaña actual del explorador Workfront o Workfront Proof, por lo que no se podía acceder a esa pestaña hasta que se cerraba el visor de revisión.

Para obtener más información, consulte .

## Mejoras en Imprimir resumen {#print-summary-enhancements}

Las siguientes mejoras están ahora disponibles en la página Imprimir resumen al imprimir una prueba o guardarla como PDF o archivo XLS:

* Puede ordenar los comentarios de la prueba por creador.

  Anteriormente, se podían ordenar los comentarios en el orden en que se creaban o en el orden en que aparecían en cada página.

* Puede filtrar los comentarios de la prueba por Autor, Acción y Estado sin resolver.

  Anteriormente, el filtrado de comentarios no estaba disponible en la página de resumen de impresión.

* Ahora se incluyen las etapas, junto con los detalles sobre cada etapa.

  Anteriormente no se incluían etapas.

Para obtener más información, consulte [Imprimir un resumen de prueba en Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/print-proof-summary-in-wf.md).

## Registrar el tiempo en días en la aplicación móvil de Workfront {#log-time-in-days-in-the-workfront-mobile-app}

Ahora puede registrar el tiempo en días en la aplicación móvil de Workfront. 

Anteriormente, solo se podía registrar tiempo utilizando horas en la aplicación móvil, incluso cuando la preferencia de perfil estaba configurada para registrar tiempo en días.

Para obtener más información sobre el registro del tiempo en la aplicación móvil, consulte . 

Esta función está disponible inmediatamente para probarla con la aplicación Android Beta. 
