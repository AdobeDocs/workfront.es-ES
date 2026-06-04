---
title: 22.4 Mejoras del proyecto
description: 22.4 Mejoras del proyecto
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 41372dd8-5002-4f8b-a5ac-a577c8b05d11
TQID: https://experienceleague.adobe.com/h42aq8ShyeC-mZrt8JlpHYFGfgml9HQ2vWHI0-Op-io
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 965
ht-degree: 97%

---

# 22.4 Mejoras del proyecto

Esta página describe todas las mejoras del proyecto realizadas con la versión 22.4 en el entorno de vista previa. Estas mejoras estarán disponibles la semana del 3 de octubre de 2022.

Para obtener una lista de todos los cambios disponibles con la versión 22.4, consulte [Información general de la versión 22.4](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## Ya están disponibles los detalles de la predecesora

Para ver los detalles de las predecesoras de una tarea, ahora puede pasar el puntero por encima de número de predecesoras en la columna Predecesoras. El cuadro de detalles muestra la tarea predecesora y el proyecto al que se hace referencia, las fechas de inicio y finalización planificadas de la tarea predecesora y el número de predecesoras y sucesoras de la tarea predecesora. Puede expandir los detalles del proyecto para ver más información sobre él. Se incluye información adicional para las predecesoras entre proyectos.

Para obtener más información, consulte [Crear una relación de predecesora en la lista de tareas](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

## Asignar varios equipos a una tarea o un problema

Para darle mucha más flexibilidad en la forma en que administra las tareas y los problemas, hemos hecho posible que se asignen varios equipos a una tarea o un problema. Anteriormente, solo se podía asignar un equipo a una tarea o un problema.

>[!NOTE]
>
>Actualmente, esta funcionalidad no está disponible en el Distribuidor de cargas de trabajo en el área de Equipos.

Para obtener más información, consulte [Asignar tareas](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md) y [Asignar problemas](/help/quicksilver/manage-work/issues/manage-issues/assign-issues.md).

## Selección inteligente de usuarios para las funciones de proyecto en las áreas de edición y detalles

Hemos mejorado la forma en que se muestran los usuarios cuando los añade a los siguientes campos de proyecto desde el cuadro Editar y la sección Detalles del proyecto:

* Propietario del proyecto

* Patrocinador de proyecto

* Gerente de recursos

Ahora, cuando añada un usuario a cualquiera de estos campos en las áreas de Edición o Detalles, además de su nombre y avatar, también se mostrarán su función principal y su correo electrónico. Esto ayuda a distinguir entre varios usuarios con nombres similares o idénticos.

Para obtener más información, consulte [Editar proyectos](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

NOTA: En futuras versiones, se actualizarán los campos de usuario adicionales para proyectos, tareas y problemas con esta funcionalidad.

[Vea un vídeo de demostración de esta función.](https://video.tv.adobe.com/v/3412390/){target=_blank}

## Los campos de fecha calculados siempre se guardan en función de la Hora Universal Coordinada (UTC)

Ahora puede estar seguro de que todas las funciones de fecha de los campos calculados funcionan de forma coherente y producen el mismo resultado para todos, independientemente de cómo se actualice una expresión de datos personalizados o de dónde estén colaborando los usuarios en el objeto en todo el mundo.

Ahora, todos los cálculos se calculan y guardan según un único estándar, la hora universal coordinada (UTC), y no según las configuraciones de zona horaria establecidas para la instancia de su organización y el perfil de usuario individual. Sin embargo, los cálculos se muestran en un formulario personalizado basado en las zonas horarias individuales de cada usuario establecidas en su explorador.

Anteriormente, la configuración del tiempo en los cálculos se prestaba a confusión cuando variaba en los siguientes casos:

* Si alguien recalculaba una expresión de campo calculada usando “Actualizar cálculos anteriores” en el generador de formularios, los resultados de la función de fecha se determinaban según la zona horaria UTC de su organización.

* Si alguien editaba el objeto y eso hacía que la expresión del campo calculado se volviera a calcular los resultados de la función de fecha se determinaban en función de la zona horaria local del usuario. Los resultados de los campos de fecha calculados en este escenario también se calcularán según la UTC.

Para obtener más información, consulte [Trabajar en diferentes zonas horarias](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

## Mejoras en los formularios personalizados: Adobe XD y el filtro rápido

En función de sus comentarios, hemos introducido las siguientes mejoras para mejorar su experiencia al administrar formularios personalizados:

* Añada un archivo Adobe XD para que un formulario personalizado sea más visual e informativo. Cuando el formulario se adjunta a un objeto, los usuarios que trabajan con el objeto pueden ver el archivo XD e interactuar con él desde el formulario.


* Utilice el Filtro rápido para localizar fácilmente elementos en la lista de campos y formularios personalizados modernizados. Disfrute también de un aspecto mejorado al administrar sus formularios y campos.

  Para obtener más información acerca del Filtro rápido, consulte [Aplicar el filtro rápido a una lista](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

[Vea un vídeo de demostración de esta función.](https://video.tv.adobe.com/v/3412469/){target=_blank}

## Versión beta pública: nueva experiencia de filtro para proyectos, tareas y problemas

El filtrado en las listas de proyectos, tareas y problemas se ha rediseñado para ayudarle a crear y compartir filtros rápidamente. Las funciones incluyen las siguientes:

* Una interfaz intuitiva del “generador Beta” para crear un nuevo filtro

* La posibilidad de marcar un filtro como favorito

* El apilado de filtros (aplicar más de un filtro guardado)

* La duplicación de filtros

* Compartir filtros

* Quitar filtros compartidos con usted


La nueva experiencia de filtro también está disponible en las listas de plantillas de horas y en el planificador de escenarios.

El modo Texto permanece disponible para la edición avanzada de filtros y los administradores del sistema pueden asignar filtros predeterminados para todos los usuarios a través de las plantillas de diseño.

### ¿Dónde estará esto disponible?

* Listas de proyectos/tareas/problemas

* Planificador de escenarios

* Hojas de horas


### Necesitamos sus comentarios.

Con esta versión Beta pública, los usuarios tienen la oportunidad de enviar comentarios directamente al equipo que trabaja en la experiencia de los filtros haciendo clic en el botón de comentarios. Esperamos recibir noticias suyas y de sus usuarios sobre la nueva experiencia de filtro en la versión beta pública. Si su equipo desea reunirse directamente con el producto para proporcionar comentarios adicionales, no dude en programar una reunión aquí: https://calendly.com/wf-product-and-design-research/filtersfeedbackpublicbeta?month=2022-08&amp;date=2022-08-25

### ¿Qué es lo próximo?

* Nueva experiencia de agrupaciones y vistas (también conocida como columnas)

  Empezaremos a trabajar en la nueva experiencia para agrupaciones y vistas (también conocida como columnas), de modo que sea coherente con la nueva experiencia de filtros y tenga algunas de las mismas características interesantes que la nueva experiencia de filtros.

* Implementar nuevos filtros en otras áreas de Adobe Workfront

  Trabajaremos con los equipos de todo el producto para implementar la nueva experiencia de filtros en otras áreas de Workfront.


Queremos ofrecerle valor de forma iterativa, por eso seguiremos ofreciendo nuevas experiencias y otras áreas a medida que vayan estando listas. Manténgase pendiente para ir conociendo otras actualizaciones interesantes.

Para obtener más información, consulte [Información general de filtros](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md) y [Crear o editar filtros en Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

[Vea un vídeo de demostración de esta función.](https://video.tv.adobe.com/v/3412391/)
