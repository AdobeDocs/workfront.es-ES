---
title: 22.4 Mejoras del proyecto
description: 22.4 Mejoras del proyecto
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 41372dd8-5002-4f8b-a5ac-a577c8b05d11
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 2%

---

# 22.4 Mejoras del proyecto

Esta página describe todas las mejoras de Project realizadas con la versión 22.4 en el entorno de vista previa. Estas mejoras estarán disponibles la semana del 3 de octubre de 2022.

Para obtener una lista de todos los cambios disponibles con la versión 22.4, consulte [Información general de la versión 22.4](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## Ya están disponibles los detalles de la predecesora

Para ver los detalles de las tareas predecesoras de una tarea, ahora puede situar el cursor sobre el número de predecesora en la columna Predecesoras. El cuadro de detalles muestra la tarea y el proyecto predecesores a los que se hace referencia, las fechas de inicio y finalización planificadas de la tarea predecesora y el número de predecesoras y sucesoras de la tarea predecesora. Puede expandir los detalles del proyecto para ver más información sobre él. Se incluye información adicional para las tareas predecesoras entre proyectos.

Para obtener más información, consulte [Crear una relación de predecesoras en la lista de tareas](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

## Asignar varios equipos a una tarea o un problema

Para darle mucha más flexibilidad en la forma en que administra las tareas y los problemas, hemos permitido asignar varios equipos a una tarea o un problema. Anteriormente, solo se podía asignar un equipo a una tarea o un problema.

>[!NOTE]
>
>Actualmente, esta funcionalidad no está disponible en el Distribuidor de cargas de trabajo en el área de Equipos.

Para obtener más información, consulte [Asignar tareas](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md) y [Asignar problemas](/help/quicksilver/manage-work/issues/manage-issues/assign-issues.md).

## Selección inteligente de usuarios para las funciones de proyecto en las áreas Editar y Detalles

Hemos mejorado la forma en que se muestran los usuarios al agregarlos a los siguientes campos de proyecto desde el cuadro Editar y la sección Detalles del proyecto:

* Propietario del proyecto

* Patrocinador de proyecto

* Gerente de recursos

Ahora, cuando agregue un usuario a cualquiera de estos campos en las áreas Editar o Detalles, además de su nombre y avatar, también se mostrarán su función principal y su correo electrónico. Esto ayuda a distinguir entre varios usuarios con nombres similares o idénticos.

Para obtener más información, consulte [Editar proyectos](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

NOTA: En futuras versiones, se actualizarán los campos de usuario adicionales para proyectos, tareas y problemas con esta funcionalidad.

[Vea un vídeo de demostración de esta función.](https://video.tv.adobe.com/v/3412390/){target=_blank}

## Los campos de fecha calculados siempre se guardan en función de la hora universal coordinada (UTC)

Ahora puede estar seguro de que todas las funciones de fecha de los campos calculados funcionan de forma coherente y producen el mismo resultado para todos, independientemente de cómo se actualice una expresión de datos personalizada o de dónde colaboren los usuarios en el objeto en todo el mundo.

Ahora, todos los cálculos se calculan y guardan según un estándar (hora universal coordinada (UTC)), no según las configuraciones de zona horaria establecidas para la instancia de su organización y el perfil de usuario individual. Sin embargo, los cálculos se muestran en un formulario personalizado basado en las zonas horarias individuales de cada usuario establecidas en el explorador.

Anteriormente, la configuración de tiempo en los cálculos causaba confusión cuando variaba en estas situaciones:

* Si alguien recalculó una expresión de campo calculado usando &quot;Actualizar cálculos anteriores&quot; en el generador de formularios, los resultados de las funciones de fecha estaban determinados por la zona horaria UTC de su organización.

* Si alguien editó el objeto y eso hizo que la expresión del campo calculado se recalculara, los resultados de la función de fecha estaban determinados por la zona horaria local del usuario. Los resultados de los campos de fecha calculados en este escenario también se calcularán según la fecha UTC.

Para obtener más información, consulte [Trabajo entre zonas horarias](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

## Mejoras en los formularios personalizados: Adobe XD y el filtro rápido

En función de sus comentarios, hemos introducido las siguientes mejoras para mejorar su experiencia al administrar formularios personalizados:

* Agregue un archivo Adobe XD para que un formulario personalizado sea más visual e informativo. XD Cuando el formulario está adjunto a un objeto, los usuarios que trabajan con el objeto pueden ver el archivo de datos e interactuar con él desde el formulario.

  Para obtener más información, consulte [Agregar o editar una imagen u otro widget de recursos en un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

* Utilice el Filtro rápido para localizar fácilmente elementos en la lista de campos y formularios personalizados modernizados. Además, disfrute de una apariencia mejorada al administrar los formularios y campos.

  Para obtener más información sobre el Filtro rápido, consulte [Aplicar el filtro rápido a una lista](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

[Vea un vídeo de demostración de esta función.](https://video.tv.adobe.com/v/3412469/){target=_blank}

## Versión beta pública: nueva experiencia de filtro para proyectos, tareas y problemas

El filtrado en las listas de proyectos, tareas y problemas se ha rediseñado para ayudarle a crear y compartir filtros rápidamente. Las funciones incluyen:

* Una interfaz intuitiva del &quot;generador beta&quot; para crear un nuevo filtro

* La capacidad de marcar un filtro como favorito

* Apilamiento de filtros (aplicar más de un filtro guardado)

* Duplicación de filtros

* Compartir filtros

* Eliminación de filtros compartidos con usted


La nueva experiencia de filtrado también está disponible en las listas de plantillas de horas y en el Scenario Planner.

El modo Texto permanece disponible para la edición avanzada de filtros y los administradores del sistema pueden asignar filtros predeterminados para todos los usuarios a través de las plantillas de diseño.

### ¿Dónde estará disponible?

* Listas de proyectos/tareas/problemas

* Planificador de escenarios

* Hojas de horas


### Queremos sus comentarios.

Con esta versión beta pública, los usuarios tienen la oportunidad de enviar comentarios directamente al equipo que trabaja en la experiencia de los filtros haciendo clic en el botón de comentarios. Esperamos recibir noticias suyas y de sus usuarios sobre la nueva experiencia de filtrado en la versión beta pública. Si su equipo desea reunirse directamente con el producto para proporcionar comentarios adicionales, no dude en programar una reunión aquí: https://calendly.com/wf-product-and-design-research/filtersfeedbackpublicbeta?month=2022-08&amp;date=2022-08-25

### ¿Cuál es el siguiente paso?

* Nueva experiencia de agrupaciones y vistas (también conocida como columnas)

  Empezaremos a trabajar en la nueva experiencia para agrupaciones y vistas (también conocida como columnas), de modo que sea coherente con la nueva experiencia de filtros y tenga algunas de las mismas características interesantes que la nueva experiencia de filtros.

* Implementar nuevos filtros en otras áreas de Adobe Workfront

  Trabajaremos con equipos de todo el producto para implementar la nueva experiencia de filtros en otras áreas de Workfront.


Queremos ofrecerle valor de forma iterativa para que podamos seguir ofreciendo a medida que las nuevas experiencias y otras áreas estén listas. Manténgase al pendiente de actualizaciones más interesantes.

Para obtener más información, consulte [Resumen de filtros](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md) y [Creación o edición de filtros en Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

[Vea un vídeo de demostración de esta función.](https://video.tv.adobe.com/v/3412391/)
