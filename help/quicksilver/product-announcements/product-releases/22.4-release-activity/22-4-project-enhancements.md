---
title: 22.4 Mejoras del proyecto
description: 22.4 Mejoras del proyecto
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 41372dd8-5002-4f8b-a5ac-a577c8b05d11
source-git-commit: 6cd6b1433fb56b92872f0ad80bb1a700fc0854cc
workflow-type: tm+mt
source-wordcount: '967'
ht-degree: 2%

---

# 22.4 Mejoras del proyecto

En esta página se describen todas las mejoras del proyecto realizadas con la versión 2.4 del entorno de vista previa. Estas mejoras estarán disponibles la semana del 3 de octubre de 2022.

Para obtener una lista de todos los cambios disponibles con la versión 2.4, consulte [Resumen de la versión 2.4](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## Los detalles del predecesor ya están disponibles

Para ver los detalles de los predecesores de una tarea, ahora puede pasar el ratón sobre el número predecesor en la columna Predecesores . El cuadro de detalles muestra la tarea predecesora y el proyecto al que se hace referencia, las fechas de inicio y finalización planificadas para la tarea predecesora y el número de predecesores y sucesores de la tarea predecesora. Puede ampliar los detalles del proyecto para obtener más información sobre él. Se incluye información adicional para los predecesores entre proyectos.

Para obtener más información, consulte [Crear una relación predecesora en la lista de tareas](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

## Asignar varios equipos a una tarea o problema

Para darle mucha más flexibilidad en la forma en que gestiona las tareas y los problemas, hemos hecho posible asignar varios equipos a una tarea o problema. Anteriormente, solo se podía asignar un equipo a una tarea o problema.

>[!NOTE]
>
>Actualmente, esta funcionalidad no está disponible en el equilibrador de carga de trabajo del área Equipos .

Para obtener más información, consulte [Asignación de tareas](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md) y [Asignación de problemas](/help/quicksilver/manage-work/issues/manage-issues/assign-issues.md).

## Selección inteligente de usuarios para funciones de proyecto en las áreas Editar y Detalles

Hemos mejorado la forma en que se muestran los usuarios al agregarlos a los siguientes campos de proyecto desde el cuadro Editar y la sección Detalles del proyecto:

* Propietario del proyecto

* Patrocinador de proyecto

* Gerente de recursos

Ahora, cuando agrega un usuario a cualquiera de estos campos en las áreas Editar o Detalles, además de su nombre y avatar, también se muestran su Función principal y su correo electrónico. Esto ayuda a distinguir entre varios usuarios con nombres similares o idénticos.

Para obtener más información, consulte [Editar proyectos](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

NOTA: En futuras versiones se actualizarán campos de usuario adicionales para proyectos, tareas y problemas.

[Vea una demostración en vídeo de esta función.](https://video.tv.adobe.com/v/3412390/){target=_blank}

## Los campos de fecha calculada siempre se guardan en función de la hora universal coordinada (UTC)

Ahora, puede estar seguro de que todas las funciones de fecha de los campos calculados funcionan de forma coherente y producen el mismo resultado para todos, independientemente de cómo se actualice una expresión de datos personalizada o de dónde estén colaborando los usuarios en el objeto en todo el mundo.

Ahora, todos los cálculos se calculan y guardan de forma estándar (el tiempo universal coordinado (UTC)), no según las configuraciones de zona horaria establecidas para la instancia de su organización y su perfil de usuario individual. Sin embargo, los cálculos se muestran en un formulario personalizado basado en las zonas horarias individuales de cada usuario establecidas en su explorador.

Anteriormente, la configuración de tiempo en los cálculos provocaba confusión cuando variaban en estas situaciones:

* Si alguien volvió a calcular una expresión de campo calculada mediante &quot;Actualizar cálculos anteriores&quot; en el generador de formularios, la zona horaria UTC de su organización determinaba los resultados de la función de fecha.

* Si alguien editó el objeto y eso causó que la expresión de campo calculado se volviera a calcular, la zona horaria local del usuario determinaba los resultados de la función de fecha. Los resultados de los campos de fecha calculada en este escenario también se calcularán en función de la UTC.

Para obtener más información, consulte [Trabajo en zonas horarias](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

## Mejoras en los formularios personalizados: Adobe XD y el filtro rápido

En función de sus comentarios, hemos introducido las siguientes mejoras para mejorar su experiencia al administrar formularios personalizados:

* Añada un archivo Adobe XD para que un formulario personalizado sea más visual e informativo. Cuando el formulario está adjunto a un objeto, los usuarios que trabajen con él pueden ver e interactuar con él desde el formulario.

   Para obtener más información, consulte [Agregar o editar una imagen u otro widget de recursos en un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

* Utilice el filtro rápido para localizar fácilmente elementos en la lista de campos y formularios personalizados modernizados. Disfrute también de una apariencia mejorada mientras gestiona sus formularios y campos.

   Para obtener más información sobre el Filtro rápido, consulte [Aplicar el filtro rápido a una lista](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

[Vea una demostración en vídeo de esta función.](https://video.tv.adobe.com/v/3412469/){target=_blank}

## Versión beta pública: nueva experiencia de filtro para proyectos, tareas y problemas

El filtrado en las listas de proyectos, tareas y problemas se ha rediseñado para ayudarle a crear y compartir filtros rápidamente. Las funciones incluyen:

* Una interfaz intuitiva del &quot;generador beta&quot; para crear un nuevo filtro

* La capacidad de marcar un filtro como favorito

* Apilamiento de filtros (aplicar más de un filtro guardado)

* Duplicación de filtros

* Compartir filtros

* Eliminación de filtros compartidos con usted


La nueva experiencia de filtro también está disponible en listas de hojas de horas y en el planificador de escenarios.

El modo de texto permanece disponible para la edición avanzada de filtros, y los administradores del sistema aún pueden asignar filtros predeterminados para todos los usuarios a través de las plantillas de diseño.

### ¿Dónde estará disponible?

* Listas de proyectos/tareas/problemas

* Planificador de escenarios

* Plantillas de horas


### ¡Queremos tus comentarios!

Con esta beta pública, los usuarios tienen la oportunidad de enviar comentarios directamente al equipo que trabaja en la experiencia de filtros haciendo clic en el botón de comentarios. Esperamos con interés recibir de usted y de sus usuarios información sobre la nueva experiencia de filtrado en la versión beta pública. Si su equipo desea reunirse directamente con el producto para proporcionar comentarios adicionales, no dude en programar una reunión aquí: https://calendly.com/wf-product-and-design-research/filtersfeedbackpublicbeta?month=2022-08&amp;date=2022-08-25

### ¿Qué sigue?

* Experiencia de nuevos grupos y vistas (también conocidos como columnas)

   Empezaremos a trabajar en la nueva experiencia para agrupaciones y vistas (también conocidas como columnas), de modo que sea coherente con la nueva experiencia de filtros y tenga algunas de las mismas buenas características que la nueva experiencia de filtros.

* Implementar nuevos filtros en otras áreas de Adobe Workfront

   Trabajaremos con equipos de todo el producto para implementar la nueva experiencia de filtros en otras áreas en Workfront.


Queremos ofrecerle valor de forma iterativa, de modo que seguiremos ofreciendo las nuevas experiencias y otras áreas estén listas. Manténgase atento a las actualizaciones más emocionantes.

Para obtener más información, consulte [Información general sobre filtros en Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md) y [Crear o editar filtros en Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

[Vea una demostración en vídeo de esta función.](https://video.tv.adobe.com/v/3412391/)
